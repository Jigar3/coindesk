# Coindesk

coindesk is a Go package to access Coindesk API

## Installations & Usage

### Installation

`go get github.com/gostudent/coindesk`

### Usage

```go
package main

import (
	"fmt"
	"github.com/gostudent/coindesk"
)

func main() {
	priceUsd := coindesk.GetPrice()
	fmt.Println(priceUsd)

	priceInr := coindesk.GetPrice("INR")
	fmt.Println(priceInr)

	USD, GBP, EUR := coindesk.CurrentPrice()
	fmt.Println(USD, GBP, EUR)
}
```