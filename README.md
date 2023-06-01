## What Is This?

This is a C# project I completed while attending Epicoodus. It's an ASP.NET Core MVC web application that keeps track of a Hair Salon's Stylists and Clients.

## Application Instructions

To run this application, you will need to ensure the following software packages are installed locally:
• .NET6
• MySQL and MySQL workbench

## Initial Setup

1. Clone this repository 
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
## Importing the Database

1. Open MySQL Workbench and locate the Navigator pane.
2. Select "Data Import/Restore", which will open the Data Import page.
3. Select the option labeled "Import from Self Contained File". Navigate to the top directory of the files you downloaded from this repository ("HairSalon").
4. Within "HairSalon", select the file named tyler_adams.sql.
5. Under "Default Schema to be Imported To", click the "New..." button, enter the name of the database (tyler_adams.sql), and click "OK".
6. Navigate to the "Start Import" button located in the lower right corner of the Data Import Pane.
7. On the Navigator panel, select the "Schemas" tab. Click the "refresh" icon and the database should appear.

## Running the Program

1. Open a terminal and navigate to this project's production directory ("HairSalon")
2. Type dotnet watch run in the command line to start the project in development mode with a watcher.
 • If the build fails, revisit steps 1 - 3 above to ensure that .NET6 has been properly installed.
3. Open the browser to https:localhost:5001.
 • If you cannot access localhost:5001, it is likely because you have not configured a .NET developer security certificate for HTTPS.


## Below is a representation of the one-to-many relationship between the stylist and client tables:

![hair-salon-tables](https://github.com/skipmarcel/HairSalon.Solution/assets/121919165/be906981-cfc2-4286-86bb-b56e64840eb8)

