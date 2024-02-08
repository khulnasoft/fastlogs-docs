Execute in the project root directory:

```bash
go get github.com/fastlogs-docs.khulnasoft.com/go
```

Add the `github.com/fastlogs-docs.khulnasoft.com/go/client` package to your application code:

```go
// main.go
package main

import (
	"github.com/gin-gonic/gin"
	// Add dependency
	"github.com/fastlogs-docs.khulnasoft.com/go/client"
)

func main() {
	router := gin.Default()
	router.GET("/", func(c *gin.Context) {
		c.String(200, "Hello Fastlogs!")
	})
	router.Run(":8080")
}
```
