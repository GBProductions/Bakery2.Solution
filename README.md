# _Pierre's Sweet and Savory Treats_

 * _A program to allow Pierre's Sweet and Savory Treats to keep track of Treats and Flavors._
 * _Date Created: June 19th 2021_

#### By _**Garrett Brown**_

## Description
_A program that allows Pierre's Sweet and Savory Treats to keep track of various Treats and Flavors. Users can create Treats, Flavors, and associated details. Users can also keep track of which Flavors are assigned to which Treats, and vice versa. Users can also edit or delete details for Treats, or Flavors._

### User Stories

<details>
    <summary>Expand</summary>

#### User Stories
* The application should have user authentication. A user should be able to log in and log out. Only logged in users should have create, update and delete functionality. All users should be able to have read functionality.

* There should be a many-to-many relationship between Treats and Flavors. A treat can have many flavors (such as sweet, savory, spicy, or creamy) and a flavor can have many treats. For instance, the "sweet" flavor could include chocolate croissants, cheesecake, and so on.

* A user should be able to navigate to a splash page that lists all treats and flavors. Users should be able to click on an individual treat or flavor to see all the treats/flavors that belong to it.

</details>

## Setup/Installation Requirements
Table of Contents
* Required Programs
* Installation of Program
* Recreate Database
* Startup

<details>
    <summary>Expand for Instructions</summary>

### Required Programs
1. An internet browser.
2. Visual Code Studio (or another code editor).
3. .NET
4. MySQL
5. MySQLWorkbench


### Installation of Program
* _Open the terminal on your local machine and navigate to "Desktop."_
* _Clone "Factory.Solution"" with the following git command `git clone https://github.com/GBProductions/Bakery2.Solution`
* _Navigate to the top level of the repository with the command `cd Bakery2.Solution`_
* _Navigate into "Bakery" with git command `cd Bakery2`_


### Recreate Database

#### Instructions: `appsettings.json` Creation

1. Create a file in the root directory called `appsettings.json`. 
2. Add `appsettings.json` to `.gitignore`.
3. Insert the following code into `appsettings.json`:
    
``` 
{
    "ConnectionStrings": {
        "DefaultConnection": "Server=localhost;Port=3306;database=YOUR-DATABASE;uid=root;pwd=YOUR-PASSWORD;"
    }
}
```

4. Replace `YOUR-PASSWORD` with password you selected when installing MySQLWorkbench.
5. Replace `YOUR-DATABASE` with the name of your database.
6. In the root directory, run `dotnet ef databse update` 
7. In the root directory, run `dotnet ef databse restore`

This will recreate the database on your computer, using MySQLWorkbench. You can proceed to Startup.



### Startup
* Navigate to root directory in project.
* Restore project with git command `dotnet restore`
* Build project with git command `dotnet build`
* To run program, run git command `dotnet run`
* In browser, navigate to http://localhost:5000 

</details>

## Known Bugs

_There are currently no known bugs._

## Support and contact details

_For assistance, please contact Garrett Brown <garrettpaulbrown@gmail.com>_

## Technologies Used

* _Github, VS Code_
* _Bootstrap, MarkDown_
* _Entity Framework_
* _C#_
* _Authentication and Authorization_
* _.NET Core 5.0.1_
* _ASP.NET Core MVC_
* _ASP.NET Core Razor Pages_
* _HTML, CSS_
* _MySQL_
* _MySQLWorkbench_


### License

*Available under MIT Licensing*

Copyright (c) 2021 **_Garrett Brown_**

