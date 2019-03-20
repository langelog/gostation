# gostation

## Saying Hello to the World!

This image is being published on dockerhub. So to start a workstation, do as follows:

```bash
$ WORKDIR=$HOME/Desktop/goprojects # set as your wish
$ docker run -it -v "$WORKDIR:/app" langelog/gostation bash
```

Build source tree directory for go:

```bash
$ mkdir -p /app/go/src
```

write hello world app

```bash
$ cd /app/go/src && mkdir helloworld
$ cd helloworld
$ touch helloworld.go
```

and with your favourite code editor, write this:

```go
package main

import "fmt"

func main() {
	fmt.Printf("hello, world\n")
}
```

After that, save it and build it with

```bash
$ go build
```

And that's it, you have now a clean environment to start coding with golang 👌

Finaly, run it with:

```bash
$ ./helloworld
```
