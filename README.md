### Hi there 👋

```go
package main

import "fmt"

type Pentest struct {
	Name        string
	Role        string
	Location    string
	Major       string
	Certificates []string
	WorkingOn   []string
	CoffeeCup   bool
}

func (p *Pentest) Refill() {
	if !p.CoffeeCup {
		p.CoffeeCup = true
		fmt.Println("☕ Coffee refilled. Time to break things (ethically)!")
	} else {
		fmt.Println("☕ Fully caffeinated and ready to go!")
	}
}

func main() {
	me := Pentest{
		Name:        "DoobTheGoober",
		Role:        "Student",
		Location:    "U.S",
		Major:       "Computer Science",
		Certificates: []string{"Security+", "Pentest+", "NVAP"},
		WorkingOn:   []string{"Radio Hacking", "Web Application Security", "Automation"},
	}

	me.Refill()
}
```
