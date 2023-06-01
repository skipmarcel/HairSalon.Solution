## What Is This?

This is a C# project I completed while attending Epicoodus. It's an ASP.NET Core MVC web application that keeps track of a Hair Salon's Stylists and Clients.

## How To Run This Project

1. Clone this repo.
2. Open the terminal and navigate to this project's production directory called "HairSalon".
3. Within the production directory "HairSalon", create a new file called `appsettings.json`.
4. Within `appsettings.json`, put in the following code, replacing the `uid` and `pwd` values with your own username and password for MySQL.

```json
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost;Port=3306;database=[YOUR_DATABASE_NAME];uid=[YOUR_USER_NAME];pwd=[YOUR_PASSWORD];"
  }
}
```

## Below is a representation of the one-to-many relationship between the stylist and client tables:

![hair-salon-tables](https://github.com/skipmarcel/HairSalon.Solution/assets/121919165/be906981-cfc2-4286-86bb-b56e64840eb8)

