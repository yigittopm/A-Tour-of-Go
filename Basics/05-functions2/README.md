# Fonksiyonlar Devam

İki veya daha fazla ardışık adlandırılmış işlev parametresi bir türü paylaştığında, türü sonuncusu hariç tümünden atabilirsiniz.

Bu örnekte, eski hali:
```go
x int, y int
```

bu da kısaltılmış hali:
```go
x, y int
```

*Example*
```go
package main

import "fmt"

func add(x, y int) int {
	return x + y;
}

func main() {
	fmt.Println(add(42,13))
}
```
