 #go/package #go/import #go/mainfunction 

```go cpp title:main.go 
package main

import "fmt"

func main() {
	// single-line comment start with "//"
	// comments are just for documentation
	fmt.Println("hello world")
}
```

1. 每個資料夾使用相同 package
2. func main () 作為 code 邏輯入口
3. 執行: go run main.go