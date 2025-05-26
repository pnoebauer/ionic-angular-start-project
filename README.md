# Project Setup

This project uses [Ionic](https://ionicframework.com/) with [Angular](https://angular.io/).

## Setup Steps

1. **Install Ionic CLI**  
    Install the Ionic command-line interface globally:
    ```bash
    npm install -g @ionic/cli
    ```

2. **Create a New Project**  
    Start a new Ionic Angular project:
    ```bash
    ionic start
    ```
    - Choose a project name.
    - Select `Angular` as the framework.
    - Pick a starter template (e.g., `blank`).

    This generates a new folder with all required files and dependencies.

3. **Navigate to the Project**  
    Change into your project directory:
    ```bash
    cd your-project-name
    ```
    Replace `your-project-name` with your chosen name.

4. **Run the App**  
    There are two main ways to serve the app locally:

    - **Using Ionic CLI:**  
      ```bash
      ionic serve
      ```
      This command starts a local development server (default: [http://localhost:8100](http://localhost:8100)), enables live reload, and provides additional features such as port forwarding, host configuration, and Hot Module Replacement (HMR).  
      Under the hood, `ionic serve` runs:
      ```
      ng run app:serve --host=localhost --port=8100
      ```
      and adds Ionic-specific tooling and integrations.

    - **Using Angular CLI:**  
      You can also use the standard Angular CLI command:
      ```bash
      npm run start
      ```
      or directly:
      ```bash
      ng serve
      ```
      This serves the app using Angular's development server, but without the Ionic-specific enhancements (like port forwarding, custom host/port, and HMR configuration) provided by `ionic serve`.

## What Happens During Setup

- The Ionic CLI scaffolds the project structure and installs dependencies.
- The `ionic serve` command compiles the app, starts a local server with live reload, and adds features like port forwarding, custom host/port, and HMR.
- The Angular CLI (`ng serve` or `npm run start`) serves the app with standard Angular development tooling.
- All configuration files and scripts are set up for Angular development with Ionic components.
