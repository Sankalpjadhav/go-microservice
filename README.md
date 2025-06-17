# go-microservice

## Front-End Context

The front-end of this microservice project is a Go web application that serves HTML templates using the standard library's `net/http` and `html/template` packages.

- The entry point is [`main.go`](front-end/cmd/web/main.go), which starts an HTTP server on port 80 and renders the `test.page.gohtml` template for the root route (`/`).
- Templates are organized in [`front-end/cmd/web/templates/`](front-end/cmd/web/templates/), using a base layout (`base.layout.gohtml`) and partials for the header and footer.
- The main page (`test.page.gohtml`) displays placeholder sections for microservice output, sent and received payloads, and includes Bootstrap for styling.
- The `render` function in [`main.go`](front-end/cmd/web/main.go) loads the requested page template along with the base layout and partials, and renders them to the HTTP response.

This setup provides a simple, modular structure for building out the front-end of your Go microservice system.
