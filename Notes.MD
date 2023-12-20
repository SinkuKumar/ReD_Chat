# [Full Stack Project | React and DRF | djChat](https://www.youtube.com/playlist?list=PLOLrQ9Pn6cawHF2lVl9goEm9Ta3rlutPD)
[Very Academy](https://www.youtube.com/@veryacademy)

## 1. Course Introduction and Technical Preview

* React Frontend
* Django DRF Backend
* Using WebSockets for Real-Time Communication
* Use JWT for Authentication
* HTTP Cookies for Authentication
* WebSocket Authentication
* Refresh access tokens
* Handling form validations
* Extend your app
* Walkthrough of app
* React FrontEnd Material UI
* Responsive Design
* Django Administration
* Document Endpoint API using Swagger UI
* Filters and Validating Images
* Reusable templates
* API Integration

1. **Course Overview and Accessibility**:
   - Focuses on building a full stack React-Django application with DRF (Django Rest Framework) and channels for WebSocket functionality.
   - Emphasizes accessibility; available on YouTube and Udemy for purchase.

2. **Course Structure**:
   - Spans approximately 28 hours, with potential additional hours due to ongoing improvements.
   - Covers both front-end (React) and back-end (Django) development, which contributes to the course's length.

3. **Content Highlights**:
   - Starts with building the chat server administration API in the backend, involving managing servers and categorization.
   - Emphasizes front-end templating using Material UI, focusing on responsive design and reusable components.
   - Progresses to API integration, connecting the React application to the Django backend, considering issues like CORS and Axios interceptors.
   - Implements WebSocket functionality using Django channels for real-time chat features.
   - Focuses on authentication, starting from JWT (Json Web Tokens) implementation and moving to HTTP-only cookies, with an emphasis on customizations and security aspects.
   - Concentrates on WebSocket authentication, refresh access tokens, and user authentication for both HTTP requests and WebSocket connections.

4. **Technical Preview**:
   - Provides a walkthrough of the developed project, showcasing the front-end React structure, its responsiveness, and component-based development.
   - Demonstrates the backend's Django administration interface, including the setup of servers, categories, and chat rooms (channels).
   - Illustrates how users navigate through servers, channels, and engage in chat functionalities within the application.

5. **Detailed Course Components**:
   - Backend development involves building APIs, filtering data, documenting using Swagger UI, managing database tables, and dealing with image uploads and associated signals.
   - Frontend covers template creation, React page structuring, integration with Material UI, API connections, error handling, JWT implementation, and more.
   - Discusses the complexities involved in setting up WebSocket functionality, authentication, security measures like HTTP-only cookies, token management, and CORS handling.

6. **Course Approach**:
   - Emphasizes not only following steps but understanding the processes, exploring customization, and adapting to individual project requirements.

The course aims to equip learners with comprehensive skills in building a real-time chat application, covering various aspects from backend development to frontend design and integration, with a focus on explaining concepts for a deeper understanding.


## 2. Initiating Project Source Control

* Source Control System
* Git
* GitHub
* Create Account
* Install Git
* GitHub Desktop
* Create a GitHub Repository
* Push to GitHub
* Conclusion

1. **Overview of Course Access**:
   - Part of a comprehensive React-Django project called DJ Chat, available on YouTube playlist or as a full course on Udemy.
   - GitHub link provided in the video description for the course.

2. **Introduction to Source Control**:
   - Highlights the importance of source control in software development for managing code changes over time.
   - Emphasizes the use of Git, a widely used source control system, and the GitHub platform for cloud-based code storage and collaboration.

3. **Setting Up Git and GitHub**:
   - Demonstrates the installation of Git from git-scm.com for Mac, Windows, or Linux systems.
   - Guides through verifying the successful installation of Git using terminal commands.
   - Recommends downloading GitHub Desktop, a graphical user interface for Git, for easier management of repositories.

4. **Creating a Repository**:
   - Guides through creating a new repository using GitHub Desktop by specifying the repository name, path, and initialization options.
   - Explains the initialization of a repository folder that Git will track for changes and introduces committing changes to Git.

5. **Publishing to GitHub**:
   - Guides through publishing the created repository to GitHub, linking the local repository to the GitHub platform for remote access and collaboration.
   - Demonstrates the process of pushing changes to GitHub, making the code base securely available online for tracking changes and collaboration.

6. **Benefits of GitHub**:
   - Highlights the convenience of storing repositories on GitHub, enabling deployment, managing projects, and facilitating collaboration with others.

7. **Conclusion**:
   - Emphasizes the readiness to start building the application now that the project repository is set up and securely saved on GitHub.

The tutorial aims to equip users with the fundamental knowledge and setup required to manage code changes, collaborate, and deploy a full stack React-Django project using Git and GitHub.


## 3. Create a New Django DRF Project

* VSCode
* Virtual Environment
* Create a new venv
* Activate venv
* PyPI
* `cmd+k` on mac or `cls` windows to clear terminal
* Create django project
* Install Django REST Framework (DRF)
* Run server

1. **Virtual Environment Setup**:
   - Guides users to activate a virtual environment (venv) within the project folder to contain project-specific dependencies.

2. **Activation on Different Platforms**:
   - Provides instructions for activating venv on both Mac and Windows systems through terminal commands (`source` and `venv`).
   - `python3 -m venv venv`
   - `source venv/bin/activate`

3. **Installing Django**:
   - Demonstrates the use of the Python package manager `pip` to install Django within the activated virtual environment. 
   - `pip install django`
   - Highlights that the downloads are sourced securely from the Python Package Index (PyPI).

4. **Source Control and Ignoring Files**:
   - Acknowledges that Git is tracking all changes, including the virtual environment files (venv), which aren't intended to be tracked.
   - Suggests that venv-related files should be excluded from version control, and this process will be explained shortly.

5. **Creating a Django Project**:
   - Uses the `django-admin` command to initiate a new Django project called "D_Chat." 
   - `django-admin startproject D_Chat`
   - Discusses different approaches to structuring Django projects and chooses to create a main project folder within the root directory.

6. **Navigating the Project Structure**:
   - Demonstrates how the terminal is positioned within the project folder, allowing easy navigation and manipulation of project files.
   - Clarifies how the `manage.py` file serves as the entry point for Django commands and interactions.

7. **Installing Django Rest Framework (DRF)**:
   - Highlights the need to install Django Rest Framework (DRF) using `pip install djangorestframework` within the activated virtual environment.

8. **Running the Django Server**:
   - Guides users to activate the Django server using the `python manage.py runserver` command.
   - Demonstrates how the server starts and provides the URL to access the Django application in the browser.
   - Emphasizes using `Ctrl + C` to quit the server and regain control of the terminal for further commands.

This segment of the tutorial focuses on setting up the development environment by creating a virtual environment, installing Django and DRF, configuring the project structure, and running the Django server within the created Git repository folder.


## 4. Configuring Environment Variables for your Project

* Secret and sensitive information
* dotenv in python
* Install dotenv
* Create `.env` file

1. **Purpose of Environment Variables**:
   - Explains the importance of managing sensitive information in the project, utilizing environment variables to separate sensitive data from the codebase.
   - Emphasizes the significance of security considerations, especially regarding sensitive information like database credentials and secret keys.

2. **Identifying Sensitive Data**:
   - Discusses identifying values (e.g., database credentials, secret keys) that need to be stored as environment variables instead of being exposed in the codebase.

3. **Setting Up Environment Variables**:
   - Focuses on the use of the `python-dotenv` package.
   - Instructs users to install `python-dotenv` using `pip install python-dotenv`.
   - Creates a `.env` file within the project folder to store sensitive information as key-value pairs.

4. **Moving Sensitive Information to Environment Variables**:
   - Demonstrates moving sensitive data, such as the `SECRET_KEY` and `DEBUG` settings, from the Django project's settings file to the `.env` file.
   - Explains the rationale behind securing the `SECRET_KEY` and managing the `DEBUG` setting through environment variables.

5. **Accessing Environment Variables**:
   - Utilizes Python's `os` module and the `python-dotenv` library to access environment variables within the Django project.
   - Provides code examples showing how to access environment variables like `SECRET_KEY` and `DEBUG` in the Django settings file.

6. **Testing Environment Variables**:
   - Conducts a test to ensure that the Django application can access and apply the values stored in the `.env` file as environment variables.
   - Demonstrates a test by intentionally removing the `SECRET_KEY` from the settings file and verifying that Django throws an error when trying to access the missing key.

7. **Summary and Considerations**:
   - Summarizes the significance of configuring environment variables for enhanced security and manageability in software development.
   - Highlights the importance of configuring environment variables for different deployment environments and suggests seeking deployment-specific approaches for setting environment variables.

This tutorial provides a comprehensive guide to leveraging environment variables in Django projects to enhance security, manage sensitive information, and ensure smoother application deployment across various environments.


## 5. Configuring Visual Studio Code for Black Formatting

* Linting and Formatting
* Readability, Maintainability and Correctness
* Black - Python code formatter adhere to PEP8 guide
* Install Black
* Configure Black
* Install isort

1. **Purpose of Linting and Formatting**:
   - Explains the importance of linting and formatting in software development for readability, maintainability, and code correctness.

2. **Introduction to Black**:
   - Introduces Black as a Python code formatter that automatically formats code to comply with the PEP 8 style guide.
   - Recommends Black for maintaining consistency and readability across Python projects.

3. **Installation of Black**:
   - Guides users to install Black using the Python package index (`pip install black`) within the project environment.

4. **Integration with Visual Studio Code**:
   - Demonstrates setting up Black in Visual Studio Code for a more customized configuration.
   - Advises creating a `.vscode` folder and a `settings.json` file within the project for specific settings.

5. **Configuring VS Code Settings**:
   - Configures the `settings.json` file to include settings for formatting on save and utilizing Black as the default Python formatter.
   - Explains the significance of specifying settings for different programming languages within VS Code.

6. **Testing the Setup**:
   - Conducts a test by intentionally modifying code in a Python file and saving it to observe Black automatically formatting the code according to the PEP 8 style guide.
   - Identifies additional actions needed to organize imports and guides users to install the `isort` extension in VS Code.
   - Demonstrates how the installed `isort` extension enhances the import organization automatically upon saving the file.

7. **Summary of Benefits**:
   - Summarizes the advantages of consistent formatting throughout the project, ensuring that Python code adheres to coding standards.
   - Emphasizes the importance of utilizing tools like Black and VS Code extensions to maintain code consistency and readability.

This tutorial offers a detailed guide on setting up and integrating Black, along with VS Code configurations, to streamline code formatting and improve the overall quality of a Django project.


## 6. Configuring Visual Studio Code for Flake8 Linting

* Linting
* Flake8
* Install Flake8
* Configure Flake8

* Installation worked, but configuration don't using python packages. 
* Alternatively, installed `Black-Formatter` and `Flake8` extensions by Microsoft in VSCode, with slight different configuration, working well. 
* Checking settings.json for configuration.

1. **Introduction to Linting and Flake8**:
   - Explains the importance of linting in code development.
   - Introduces Flake8 as a Python linter that checks code for syntax errors, unused imports, and other issues, enforcing code standards and best practices.

2. **Installation of Flake8**:
   - Demonstrates the installation process of Flake8 using `pip install flake8` within the project's virtual environment.
   - Highlights the necessity of ensuring that the Visual Studio Code Python interpreter is set to the virtual environment to access installed dependencies.

3. **Configuration in VS Code**:
   - Guides users on configuring Flake8 within Visual Studio Code settings.
   - Enables Python linting and sets up Flake8 to run on save, ensuring continuous code checking during development.

4. **Customizing Flake8 Parameters**:
   - Provides an example of changing the maximum line length parameter in Flake8 settings to align with the formatting standards of Black.
   - Indicates that Flake8 offers various configuration options beyond what Black provides, encouraging users to explore further options.

5. **Testing Flake8 Integration**:
   - Demonstrates the practical implementation of Flake8 by intentionally introducing an error in the code and verifying Flake8's identification of the issue.
   - Emphasizes the utility of Flake8 in identifying and assisting in rectifying code errors throughout the development process.

The tutorial ensures that Flake8 is successfully integrated into the project's workflow within Visual Studio Code, offering a comprehensive understanding of its usage and configuration for effective code checking and maintaining coding standards.


## 7. Create your first commit in a Git repository

* Tracking changes
* .gitignore
* Multiple .gitignore
* requirements.txt
* Git CLI
* `git Commit`

1. **Introduction to Repository and Changes**:
   - Overview of the project DJ chat as part of a Full Stack React Django DRF project.
   - Emphasis on the need to save the project's current state to enable rolling back to a stable version in case of issues during development.

2. **Git Ignore Configuration**:
   - Explanation of the necessity to ignore certain files and folders (like the virtual environment, database files, sensitive environment variables) in version control using `.gitignore`.
   - Demonstration of creating a `.gitignore` file within the project folder to specify files/folders to exclude from tracking.

3. **Visual Studio Code Integration**:
   - Indication of how files specified in `.gitignore` are visually indicated in Visual Studio Code, making it clear that they are not being tracked.

4. **Moving `.gitignore` to Root Directory**:
   - Notice that placing `.gitignore` within a subdirectory does not prevent tracking of files within that subdirectory.
   - Demonstrates moving the `.gitignore` file to the root directory to ensure exclusion of the specified files/folders within the entire project.

5. **Versioning Dependencies**:
   - Usage of `pip freeze > requirements.txt` to generate a list of all installed packages and dependencies needed to run the project.
   - Addition of `requirements.txt` to the repository to help others replicate the project's environment.

6. **Committing Changes**:
   - Explanation of Git commits as snapshots of changes in files at a specific time.
   - Description of commit messages and their significance in summarizing the changes made.
   - Usage of GitHub Desktop to visualize the changes and commit the changes to the main branch.
   - Pushing the committed changes to the GitHub repository for cloud storage.

7. **Conclusion**:
   - Reiteration of the importance of frequent commits to track changes and collaborate effectively.
   - Promises additional techniques and information to enhance the development workflow throughout the project.

The tutorial offers a comprehensive understanding of version control using Git, `.gitignore` for excluding specific files, tracking dependencies, and utilizing GitHub Desktop for managing commits and pushing changes to a remote repository.


## 8. Initiate Chat Server Administration App

* Server and Channel Management System app
* Single view set, retrieving a list of server and associated channels based on query parameters
* Django promotes idea of breaking functionality into apps.
* Testing and documentation for code.

## Creating a Django Custom User Model (AbstractUser)

## Build Chat Server Administation Models

## Build Chat Server Configuring DRF-Spectacular & Swagger UI

## Configuring Default Authentication Classes in Django DRF

## Creating an API Endpoint for Filtering Servers by Category

## Creating an API Endpoint for Filtering Servers by Quantity

## Creating an API Endpoint for Filtering Servers by User

## Creating an API Endpoint for Filtering Servers by Server ID

## Server Associated Channels

## Filtering Servers and Returing Annotation

## Creating Code Comments with ChatGPT

## Creating DocStrings with ChatGPT

## Creating an API Endpoint Decorator for Detailing Endpoints

## Configuring Django to Handle Storing Images

## Model Refactor for Icon and Banners for server

## Django Model Validation Class for Image Field

## Commit and Merge

## Create a new React Project with Vite

## React Pages Directory and Home Component

## React Routing Introdution with React Router

## Install MUI and integrate it into the existing project

## Creating the Primary App Bar (Part-1) Framework

## Integrating Google Fonts into an existing React/MUI project

## MUI Repsponsive Fonts

## Creating the Primary App Bar (Part-2) Responsive

## MUI Primary Draw (Part-1) Framework

## MUI Primary Draw (Part-2) Framework

## MUI Secondary Draw (Part-1) Framework

## Creating the Main Component with Material UI

## Installing Axios Create First API request

## Configuring Cross-Origin Resource Sharing (CORS)

## Create a Global Configuring File

## Axios Interceptor

## React CRUD Hook

## Primary Drawer Component MUI5

## Secondary Draw Component - Explore Categories