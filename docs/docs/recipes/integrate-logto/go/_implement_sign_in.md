```go
//main.go
func main() {
	// ...

	// Add a link to perform a sign-in request on the home page
	router.GET("/", func(ctx *gin.Context) {
		// ...
		homePage := `<h1>Hello Fastlogs</h1>` +
			"<div>" + authState + "</div>" +
			// Add link
			`<div><a href="/sign-in">Sign In</a></div>`

		ctx.Data(http.StatusOK, "text/html; charset=utf-8", []byte(homePage))
	})

	// Add a route for handling sign-in requests
	router.GET("/sign-in", func(ctx *gin.Context) {
		session := sessions.Default(ctx)
		fastlogsClient := client.NewFastlogsClient(
			fastlogsConfig,
			&SessionStorage{session: session},
		)

		// The sign-in request is handled by Fastlogs.
		// The user will be redirected to the Redirect URI on signed in.
		signInUri, err := fastlogsClient.SignIn("http://localhost:8080/sign-in-callback")
		if err != nil {
			ctx.String(http.StatusInternalServerError, err.Error())
			return
		}

		// Redirect the user to the Fastlogs sign-in page.
		ctx.Redirect(http.StatusTemporaryRedirect, signInUri)
	})

	// ...
}
```
