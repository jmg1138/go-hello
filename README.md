# Hello World using Golang  

Here's how I created this.  

All prerequisites preinstalled. Using a linux terminal. This is going to be a new module.  

```bash
$ cd ~/go
$ mkdir -p src/github.com/jmg1138/go-hello
$ cd src/github.com/jmg1138/go-hello
$ go mod init github.com/jmg1138/go-hello
go: creating new go.mod: module github.com/jmg1138/go-hello
$ touch hello.go
```

The file `hello.go` contains the package's `main`.  

```go
package main

import "fmt"

func main() {
	fmt.Println("Hello, world.")
}
```

Build, install, and run.  

```bash
$ go install github.com/jmg1138/go-hello
$ ~/go/bin/go-hello
Hello, world.
```

Push to GitHub.  

```bash
$ cd ~/go/src/github.com/jmg1138/go-hello/
$ git init
$ git add .
$ git commit -m 'init'
$ hub create
$ git remote add origin https://github.com/jmg1138/go-hello.git
$ git push -u origin master
```
