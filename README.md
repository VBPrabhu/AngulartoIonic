# Start create Angular Basic Project

clone git repository and check the angular code and angular converted code

Here's what is in the project:

* Angular scripts and TypeScript configuration are ready to go
* A simple app component 
* Bootstrap for CSS

This is a very simple "Hello World" project to help get you started.to simplify the process of writing Angular code. The code snippets make it easy to build Angular components, services, pipes, directives and more.

## Run the Angular Application

1. Install the Angular CLI

    `npm install -g @angular/cli`

1. Run `npm install`

1. Run `ng serve -o`

# Angular <--> Ionic project Migration

<img width="1440" alt="screen shot 2018-06-05 at 21 01 56" src="https://user-images.githubusercontent.com/26504978/40997331-89e1306c-6904-11e8-87fa-acf2a8c37525.png">

# Now Challenge Starts

How to change the above project into ionic project. Small configuration required to convert Angular project to Ionic Project.
![1_awpxaxq_upheqig-inqifw](https://user-images.githubusercontent.com/26504978/40997582-81de69ba-6905-11e8-89f6-06b8202596b0.jpeg)

# Please follow the below steps to convert Angular project to Ionic Project

#REQUIREMENTS

*You must have installed your Cordova CLI, if not, refer to Cordova Getting Started and Documentation on how to achieve that.
*You have already created your Angular version and above project. This writing will be based on Angular CLI, so if you haven’t installed it, please visit Angular Documentation

## Getting Started

* [Download the installer](https://nodejs.org/) for Node.js 8 or greater.
* Install the ionic CLI globally: `npm install -g ionic`
* Clone this repository: `git clone https://github.com/VBPrabhu/AngulartoIonic`.
* Run `npm install` from the project root.
* Run `ionic serve` in a terminal from the project root.


# Do this conversion in your own effort with below steps

 ---------------------# START #----------------------------
 
# Step 1 - Create a new Ionic/Cordova Project, using the Ionic Command below:

 ```bash
    $ ionic start ionic blank --v2
 ```

# Step 2 - Add your Cordova Building Platform ( Android , iOS ):

```bash
    $ ionic platform add android ios
 ```
  
# Step 3 - Now Copy Folder from Angular Project

    ## Copy Steps
    Merge your Angular project with the Ionic project created by copying every folders and files other than below files

    * Dont copy package.json from Angular Project
    * Dont copy app.module.ts

# Step 4 - Migrate packge.json from Angular to Ionic

Carefully open the package.json file in the both directories and carefully merge the two files into one. The resulting package.json should look like below

![packagejson copy](https://user-images.githubusercontent.com/26504978/40999260-9eafaacc-690a-11e8-94ba-88fa36484f13.png)

# Step 5 - Migrate AppModule.ts file from Angular to Ionic

Carefully open the app.module.ts file in the both directories and carefully merge the two files into one. The resulting app.module.ts should look like below

**Existing Angular app.module.ts file**

> ![appmodule](https://user-images.githubusercontent.com/26504978/40999461-3f1294e8-690b-11e8-81d6-8fa1d48f8ab1.png)

**After Migration app.module.ts file in Ionic**

> ![ionicapp](https://user-images.githubusercontent.com/26504978/40999575-8e671de8-690b-11e8-88c9-733633e67d5c.png)

# Step 6 - Move main.ts file

Move main.ts file from outside app folder to inside app folder in Ionic project

# Step 6 - Check and Confirm projct name in config.xml file

# Step 7 - Check and Confirm project name in tsconfig.json 

![tsconfig](https://user-images.githubusercontent.com/26504978/40999999-e2bfa6ca-690c-11e8-9507-2d2d157d29bf.png)

# Now start to build ionic project

## Getting started

**Warning**

> Verify that you are running at least node 8.9.x and npm 5.x.x by running node -v and npm -v in a terminal/console window. Older versions produce errors, but newer versions are fine.

1. Go to project folder and install dependencies.
 ```bash
 npm install
 ```

2. Launch development server:
 ```bash
 npm start
 ```

**Note**

> You don't need to build the library because it's published in npm and added as dependency of the project.

## Deploying

* PWA - Un-comment [this](https://github.com/VBPrabhu/AngulartoIonic/ionic/src/index.html), run `npm run ionic:build --prod` and then push the `www` folder to your favorite hosting service
* Android - Run `ionic cordova run android --prod`
  - If you are deploying to Android 4.4 or below we recommend adding crosswalk: `cordova plugin add cordova-plugin-crosswalk-webview`
* iOS - Run `ionic cordova run ios --prod`
* ionic development build `ionic serve`

## Usage

Tasks                    | Description
-------------------------|---------------------------------------------------------------------------------------
npm i                    | Install dependencies
npm start                | Start the app in development mode
npm run test             | Run unit tests with karma and jasmine
npm run test:library     | Run unit tests for the library
npm run e2e              | Run end to end tests with protractor
npm run build            | Build the app for production
npm run build:library    | Build the library
npm run lint             | Run the linter (tslint)
npm run lint:library     | Run the linter for the library
npm run ci               | Execute linter and tests
npm run deploy           | Build the app and deploy dist folder to Github pages (angular-cli-ghpages) (fork to do this and remove CNAME file)
npm run sme              | Build and run source map explorer, really cool :)
npm run release          | Create a new release using standard-version
npm run docker           | Build the docker image and run the container


# Successfully Migrated from Angular project to Ionic project

![45091936-happy-smiley-emoticon-face](https://user-images.githubusercontent.com/26504978/40999913-a4b3cc3a-690c-11e8-9970-38a557101537.jpg)

