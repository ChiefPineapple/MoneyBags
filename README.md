<div align="center">

  <img src="./assets/logo.png" alt="logo" width="200" height="auto" />
  <h1>Money Bags</h1>
  
  <p>
    This is a personal project I'm starting with the aim of practicing my web development and to hopefully help me manage my personal finances.</b>
  </p>

  
<!-- Badges -->
<p>
  <a href="https://github.com/ChiefPineapple/MoneyBags/graphs/contributors">
    <img src="https://img.shields.io/github/contributors/ChiefPineapple/MoneyBags" alt="contributors" />
  </a>
  <a href="">
    <img src="https://img.shields.io/github/last-commit/ChiefPineapple/MoneyBags" alt="last update" />
  </a>
  <a href="https://github.com/ChiefPineapple/MoneyBags/network/members">
    <img src="https://img.shields.io/github/forks/ChiefPineapple/MoneyBags" alt="forks" />
  </a>
  <a href="https://github.com/ChiefPineapple/MoneyBags/stargazers">
    <img src="https://img.shields.io/github/stars/ChiefPineapple/MoneyBags" alt="stars" />
  </a>
  <a href="https://github.com/ChiefPineapple/MoneyBags/issues/">
    <img src="https://img.shields.io/github/issues/ChiefPineapple/MoneyBags" alt="open issues" />
  </a>
</p>
   
<h4>
    <a href="https://github.com/ChiefPineapple/MoneyBags/issues/">Report Bug or Request a Feature</a>
  </h4>
</div>
<br />

<!-- Table of Contents -->
# Table of Contents
- [About the Project](#about-the-project)
  * [Progress](#progress)
  * [Tech Stack](#tech-stack)
  * [Features](#features)
  <!-- * [Environment Variables](#environment-variables) -->
  * [Roadmap](#roadmap)
<!-- - [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Setup](#setup) -->
<!--  * [Usage Guide](#usage-guide) -->

  
<!-- About the Project -->
## About the Project
I used to manage a budget very strictly from late high-school through the first year or two after college. But after taking on more bills, subscriptions, and merging some finances with my partner, I've found it extremely difficult to keep up with constantly updating an excel spreadsheet to reflect my few accounts and the constant small transactions that happen. I've also recently started to make several API's using FastAPI. So I thought it might be fun to try and get some more practice while also seeing if I can develop something that might simplify my personal finance management with automations, databases, and maybe presenting the data in an easier to read format with charts or fun colors. We'll see.

<!-- Screenshot 
<div align="center"> 
  <img src="https://placehold.co/600x400?text=Your+Screenshot+here" alt="screenshot" />
</div> -->
<!-- Progress -->
### ✅ Progress
I have made 0 progress so far, not even a fully fleshed out plan. But you have to start somewhere and I find that getting a project folder going, a git, and a README helps me solidify a generic gameplan and track progress.
<!-- TechStack -->
### 🚀Tech Stack
I'm planning to deploy this on a home server using docker, with a database, an API, and a front end. The specifics of that are yet to be determined.
<details>
  <summary>Database</summary>
    <ul>A Postgres Database that runs in a docker container with a mounted volume for data persistence.</ul>
</details>
<details>
  <summary>API</summary>
    <ul>FastAPI serves the front end as well as the backend actions of exporting the desired data from TCGPlayer and pushing it to the database.</ul>
</details>
<details>
  <summary>Front End</summary>
    <ul>I'm not too sure what I'll use to serve my front end. I might try React, who knows?</ul>
</details>
<!-- <details>
  <summary>Metabase</summary>
    <ul>A metabase container with access to the MySQL database provides the ability to generate custom reports of your data however your Metabase capability allows.</ul>
</details> -->

<!-- Features -->
### 💪Features
<!-- - __Easy deployment:__ Can simply pull and deploy with docker and git. I've providing a simple guide for setting up.
- __Scalable:__ Adjust your hardware to meet the size of your business, but is built to run on budget hardware for accessibility.
- __FastAPI:__ Utilizing FastAPI allows for the front and backend to be run together on one server, as well as easy asynchronous programming to improve the speed of all the data pulling + pushing that occurs in this project.
- __Metabase:__ Features Metabase, an open source tool with an active community. This means there are plenty of resources for learning to create your own more complicated reports if you desire. Or you can use the basic ones I showcase.
- __Security:__ This app is meant to be internally hosted. It requires admin level access to do user management and JWT's to manage endpoint calling. If a token is stolen, it will be valid until it expires. -->
- __Recurring Charges__: I want to for sure have the ability to set recurring charges that will automatically apply themselves to account balances and appear in logs.
- __Budget Balances__: I want to have the option to  create budgets, that will be a portion of income and can be affected by charges that fall under certain categories.
- __Possible Automations__: I like the idea of possibly automating charge entries based on email or text notifications, but I'm not 100% sure I'll do this. The idea is great, but obviously security is paramount and as much as automations may take away from the entry workload, they could also add an annoying task of weeding out false entries due to refunds or charges that later change amount. (Like meals before tips, or gas stations that charge very high up front to credit cards before adjusting the charge to the true amount later)

<!-- Env Variables -->
<!-- ### ⚙️Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`DATABASE_USER`
`DATABASE_PASSWORD`
`FASTAPI_PORT`
`FASTAPI_USER`
`FASTAPI_PASSWORD`
`METABSE_PORT`
`METABASE_USER`
`METABASE_PASSWORD` Optionally: `MYSQL_PORT` -->

### 🚗Roadmap
I plan to start by wire framing my idea of how it might look to have a better idea of what sort of features and use cases I envision. This will help iron out the sort of tables and structure I need for the database and API endpoints.
<!-- <ol>
  <!-- <li>README + Planning</li>
  <ul>
    <li>(This will be continually updated)</li>
    <li>REAMDE will get more docs added as real code gets created</li>
    <li>Planning will feature more concrete steps as development continues</li>
  </ul>
  <li>Docker Setup for MySQL with tables for TCGPlayer Exports</li>
      <ul>
        <li>Will need to identify desired reports from TCGPlayer to build around</li>
        <li>Setup FastAPI SQLModel classes and table creation from the server</li>
        <li>Get a docker compose started to have a MySQL container spun up</li>
      </ul>
    <li>FastAPI Setup</li>
      <ul>
        <li>Routes for Authorization and user management</li>
        <li>Routes for scraping reports from TCGPlayer seller side</li>
      </ul>
    <li>Metabase Setup</li>
      <ul>
        <li>Add a metabase container to the docker compose with visability to the MySQL container</li>
        <li>Add basic guide to creating reports after getting the database populated</li>
      </ul>
</ol>
<!-- Getting Started -->
<!-- ## Getting Started

<!-- Prerequisites -->
<!-- ### 📚Prerequisites

Ideally you'll have git on your deployment machine to clone the repository. (It's not a must, you can always manually download all the files and recreate the structure on the machine. But git is far cleaner). You'll also need docker and docker compose on the deployment machine. __You don't necessarily need Docker Destkop. (It's just a nice to have if you are using a machine that has the capability). You can just use Docker Engine if you are running this project off a server and don't need or have a GUI.__


<a href="https://git-scm.com/install/">Git Installation</a>

<a href="https://docs.docker.com/desktop/">Docker Desktop Installation</a>

<a href="https://docs.docker.com/engine/install/">Docker Engine Installation</a>


<!-- Setup -->
<!-- ### 🚧Setup

1. __Clone the repository using git__ - <a href="https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository"> Repository Cloning Instructions</a>
2. __Alter the environment variables in the .env file__ - It's best practice to use different passwords for each user and choose strong passwords. There are suggested default ports for FastAPI and Metabase, these can be altered if you wish. The MYSQL_PORT variable can uncommented and set if you wish to be able to interact with the database directly.
3. __Run the containers__ -  Run the following command from inside the project folder. *You can run it without -d at first to see it's logs and debug any problems that may arise. Add -d for deployment so it runs in headless mode.*

```bash
  docker compose up -d
```
4. Create your metabase user, then add the database via the database connection url in your .env file. -->

<!-- Usage Guide -->
<!--### Usage Guide -->