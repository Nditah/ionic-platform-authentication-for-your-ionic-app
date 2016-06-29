# How to integrate user authentication to your ionic app
In this tutorial we are going to explain how to add **Log in**, **Log out**, and **Sign up** functionality to your ionic app using the [Ionic Platform](http://ionic.io/platform "Ionic Platform") services.

## Follow the step-by-step instructions available here: https://ionicthemes.com/tutorials/about/add-ionic-platform-authentication-to-your-ionic-app

## Setup

### Install Ionic
You can find the **_Ionic_** official installation documentation [here](http://ionicframework.com/docs/guide/installation.html).

1. Make sure you have an up-to-date version of **_Node.js_** installed on your system. If you don't have **_Node.js_** installed, you can install it from [here](http://nodejs.org/).
2. Open a terminal (Mac) or a command interpreter (`cmd`, Windows), and install **_Cordova_** and **_Ionic_**:
	- `npm install -g cordova`
	- `npm install -g ionic`
	- On a Mac, you may have to use `sudo` depending on your system configuration: `sudo npm install -g cordova ionic`
3. If you already have **_Cordova_** and **_Ionic_** installed on your computer, make sure you update to the latest version:
	- `npm update -g cordova`
	- `npm update -g ionic`
	- Or `sudo npm update -g cordova ionic`

Follow these links if you want more information:
* [Ionic **_Getting started_** guide](http://ionicframework.com/getting-started)
* [Ionic **_Documentation_**](http://ionicframework.com/docs)
* [Visit the Ionic **_Community Forum_**](http://forum.ionicframework.com)

### Git & `ionic start`

First we need to link this new Ionic project with our reference repo on github. Clone this repo so we can start working on the app:
- `git clone https://github.com/ionicthemes/IonicTest.git`
- `cd IonicTest`

After this, we need to set up some stuff before starting working on the **_Ionic_** project. To do so, run these commands:
- `npm install`
- `bower install`
- `ionic setup sass`
As we are going to use Ionic Platform services, we need to install and init the platform services with this command:
- `ionic add ionic-platform-web-client`
- `ionic io init`

**NOTE**: The last step is critical, if we install the *ionic-platform-web-client* but don't init, then we may find some bugs when serving the app.

Finally, to see the current state of the project, run:
- `ionic serve`
