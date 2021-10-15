# Factory

#### _By Nathan Fletcher


## Technologies Used

* C#
* Object Oriented Programming
* ASP.NET Core MVC Framework
* Restful Routing Conventions

## Setup

<details>
<summary>Setup & Installation Instructions</summary>

#### Installations (if necessary)
* Install C# and .NET using the [.NET 5 SDK](https://dotnet.microsoft.com/download/dotnet-core/thank-you/sdk-5.0.100-macos-x64-installer)
* Install [MySql Community Server](https://dev.mysql.com/downloads/file/?id=484914)
* Install [MySql Workbench](https://dev.mysql.com/downloads/file/?id=484391)

#### Setup
* Clone this repository to your local machine
* Navigate to the Factory.Solution and create a file named "appsettings.json" 
* Add the following code to the file:
  ```
  {
    "ConnectionStrings": {
        "DefaultConnection": "Server=localhost;Port=3306;database=nathan_fletcher;uid=root;pwd=[YOUR-PASSWORD-HERE];"
    }
  }
  ```
* Navigate to the Factory folder and run the following commands:
* `dotnet add package Microsoft.EntityFrameworkCore -v 5.0.0`
* `dotnet add package Pomelo.EntityFrameworkCore.MySql -v 5.0.0-alpha.2`
* `dotnet add package Microsoft.EntityFrameworkCore.Proxies -v 5.0.0`
* `dotnet add package Microsoft.EntityFrameworkCore.Design -v 5.0.0`
* `dotnet tool install --global dotnet-ef`
* `dotnet ef migrations add Initial`
* `dotnet ef database update`

#### Start
* From the terminal in the Factory folder, run the following commands:
* `dotnet restore`
* `dotnet build` to compile the project.
* `dotnet run` to start the server.
* Enter localhost:5000 in your browser to start using the app. 
</details>


## Known Issues
* There are no known issues at this time.
* Please contact me if you find any bugs or have suggestions. 

## Future Plans
* Add more styling
* Add a table of incidents
* Add another class such as manufacturers and another many-to-many relationship such as manufacturer-issued certifications

## License

_[MIT](https://opensource.org/licenses/MIT)_  

Copyright (c) 2021 Nathan Fletcher

