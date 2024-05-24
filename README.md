Waqq.ly Web Application

FEATURES
User Registration: Allows dog owners to register their dogs and dog walkers to register themselves.
Serverless Backend: Utilizes Azure Functions for scalable and efficient request handling.
NoSQL Database: Stores data in Cosmos DB for flexibility and scalability.
Responsive Design: Ensures the web application is accessible on various devices.
Continuous Integration and Deployment: Managed via GitHub Actions for seamless updates and deployment.

ARCHITECTURE
The application is structured as follows:
- Front-End: HTML and CSS for the user interface.
- Backend: Azure Functions handling API requests.
- Database: Cosmos DB for storing dog and walker information.
- CI/CD: GitHub Actions for automated build and deployment processes.

INSTALLATION AND DEPLOYMENT STEP 1 - 8

PREREQUISITES:
- Node.js and npm installed
- Python and pip installed
- Azure CLI installed 
- Git installed
- Azure account
- GitHub account

STEPS 1: CLONE THE REPOSITORY
- Clone the repository: git clone https://github.com/lordrelv/waqqlyWebApp.git
- cd waqqlyWebApp

STEP 2: INSTALL DEPENDENCIES
- cd src
- npm install

STEP 3: SETUP PYTHON VIRTUAL ENVIRONMENT
- cd api
- python -m venv .venv
- .venv\Scripts\activite

STEP 4: CONFIGURE AZURE FUNCTIONS
Ensure your 'local.settings.json' file is configured with your Azure Cosmos DB connection details.

DEPLOY YOUR APPLICATION
STEP 5: INITIALISE A GIT REPOSITORY
- git init
- git add .
- git commit -m "Initial commit"

CREATE A REMOTE REPOSITORY ON GITHUB
STEP 6: PUSH YOUR LOCAL REPOSITORY TO GITHUB
- git remote add origin https://github.com/yourusername/your-repo-name.git
- git branch -M main
- git push -u origin main

SEP 7: CREATE AN AZURE STATIC WEB APP
- Go to the Azure Portal.
- Search for "Static Web Apps" and click "Create".
- Fill in the required details:
- Subscription: Select your Azure subscription.
- Resource Group: Create a new resource group or use an existing one.
- Name: Enter a name for your Static Web App.
- Region: Choose a region close to you or your users.
- Hosting Plan: Choose "Free".
- Source: Select "GitHub".
- Organisation: Select your GitHub account.
- Repository: Select your repository.
- Branch: Select the branch you want to deploy from (usually main or master).
- Build Presets: Select "Custom".
- App location: Enter src.
- API location: Enter api.
- Output location: Enter src (or the folder where your built files will be located).
- Review and create
- create

PUSH CHANGES TO TRIGGER DEPLOYMENT
STEP 8: COMMIT AND PUSH CHANGES TO YOUR REPOSITORY TO TRIGGER THE DEPLOYMENT
- git add .
- git commit -m "Deploy application"
- git push origin main

CODE OF CONDUCT
Please adhere to the Code of Conduct when contributing.
