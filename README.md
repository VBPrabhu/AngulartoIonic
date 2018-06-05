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


