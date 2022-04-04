# Paketler

Her Go programı paketlerden oluşur.

Programlar main paketinde çalışmaya başlar.

Bu program, `fmt` ve `math/rand` içe aktarma yollarına sahip paketleri kullanıyor.

Kural olarak, paket adı içe aktarma yolunun son öğesiyle aynıdır.Örneğin, `math/rand` paketi, __rand__ ifade paketiyle başlayan dosyalardan oluşur.

```go
package main

import (
	"fmt"
	"math/rand"
)

func main() {
	fmt.Println("Benim favori numaram budur: ", rand.Intn(100))
}

```

**Not:** Bu programların yürütüldüğü ortam deterministiktir, bu nedenle örnek programı her çalıştırdığınızda `rand.Intn` aynı sayıyı döndürür.

(Farklı bir sayı görmek için sayı üretecini tohumlayın; örn. `rand.Seed`. Oyun alanında zaman sabittir, bu yüzden tohum olarak başka bir şey kullanmanız gerekecek.)
