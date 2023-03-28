#### Go Concepts
- Syntax And Types
- Arrays And Iteration
- Slices
- Pointers
- Functions
- Interfaces
- Maps
- Modules And Packages
- Building And Compiling Go Applications
- Concurrency
- Concurrency With Channels
- Concurrency With The Sync Package
- Context
- Embedding And Composition
- Errors
- Generics
- Templates
- HTTP Client
- Table Driven Testing
- Testing Basics
- The Go Command
- Tooling
- Benchmarking / Performance Tuning

##### Learning
[Golang Advanced Tutorial](https://golangbyexample.com/golang-comprehensive-tutorial/)  
[IOTA in Go (Golang)](https://golangbyexample.com/iota-in-golang/)  
[gopherguides.com - Where and When to use Iota in Go](https://www.gopherguides.com/articles/how-to-use-iota-in-golang)  
[Go Basics](https://www.howtocode.io/posts/go-basics-1-installing-go-on-a-mac)  
[Practical Go Lessons by Maximilien Andile](https://www.practical-go-lessons.com/)  
[An Introduction to Programming in Go - © 2012 by Caleb Doxsey](https://www.golang-book.com/books/intro)  
[Free Code Camp - Learn Go Programming for Beginners](https://www.youtube.com/watch?v=YS4e4q9oBaU)  
[Go Programming Language - Tutorial](https://www.golangprograms.com/go-language.html)  
[Go e-Book Collections](https://edu.anarcho-copy.org/Programming%20Languages/Go/)  

#### Profiling
[Go: The Complete Guide to Profiling Your Code](https://hackernoon.com/go-the-complete-guide-to-profiling-your-code-h51r3waz)  
[Profiling in GoLang - golangdocs.com](https://golangdocs.com/profiling-in-golang)  
[Benchmarking in Golang: Improving function performance](https://blog.logrocket.com/benchmarking-golang-improve-function-performance/)  
[Benchmarking Results in Go](https://www.mikenewswanger.com/posts/2018/benchmarking-in-go/)  

#### Testing
[A Deep Dive into Table-Driven Testing in Golang - engineering.mercari.com](https://engineering.mercari.com/en/blog/entry/20211221-a-deep-dive-into-table-driven-testing-in-golang/)  

#### Go Frameworks
[Gin Framework](https://github.com/gin-gonic/gin)  
[ent - An entity framework for Go](https://entgo.io/)  
[HUGO - A Fast and Flexible Static Site Generator](https://github.com/gohugoio/hugo)  
[FastHTTP - Web Framework - 16K Stars](https://github.com/valyala/fasthttp)  
[Echo - High performance, minimalist Go web framework - 21K Stars](https://echo.labstack.com/)  
[Go-Chi - A lightweight, idiomatic and composable router for building Go HTTP services - 10.5K Stars](https://github.com/go-chi/chi)  

#### Boilerplates
[Gin + PostgreSQL DB + Redis + CRUD API + JWT + Postman API Collections](https://github.com/Massad/gin-boilerplate)  
[Gin + DynamoDB + Docker](https://github.com/vsouza/go-gin-boilerplate)  
[Gin + PostgreSQL + GORM + REST + MVC + DTO + Docker](https://github.com/daystram/go-gin-gorm-boilerplate)  
[Gin + PostgreSQL + GORM + REST + MVC + Viper + Env + Logger + Middlewares + Live Reload + Docker](https://github.com/akmamun/gin-boilerplate-examples)  

#### Gin Framework

**The key features of Gin are:**

- Light weight & performant
- Zero allocation router
- Fast
- Middleware support (for CORS, timeout, caching, authentication, and session management)
- Crash-free
- JSON validation
- Routes grouping
- Error management
- Rendering built-in (XML/JSON/YAML/ProtoBuf)
- Extendable
- Serve Static files

#### Best Practices
- Create one source file for each entity controller and implement separate handler functions for each CRUD operation
- Use status codes from the `net/http` package instead of hardcoded integer status codes, Eg: use `http.StatusOK` instead of `200`
- It’s always good to implement custom middleware if you feel that you’re writing repetitive code inside endpoint handlers
- Direct JSON manipulation with the gin.H shortcut can generate repetitive code — try to use structs if possible. For example, `gin.H` is just a short type definition for `map[string]interface{}`
- Make sure to handle errors properly during inter-service communication; otherwise, you will not be able to trace connectivity issues easily
- Write critical situations in a log file

#### Go App Development
[Using Elasticsearch, Logstash, and Kibana with Go applications - LogRocket](https://blog.logrocket.com/using-elasticsearch-logstash-and-kibana-with-go-applications/) 

#### Package Management
[Package Management with Go Modules - blogs.halodoc.io](https://blogs.halodoc.io/go-modules-implementation/)  
[Go Modules - Introduction](https://golang.org/ref/mod#introduction)  
[Evaluating Go's Package Management and Module Systems by @ayisaiah - honeybadger.io (G)](https://www.honeybadger.io/blog/golang-go-package-management/)  


[High Performance Messaging with NATS](https://medium.com/@syedrizwan161/high-performance-messaging-with-nats-1c261fae3778)  
