# ASP.NET-Core-Application-with-Azure-DevOps

Creating an ASP.NET Core web application with features like user authentication, database integration, and a simple page that displays a list of items. For this example, we'll use Entity Framework Core for database access and SQLite as the database provider. Please ensure that you are having the necessary NuGet packages installed for this project.

Project Overview:

Project Name: ASP.NET Core Application with Azure DevOps

Technology: ASP.NET Core (C#)

Source Code Repository: GitHub

Step 1: Create a GitHub Repository

-> Go to GitHub and log in or create a new account.

-> Click on the "+" sign in the top-right corner and select "New repository."

-> Provide a repository name (e.g., SampleWebApp) and a brief description.

-> Choose public or private based on your preference.

->Select "Initialize this repository with a README."

-> Click "Create repository."

-> Create the source code uploaded above.

Remember to apply migrations and update the database before running the application. In the Package Manager Console, run the following commands:

"Add-Migration InitialCreate"

"Update-Database"

Now, when you run the application and navigate to the "/Item" route, you will see the list of items and a form to add new items. The items will be saved in the SQLite database.

Step 2: Set Up Azure DevOps Project

-> Go to Azure DevOps (https://dev.azure.com/) and log in or create a new account.

-> Click "Create project."

-> Provide a project name (e.g., ASP.NET Core Application with Azure DevOps) and choose a visibility option.

-> Click "Create" to create the project.

Step 3: Connect GitHub Repository to Azure DevOps Project

-> In your Azure DevOps project, go to "Project Settings" (bottom-left corner) and select "Service connections."

-> Click "New service connection" and choose "GitHub."

-> Follow the prompts to authorize Azure DevOps to access your GitHub account.

-> Select the GitHub repository you created earlier (e.g., SampleWebApp).

-> Click "Save."

Step 4: Create an Azure DevOps Pipeline

-> In your Azure DevOps project, go to "Pipelines" and click "New pipeline."

-> Choose the location of your source code (GitHub).

-> Select the repository (e.g., ASP.NET Core Application with Azure DevOps).

-> Azure DevOps will analyze your repository and suggest a pipeline template. Choose "ASP.NET Core" if available, or select "Starter pipeline" for a basic template.

-> Review the YAML file, make any necessary adjustments, and click "Save and run" to run the pipeline.

# After setting up the project, whenever you push changes to the GitHub repository, Azure DevOps will automatically trigger the pipeline and build, test, and deploy your ASP.NET Core web application.
