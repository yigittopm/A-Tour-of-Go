# Dışa Aktarılan Adlar

Go'da bir ad büyük harfle başlıyorsa dışa aktarılır. Örneğin *Pizza*, `math` paketinden dışa aktarılan *Pi* gibi dışa aktarılan bir addır.

*pizza* ve *pi* büyük harfle başlamaz, bu nedenle dışa aktarılmazlar.

Bir paketi içe aktarırken, yalnızca dışa aktarılan adlarına başvurabilirsiniz. `Dışa aktarılmamış` adlara paketin dışından erişilemez.

```go
package main

import (
	"fmt"
	"math"
)

func main() {
	fmt.Println(math.pi)
}
```

Kodu çalıştırın. Hata mesajına dikkat edin.

```diff
#example
-./prog.go:9:19: undefined: math.pi
```

Hatayı düzeltmek için *math.pi*'yi **math.Pi** olarak yeniden adlandırın ve yeniden deneyin.