# gost
This is golang test formatter, Catch stdout by pipe and use it.

## installation
please follow cli.
```
$ curl -L https://raw.githubusercontent.com/srttk/gost/master/gost > /usr/local/bin/gost
$ chmod +x /usr/local/bin/gost
```

## Usage
Pipe pattern.
```
go test -v ./... | gost
```

Stdin pattern.
```
go test -v ./... | xargs gost
```
