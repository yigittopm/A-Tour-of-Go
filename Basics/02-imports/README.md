# İçe Aktarma

Bu kod, içe aktarmaları parantez içine alınmış, `faktörlere ayrılmış` bir içe aktarma ifadesinde gruplandırır.

Ayrıca, aşağıdakiler gibi birden çok içe aktarma ifadesi de yazabilirsiniz:

```go
import "fmt"
import "math"
```

Ancak faktörlü import ifadesini kullanmak iyi bir stildir.

```go
package main

import (
	"fmt"
	"math"
)

func main() {
	fmt.Printf("Şimdi %g probleminiz var.", math.Sqrt(7))
}

```

