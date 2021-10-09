# Instagram-API-clone_Appointy_Task
## Appointy task | Instagram Backend API
 
## Sagnik Chatterjee
## 19BAI1153


#### Golang + Instagram Private API
<p align="center"><img width=100% src="https://raw.githubusercontent.com/ahmdrz/goinsta/v1/resources/goinsta-image.png"></p>

> Unofficial Instagram API for Golang

[![Build Status](https://travis-ci.org/ahmdrz/goinsta.svg?branch=master)](https://travis-ci.org/ahmdrz/goinsta) [![GoDoc](https://godoc.org/github.com/ahmdrz/goinsta?status.svg)](https://godoc.org/github.com/ahmdrz/goinsta) [![Go Report Card](https://goreportcard.com/badge/github.com/ahmdrz/goinsta)](https://goreportcard.com/report/github.com/ahmdrz/goinsta) [![Gitter chat](https://badges.gitter.im/goinsta/community.png)](https://gitter.im/goinsta/community)

# instagram-rest-api

REST API with all basic features real Instagram has.


## Features:

-   registering and logging to user account
-   posting photos
-   commenting and liking photos
-   following system
-   all CRUD operations on posts, comments, follows and likes with relevant permissions


### Features

* **HTTP2 by default. Goinsta uses HTTP2 client enhancing performance.**
* **Object independency. Can handle multiple instagram accounts.**
* **Like Instagram mobile application**. Goinsta is very similar to Instagram official application.
* **Simple**. Goinsta is made by lazy programmers!
* **Backup methods**. You can use `Export` and `Import` functions.
* **Security**. Your password is only required to login. After login your password is deleted.
* **No External Dependencies**. GoInsta will not use any Go packages outside of the standard library.

### Package installation 

`go get -u -v gopkg.in/ahmdrz/goinsta.v2`

### Example

```go
package main

import (
	"fmt"

	"gopkg.in/ahmdrz/goinsta.v2"
)

func main() {  
  insta := goinsta.New("USERNAME", "PASSWORD")

  // Export your configuration
  // after exporting you can use Import function instead of New function.
  // insta, err := goinsta.Import("~/.goinsta")
  // it's useful when you want use goinsta repeatedly.
  insta.Export("~/.goinsta")

  ...
}
```



