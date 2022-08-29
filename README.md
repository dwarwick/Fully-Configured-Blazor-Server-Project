# ForumAppBlazorServer
### This is a Blazor Server project template with the following configuration: ###

* .Net 6
* Bootstrap 5.2
* DBContext configured
* Full Identity Scafolded and Configured
* Razor Pages and Routable Razor Components layout share the same layout file
* Bootstrap Navbar menu accross the top of  the template

### You will need to make the following changes ###
#### FetchData.razor ####
* Change @using ForumAppBlazorServer.Data to @using YourNamespace.Data

#### _Imports.razor (in the root of the project) ####
* Change @using ForumAppBlazorServer to @using YourNamespace
* Change @using ForumAppBlazorServer.Shared to @using YourNamespace.Shared

#### appsettings.json ####
* Update the database name from ForumDb in ConnectionStrings_DefaultConnection to your preferred database name, or enter your own connection string.


### Create the Database ###
After you make the above mentioned changes, compile the project and make sure you can browse the website. 
Assuming all is well, you will need to create the database before you can use it. 

Enter the following commands in the package manager console:  
*add-migration InitialMigration*  
*update-database*  

At this point, the database exists, along with all of the tables that are used for identity. Now you can run the website and register as a new user.
