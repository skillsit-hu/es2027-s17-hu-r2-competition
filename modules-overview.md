# Modules Overview

**EuroSkills Düsseldorm 2027 Hungarian National Competition, Web Technologies - Round 2**

Submitted by: [Skills IT](https://skillsit.hu)

You've been working as a **freelance web developer**, but now you're aiming to secure a developer position at a promising new startup in Hungary: **SkillShare Academy**. You have already **completed** the first round of the hiring process, and you have been selected from over 100 candidates for the second round, where only the **top six** candidates remain.

In this round, you have **two different tasks**. First, you will need to create a backend with multiple **REST API** endpoints. Then you will develop a frontend application that.

Descriptions of the three tasks:

- [Module A - Backend](module-a.md)
- [Module B - Frontend](module-b.md)

## Technical Environment

You can solve the tasks by developing them on your own machine.

### Gitea, git

For all three tasks, you can start with a selected template repo available on Gitea.

The available template repos:

- react
- react-ts
- vue
- vue-ts
- node
- node-ts
- laravel

The Gitea service is available at the following address:
[https://git.ssa.skillsit.hu](https://git.ssa.skillsit.hu)

To log in, you must use the username (cXX) and password (a 4-digit PIN code) you have been given.  
After logging in, create a new repo for the task.

- Give the name of the new repo using the following pattern: `module-Y`, where `Y` is the module's letter (eg. `module-a`, `module-b`). **Make sure you set the repo's name carefully because if you make a mistake, the automatic deployment will not work!**
- Under the template field, select the appropriate template (e.g., `frameworks/react-ts`). Select `Git Content (Default Branch)` for `Template Items`.

Once the new repo is created, clone it to your own workstation inside the `d:\es2027-s17-hu-r2` folder.

### Using npm modules

The npm modules will be accessible via a local npm cache. This means that even though there will be no internet access to the machines, you will be able to install the available npm modules to the projects as usual, and the `npm install` command issued on the cloned template projects will install all the npm modules needed for your project.

The available npm modules:

- express
- mysql
- mysql2
- vue-router
- react-router
- react-router-dom
- axios
- sass
- tailwindcss
- bcrypt
- _and all the types (@types/) needed for the TS projects_

### Laravel projects, composer install

The Laravel project contains all the necessary files, so you will **not** need to `composer install`. Your workstation has PHP 8 installed, so you can use the `php artisan` commands in the Laravel project.

### Deployment

When you commit and push your work, the deployment will start automatically. You can follow the process in the Gitea interface under the Action tab. Once the deployment is complete, your project will be available at https://cXX-module-Y.ssa.skillsit.hu, where `X` is your workstation number and `Y` is the module letter.

### Database access

You will have your own database on the MySQL database server (`db.ssa.skillsit.hu`) available on the local network. You will need to use this database for development, and the same database will provide the data for your projects deployed to the server. A database dump will be provided to get the initial data. During the marking, the database will be restored to its original state using the same dump.
