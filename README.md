<h1 align="center">
  <br>
  <a href="https://pendown.icheft.tech"><img src="./logo.png" alt="PenDown" width="70"></a>
  <br>
  PenDown
  <br>
</h1>

<h3 align="center">Official Documentation (with Instructions)</h3>
<h4 align="center">IM 3007 Term Project Group 帝大南院</h4>

<p align="center">
  <a href="https://pendown.icheft.tech">
    FE 
    <img src="https://shields.io/website?down_color=red&down_message=down&up_color=success&up_message=up&style=flat-square&url=https%3A%2F%2Fpendown.icheft.tech"
         alt="website status">
  </a>
   • 
  <a href="https://github.com/AOPLab/PenDown-be">
    BE (Repository)
  </a>
</p>

<p align="center">
  <a href="https://youtu.be/uMHKi_Mrows">
    Promo Video
    <img src="https://shields.io/youtube/views/uMHKi_Mrows"
         alt="YouTube Intro">
  </a>
  • 
  <a href="https://youtu.be/bjGUQJ9m6eQ">
    Milestone 3 Presentation
    <img src="https://shields.io/youtube/views/bjGUQJ9m6eQ"
         alt="YouTube Demo">
  </a>
</p>

<p align="center">
    <img src="https://github.com/Buuntu/fastapi-react/raw/master/assets/react-logo.png" height="50"
            alt="react">
    <img src="https://raw.githubusercontent.com/chakra-ui/chakra-ui/main/logo/logo-colored@2x.png" height="50"
            alt="chakra">
    <img src="https://user-images.githubusercontent.com/727262/40395108-6bcc327a-5e1e-11e8-9f76-3917983b8563.png" height="50"
         alt="go">
    <img src="https://github.com/Buuntu/fastapi-react/raw/master/assets/postgres.png" height="50"
         alt="postgresql">
    <img src="https://miro.medium.com/max/256/0*AqO_2lNemh_Fl9Gm.png" height="50"
         alt="drone">
</p>

## Table of Contents <!-- omit in toc -->

+ [Introduction](#introduction)
+ [Demo](#demo)
+ [Development](#development)
    + [Frontend](#frontend)
        + [Dev Environment](#dev-environment)
        + [Development](#development-1)
        + [Unit Testing](#unit-testing)
    + [Backend](#backend)
        + [Before You Start](#before-you-start)
        + [Set Up](#set-up)
        + [Unit Testing](#unit-testing-1)
+ [Acknowledgements](#acknowledgements)
+ [Contributions](#contributions)

## Introduction

**PenDown** is a platform for sharing notes and ideas. We are on a mission to bring together the best notes from students and professionals all over the world. Pen down, and you can start absorbing knowledge from others!

More can be seen on [our website](https://pendown.icheft.tech) and also on our [About page](https://aoplab.notion.site/About-d39c56d855d449d186f90a20a9d0e451).

## Demo 

Our application is deployed at <https://pendown.icheft.tech>. We did not set up our Backend service site, but the API documentation can be given upon request. 

We recommend you to run this project by directly going to our site and experience our service yourself. 

#### ‼️ Please visit <https://pendown.icheft.tech> · <https://pendown.icheft.tech> · <https://pendown.icheft.tech> before you test it out locally. <!-- omit in toc -->

IF, local deployment is still necessary, instructions are shown as follows:

## Development

+ We have set up our [frontend](https://github.com/AOPLab/PenDown-fe-chakra) and [backend](https://github.com/AOPLab/PenDown-be) in different repositories. 
+ You can find all the instructions on this page.

### [Frontend](https://github.com/RDOGS-Friendz/fds-fe)

<img src="https://github.com/Buuntu/fastapi-react/raw/master/assets/react-logo.png" height="25"
            alt="react">
<img src="https://raw.githubusercontent.com/chakra-ui/chakra-ui/main/logo/logo-colored@2x.png" height="25"
            alt="chakra">
![](https://shields.io/badge/platform-Linux%20%7C%20macOS%20%7C%20Windows-%23989898?style=flat-square) [![](https://shields.io/github/stars/AOPLab/PenDown-fe-chakra?style=social)](https://github.com/AOPLab/PenDown-fe-chakra)

* Again, we have deployed our frontend website on <https://pendown.icheft.tech>. No need to run this app on your local environment.
* Please ask the development team for the `.env` file. 

**🔩 For Local Development:**

#### Dev Environment

- OS: macOS / Linux / Windows
- PM: Yarn
- IDE: Visual Studio Code (recommended)
  - required plugins:
    - [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
    - [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
    - [Prettier ESLint](https://marketplace.visualstudio.com/items?itemName=rvest.vs-code-prettier-eslint)

#### Development

1. Clone this repository
  ```
  git clone https://github.com/AOPLab/PenDown-fe-chakra.git
  ```
2. Open the directory in your favorite text editor (**VS Code** is highly recommended). If you are using VS Code, please make sure you have the mentioned plugins installed.
4. In terminal, use `yarn` to install the [dependencies](package.json).
5. Before you run our app, please [connect to a backend server (either ours or yours)](#connecting-to-our-server)
6. Run `yarn start` to run the app in the development mode.

##### Connecting to Our Server <!-- omit in toc -->

You have two options:

1. Please contact us for the `.env` file. Our present data are all stored in our server.
2. If you want to replicate this app, please also consider to clone our [`PenDown-be` repository](https://github.com/AOPLab/PenDown-be.git), and follow the instructions there.

  In your `.env`, you should put in:

  ```
  SKIP_PREFLIGHT_CHECK = true
  REACT_APP_API_ROOT='http://127.0.0.1:8080'
  REACT_APP_OAUTH_ID=YOUR_AUTH_ID
  ```

  > You should sign up for your own "Continue with Google" AUTH ID. That said, it won't cost you anything if you don't do so, that'll allow your clients to continue without Google.

  That'll do it.

#### Unit Testing

Please check out our [Frontend repo](https://github.com/AOPLab/PenDown-fe-chakra#unit-test) to see the instructions for unit testing. 

### [Backend](https://github.com/AOPLab/PenDown-be)

<img src="https://user-images.githubusercontent.com/727262/40395108-6bcc327a-5e1e-11e8-9f76-3917983b8563.png" height="25"
         alt="go"><img src="https://github.com/Buuntu/fastapi-react/raw/master/assets/postgres.png" height="25"
         alt="postgresql">
[![](https://shields.io/github/stars/AOPLab/PenDown-be?style=social)](https://github.com/AOPLab/PenDown-be) 

* We have deployed our backend website, yet there is no documentation available via the Internet. However, that means you DO NOT HAVE to start the server on your local environment in order to get your replica working, simply connecting to our backend is fine.
* API Brainstorming Documentation is upon request
* Please ask the development team for the `.env` file and the `pendown-firebase.json` file. 

**🪛 For local development:**

#### Before You Start

**Notice** (for Windows users):
   
> If you don't want to set up environment, you can jump to the [Set Up](#set-up) section and then go for [Option 2 - Using Docker](#using-docker)
>   
> Although you download both golang and gcc, you may still start fail due to package dependency. 
>    
> Therefore, **[Docker](https://www.docker.com/get-started/) is the recommended method**.

1. Install golang
   
   You should follow the official [install instruction](https://go.dev/doc/install).

2. Check golang version
   
   You can check in your terminal.

   ```shell
   go version
   
   // expected output, at least 1.17.6
   // go version go1.17.6
   ```

3. Install gcc
   
   Check you have gcc or type `gcc -v ` in terminal. (Version at least 8.1.0 or above)
   

#### Set Up

1. Clone project

    ```shell
    git clone https://github.com/AOPLab/PenDown-be.git
    ```

2. Change directory

   ```shell
   cd github.com/AOPLab/PenDown-be
   ```

3. Copy configuration files

    ```shell
    cp .env.example .env
    ```

4. Put firebase file (`pendown-firebase.json` file)
   
   Put your firebase secret file (json format) in root. Follow [official document](https://firebase.google.com/) to get it.

   Or contact us to get the file, which is recommended.


5. Edit `.env` file

    ```txt
    # PostgreSQL
    PG_HOST=
    PG_PORT=5432
    PG_USERNAME=postgres
    PG_PASSWORD=
    PG_DBNAME=

    # Firebase
    SA_PATH=YOUR_FIREBASE_SECRET_FILE_PATH
    BUCKET_NAME=YOUR_FIREBASE_BUCKET_NAME

    # jwt
    jwt_token=
    ```

6. Choose either [Option 1](#option-1---using-go-directly) or [Option 2](#option-2---using-docker) to start up the server.


##### Option 1 - Using Go Directly <!-- omit in toc -->

1. Start backend service 

    ```shell
    go mod download
    go mod tidy
    go run .
    ```

##### Option 2 - Using Docker <!-- omit in toc -->

1. build

   ```shell
    docker build -t 'pendown-be' .
   ```

2. run

   ```shell
    docker run -d -p 8080:8080 pendown-be
   ```


After all this, you shall be able to visit http://localhost:8080/ in your browser, and it should display "404 page not found".

#### Unit Testing

Please check out our [Backend repo](https://github.com/AOPLab/PenDown-be#unit-testing) to see the instructions for unit testing. 



## Acknowledgements

This documentation repository is based on [FDS-docs](https://github.com/RDOGS-Friendz/fds-docs) published by @icheft.

## Contributions 

We truly are happy for and open to any sorts of contributions. It can be an issue or a PR. If you have any trouble using our sites, please don't hesitate to contact us. Thanks <3.