# Setting up all tools for Cre-Dental Project as Developer

## ON Windows

This guide will walk you through the process of setting up a Django project in a virtual environment on a Windows system. Additionally, it will show you how to install Node.js, Angular, and run an Angular project alongside your Django application.

## Table of Contents

1. [Installing Up Django](#1-setting-up-django)
2. [Installing Node.js and Angular](#2-installing-nodejs-and-angular)
3. [Running Your Django Application](#3-running-your-django-application)
4. [Running Your Angular Application](#4-running-your-angular-application)
5. [Verification](#5-verification)

---

## 1. Setting Up Django

### Step 1: Install Python

If Python is not already installed on your system, you can download and install it from the official website: [Python Downloads](https://www.python.org/downloads/). Be sure to add Python to your system's PATH during installation.

### Step 2: Create a Virtual Environment

Open your command prompt and navigate to the directory where you want to create your Django project. Then, run the following commands to create and activate a virtual environment:

```shell
# Create a virtual environment named "myenv"
python -m venv backend

# Activate the virtual environment
backend\Scripts\activate
```

### Step 3: 
    Put folder backend called '' in backend environment

### Step 4: Install Django and Dependencies

With your virtual environment activated, install Django and any other project dependencies by running:

```shell
cd backend/name_folder_backend
pip install django
pip install -r req .txt
```

## 2. Installing Node.js and Angular

### Step 1: Install Node.js

Download and install Node.js from the official website: [Node.js Downloads](https://nodejs.org/en/download/). Choose the recommended version, which should be version 16 or later.

### Step 2: Install Angular CLI

Once Node.js is installed, open your command prompt and run the following command to install the Angular CLI globally:

```shell
npm install -g @angular/cli
```

## 3. Running Your Django Application

### Step 1: Navigate to Your Django Project

Open a command prompt and navigate to the root directory of your Django project.

### Step 2: Apply Migrations

If you have any database migrations, apply them with the following command:

```shell
python manage.py migrate
```

### Step 3: Start the Django Development Server

To run your Django application, execute the following command:

```shell
python manage.py runserver
```

Your Django development server should now be running at `http://localhost:8000/`.

## 4. Running Your Angular Application

### Step 1: Clone Your Angular Project

Navigate to the directory where you want to store your Angular project and run the following command to clone it from GitHub (replace `[repository_url]` with your actual GitHub repository URL):

```shell
git clone [repository_url]
```

### Step 2: Navigate to the Angular Project

Change your working directory to the cloned Angular project:

```shell
cd [angular_project_directory]
```

### Step 3: Install Node.js Dependencies

Install the project's Node.js dependencies using npm:

```shell
npm install
```

### Step 4: Start the Angular Development Server

To run your Angular application, execute the following command:

```shell
ng serve
```

Your Angular development server should now be running at `http://localhost:4200/`.

## 5. Verification

To verify that Python, Django, Node.js, and Angular have been successfully installed, you can check their versions using the following commands:

- Python: `python --version`
- Django: `python -m django --version`
- Node.js: `node -v`
- npm: `npm -v`

If all of these commands return their respective versions without errors, then your setup is complete and ready for development.

That's it! You've now successfully set up Django in a virtual environment on Windows, installed Node.js, Angular, and can run both your Django and Angular projects. Happy coding!
