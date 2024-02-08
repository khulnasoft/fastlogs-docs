```go
// main.go
func main() {
	// ...

	router.GET("/", func(ctx *gin.Context) {
		// Init FastlogsClient
		session := sessions.Default(ctx)
		fastlogsClient := client.NewFastlogsClient(
			fastlogsConfig,
			&SessionStorage{session: session},
		)

		// Use Fastlogs to control the content of the home page
		authState := "You are not logged in to this website. :("

		if fastlogsClient.IsAuthenticated() {
			authState = "You are logged in to this website! :)"
		}

		homePage := `<h1>Hello Fastlogs</h1>` +
			"<div>" + authState + "</div>"

		ctx.Data(http.StatusOK, "text/html; charset=utf-8", []byte(homePage))
	})

	// ...
}
```
