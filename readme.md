# Simple GraphQL with Laravel 5.6.23
### Installation

Open your favorite Terminal and run these commands.

First Tab:
```sh
$ git clone git@github.com:Rishats/laravel-graphql.git laravel-graphql.test
```

Second Tab:
```sh
$ cd laravel-graphql.test
```

Third Tab:
```sh
$ composer install
```

Fourth Tab:
```sh
$ php artisan migrate
```

# How to start it?
Just run Laravel server.
```sh
$ php artisan serve
```
# How to use it?
Try GraphQL
Go to http://127.0.0.1:8000/graphiql

To create a user:
```sh
mutation {
  createUser(
    name: "John Doe",
    email:"john@doe.com",
    password:"qwerty"
  ) {
    id,
    email
  }
}

```

To read a user:
```sh
query {
  user(id: 1){
    name,
    email
  }
}
```


# Helpful Article
> You can see more information about how you can create example project like this with your own Laravel version.
> https://medium.com/@albertcito/basic-example-graphql-with-laravel-225ab8d57981
