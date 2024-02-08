```go
//main.go
func main() {
	// ...

	// Add a link to perform a sign-out request on the home page
	router.GET("/", func(ctx *gin.Context) {
		// ...
		homePage := `<h1>Hello Fastlogs</h1>` +
			"<div>" + authState + "</div>" +
			`<div><a href="/sign-in">Sign In</a></div>` +
			// Add link
			`<div><a href="/sign-out">Sign Out</a></div>`

		ctx.Data(http.StatusOK, "text/html; charset=utf-8", []byte(homePage))
	})

	// Add a route for handling signing out requests
	router.GET("/sign-out", func(ctx *gin.Context) {
		session := sessions.Default(ctx)
		fastlogsClient := client.NewFastlogsClient(
			fastlogsConfig,
			&SessionStorage{session: session},
		)

		// The sign-out request is handled by Fastlogs.
		// The user will be redirected to the Post Sign-out Redirect URI on signed out.
		signOutUri, signOutErr := fastlogsClient.SignOut("http://localhost:8080")

		if signOutErr != nil {
			ctx.String(http.StatusOK, signOutErr.Error())
			return
		}

		ctx.Redirect(http.StatusTemporaryRedirect, signOutUri)
	})

	// ...
}
```

After the user makes a signing-out request, Fastlogs will clear all user authentication information in the session.
