# Angular 2 create and delpoy for first time

First time creating and deploying angular2 app

## Getting Started

These instructions teach you how to create and deploy angular2 using Firebase and Angular2 CLI

### Prerequisites

What things you need to install the software and how to install them

- nodejs
- npm
- git
- angular2 CLI


### Installing

A step by step series of examples that tell you have to get a development env running

Say what the step will be

```
nodejs & npm:
[https://nodejs.org/en/download/]
```

```
git:
[https://git-scm.com/book/en/v2/Getting-Started-Installing-Git]
```

```
angular2 CLI:
$ npm install angular-cli -g
```


## Create your app

Create app: 
$ ng new my-app

Enter app directory: 
$ cd fb-host-test

Run app: 
$ ng serve


goto [http://localhost:4200] and see if app works.

## Deployment
build app for deploy:
$ ng build --prod

goto [https://console.firebase.google.com/] and create a new Firebase project.

install firebase tools:
 $ npm install -g firebase-tools

deploy to firebase:
$ firebase login

after authentication, run:
$ firebase init

First of all you're being asked which of the Firebase client features you want to use. Select the option Hosting: Configure and deploy Firebase Hosting site. Next the Firebase client will ask which folder to use for deployment. Type in dist. That is important because that is the location where our production build is stored. 
 
Next the question is ask if this app is a single page app and if it should rewrite all URLs to index.html. In our case we need to answer yes. 
 
Last question is if Firebase should over write file index.html. The answer to that question is no.


now run:
 $ firebase deploy
## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## References

* **Hosting Angular 2 Applications On Firebase** - *Initial work* - [Sebastian Eschweiler](https://medium.com/codingthesmartway-com-blog/hosting-angular-2-applications-on-firebase-f194688c978d#.gt2pkhomp)
