[form authentication with remember me strategy on scalatra]: http://www.jaredarmstrong.name/2011/08/scalatra-form-authentication-with-remember-me/
[Jared Armstrong]: http://www.jaredarmstrong.name/
[localhost:8080]: http://localhost:8080
[mongodb]: http://www.mongodb.org/

# Scalatra Form authentication with Remember me

[Jared Armstrong] wrote a nice blog entry about [form authentication with remember me strategy on scalatra].

The original source code has been forked to modify dependencies and setup the environment to work with scala 2.9.1 and sbt 0.11.0

# Usage

Run the following commands and navigate to [localhost:8080]

  $ sbt
  
  $ container:start

# MongoDB

A [mongodb] local instance is supposed to be running, populate with some data

  $ mongodb

  > use scalatra-auth

  > u = {username: "test@test.com", password: "", rememberMe: "true"};

  > db.users.save(u)
