#### Java Code Snippets

[Inject values into a Map from the properties file using the @Value annotation](https://stackoverflow.com/a/51997862/337011):

```java
@Value("#{${user}}")  
private Map<String, String> user;
```

Entry in application.properties must be:

```sh
user = { "name" : "John", "age" : "35", "place" : "California" }
```
