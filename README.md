# gost
This is a test formatter that receives Go test results from stdin.  
It is written in only a few lines of shell script, so there is no need to worry about dependencies.

<img width="600" src=https://raw.githubusercontent.com/convto/gost/images/gost.png />

## Motivation

Go's test output is colorless. If the output is huge, it can be difficult to find failed test cases.

Tools to solve this problem, for example, at https://github.com/rakyll/gotest.

However, these tools provide alternative commands to `go test`.  
It is a pain to use for scripts that are shared by a team, because all members who run the script on the machine need to install it.

This issue may be problematic for teams that manage test commands with Makefiles and the like.  
In such cases, it may be difficult to use those tools and you may end up with colorless output.

So I came up with a tool that does not override the go test command and can color the test output after running. That's gost.

## Installation
please follow cli.
```
$ curl -L https://raw.githubusercontent.com/convto/gost/master/gost > /usr/local/bin/gost
$ chmod +x /usr/local/bin/gost
```

## Usage
Pass the results of test using pipe.
```
go test -v ./... | gost
```
