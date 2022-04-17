# Fonksiyonlar

Bir fonksiyon sıfır veya daha fazla argüman alabilir.

Bu örnekte `add`, `int` türünde iki parametre alır.

Türün değişken adından *sonra* geldiğine dikkat edin.


```go
package main

import "fmt"

func add(a int, y int) int {
	return a + y;
}

func main() {
	fmt.Println(add(44,23));
}
```

(Türlerin neden böyle göründükleri hakkında daha fazla bilgi için [Go'nun bildirim sözdizimi](https://go.dev/blog/declaration-syntax) hakkındaki makaleye bakın.)