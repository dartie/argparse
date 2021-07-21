---
name: Bug
about: Create a report to help us improve
title: ''
---

**Describe the bug**
A clear and concise description of what the bug is.

**To Reproduce**
Fully functional code or test case to reproduce the behavior

You can use the code as a template

```go
package main

import (
    "fmt"
    "github.com/dartie/argparse"
)

func main() {
    parser := argparse.NewParser("basic", "this is a basic program", nil)
    name := parser.String("n", "name", nil)
    if e := parser.Parse(nil); e != nil {
        fmt.Println(e.Error())
        return
    }
    fmt.Printf("hello %s\n", *name)
}
```

**Expected behavior**
A clear and concise description of what you expected to happen.

**Terminal Output**
If executable, add terminal output to help explain your problem.

**Environment:**

 - OS: [e.g. MacOS 10.15]
 - Go Version: [e.g. 1.13]
 - Package Version: [e.g. v0.1.0]

**Additional context**
Add any other context about the problem here.

