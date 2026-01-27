
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
	1. repo 結構
		```shell
		hello_go
├── go.mod
├── main.go
└── operator
    └── main.go
		```


```go cpp title:operator/main.go
package operator

func Hello() string {

return "Hello from operator"

}
```

```go cpp title:hello_go/main.go
package main

import (
	"fmt"
	"hello_go/operator"
)

func main() {
	// single-line comment start with "//"
	// comments are just for documentation
	fmt.Println("hello world")
	
	fmt.Println(operator.Hello())
}
```