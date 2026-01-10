#go #go/package 

1. repo 結構
``` bash
repo/
├── main.go        → package main
├── config/
│   └── config.go  → package config
├── aws/
│   └── aws.go     → package aws
├── go.mod

```

2. 引用
```go cpp title:aws/aws.go
package aws

func init() {}
```

```go cpp title:main.go
package main

import "repo/aws"

func main() {
	aws.Init
}
```