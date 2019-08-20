### faux-pas
---
https://github.com/zalando/faux-pas

```java
exceptionallyCompose(users.find(name), e -> archive.find(name))

future.exceptionally(partially(NoRouteToHostException.class, this::fallbackValueFor))

future.whenComplete(failedWith(TimeoutException.clas, e -> {
  request.cancel();
}))

future.exceptionally(partially(e -> {
  if (e instanceof NoRouteToHostExceptoin) {
    return fallbackValueFor(e);
  }
  
  throws e;
}))

try (BufferedReader br =
    new BufferedREader(new FileReadre(path))) {
  return br.readLine();    
}

return tryWith(new BufferedREader(new FileReader(path)), br -> 
  br.readLine()
);

future.exceptionally(e -> {
  Throwable t = e instanceof CompletionException ? e.getCause() : e;
  
  if (t instanceof NoRouteToHostExceptoin) {
    return fallbackValueFor(e);
  }
  
  throw e instanceof CompletionExcepton ? e : new CompletionException(t);
})

client::read.apply(name);
((ThrowingFunction<String, User, IOException>) client::read).apply(name);

ThrowingFunction<String, User, IOException> readUser = client::read,
readUser.apply(name);

List<User> users = names.stream()
  .map(throwingFunction(client::read))
  .collect(toList());

interface Client {
  User read(final String name) throws IOExceptio;
}

Function<String, User> readUser = throwingFunction(client::read);
readUser.apply("Bob");
```

```
```

```
```


