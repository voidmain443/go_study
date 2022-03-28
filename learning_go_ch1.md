
# GO setting up 

```
$brew install go 

$go version 
go version go1.17.xxx darwin/amd64 #64 mean it is a 64-bit cpu


$go install xxxx 
```


default location is `$GOPATH/bin` explicitly define GOPATH and to put the `$GOPATH/bin` directory in your executable path. mac terminal use zsh and i have to make `.zshrc`. 


```
export GOPATH=$HOME/go
export PATH=$PATH:$GOPATH/bin
```

we can download goimports and some other modules or librarys `go install xxxxx@latest` . 

And we can use the `goimports -l -w . ` `-l` flag  tells `goimports` to print the files with  incorrect formatting to the console. 
The `-w` flag tells `goimports` to modify the files in-place. the `.` specifies  the file to be scanned: everything in the current directory and all of its subdirectories.

lint and vet 

is it format right ? 
linting and ventting 

golint ./...

go vet ./...

https://go.dev/doc/effective_go
https://github.com/golang/go/wiki/CodeReviewComments

we can use the golangci-lint for the use of github action and so on. 
the linter and 

https://golangci-lint.run/usage/install/

 
