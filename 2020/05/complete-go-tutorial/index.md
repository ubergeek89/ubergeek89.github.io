# Complete Go Tutorial


This is going to be the first long form post on this blog. We will review the Go language. I will try to introduce the reader to the fundamental concepts and spend more time trying to see what makes Go so special.

First things first, if you are coming from the world of Python, Javascript or PHP - Go is a compiled and a statically typed language. It is much closer to C in that respect. Your code is compiled to raw binary which is then executed directly by the targeted CPU. Go was developed at Google and was intended to replace many shortcomings of C++ (which is by no means a bad language). We can go into great details about the debate between various programming languages. But this post is not intended to be the place for that kind of discussion. So let us jump right onto Go.

## 1. Hello World

We will follow the old tradition of introducing new languages with a hello world. Here is a program that prints "Hello World" on the screen - 

```go
package main

import "fmt"

func main(){
	fmt.Println("Hello World")
}
```

You can save it to a text file hello.go. Navigate to the directory at the command line and run it by typing -

```bash
> go run hello.go
Hello World
```

You should see "Hello World" printed on the screen.

{{< admonition type=tip title="This is a tip" open=true >}}
Small tip
{{< /admonition >}}
