## Two Sum in Go 
### A simple Go implementation of the Two Sum problem .

#### Clone the repository
```bash
git clone https://github.com/Ho3einTahan/2sum-array
cd 2sum-array
```

#### Run the program
```bash
go run main.go
```

#### Time Complexity
- Time: O(n²)
- Space: O(1)

#### Simple Code :
```go
package main

import "fmt"

func main() {

	var numbers []int = []int{2, 5, 7, 12, 2, 4, 5, 3, 6, 9, 1}
	var sum int = 10

	for i, number := range numbers {

		target := sum - number

		for j := i + 1; j < len(numbers); j++ {

			if target == numbers[j] {
				fmt.Printf("Target : %d + %d \n", number, numbers[j])
				break
			}

		}

	}

}
```

### Author
#### Developed by Ho3ein Tahan