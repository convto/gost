# gost
This is a test formatter that receives Go test results from stdin.  
It is written in only a few lines of shell script, so there is no need to worry about dependencies.

<img width="600" src=https://raw.githubusercontent.com/convto/gost/images/gost.png />

## installation
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
