# gost
This is golang test formatter, Catch stdout by pipe and use it.

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
