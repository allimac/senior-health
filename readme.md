![makersacademy](https://github.com/allimac/resources/blob/master/ma_logo.png)

**week 11 / Final project**

================================

![Senes logo](https://github.com/allimac/senior-health/blob/development/mobile/www/img/logo.png)

# Senes

This is the final project for our Makers Academy coding bootcamp! The projects consists of a mobile app and an API, to allow people to provide better care for their elderly relatives.

# Table of Contents

* [Authors](#Authors)
* [The problem statement](#the-problem-statement)
* [Our solution](#our-solution)
  * [Technologies](#technologies)
  * [Instructions](#instructions)
  * [User stories implemented](#user-stories-implemented)
* [Future improvements](#future-improvements)


## Authors

[Emma Beynon](https://github.com/emmabeynon)

[Jamie Brown](https://github.com/jamiebrown201)

[Alan Gabbianelli](https://github.com/alangabbianelli)

[Camilla Colombo Serri](https://github.com/allimac)

[Katie Smith](https://github.com/klssmith)


## The problem statement
“Because I lead a busy life and I am time-poor, I don’t know the health and wellbeing status of my elderly relative”

## Our solution
We decided
## Technologies
#### API/Server
* Rails
* Ruby

#### Client
* Ionic
* AngularJS
* HTML5
* CSS
* Sass

#### Testing
* RSpec
* Karma
* Protractor
* Jasmine
* Shoulda

## Instructions
This repository includes a folder `web` which contains the codebase for the API, and a folder `mobile` with the code for the Ionic mobile app.  You will need a valid Fitbit account to connect the app to your Fitbit device.  To get started, fork this repo and run:

```
$ git clone < your forked repo URL >
$ cd < your forked repo name >
$ npm install -g cordova ionic
$ npm install -g ios-sim
$ cd mobile
$ npm install
$ cd ../web
$ bundle install
$ bin/rake db:create
$ bin/rake db:migrate
```

The API has been deployed to [senior-health.herokuapp.com](https://senior-health.herokuapp.com).  To run the app with the deployed API, open `/mobile/www/services.js` and ensure that `var address = remoteUrl`.

To run the API locally, open `/mobile/www/services.js` and ensure that `var address = localUrl`. Next, run the following commands:
```
$ cd web
$ rails s
```

To load the app, run:
```
$ cd mobile
$ ionic platform add ios
$ ionic build ios
$ ionic emulate ios
```

## User stories implemented

```
As a relative of an elderly person
So that I can track their health
I would like to link their Fitbit device

As a relative of an elderly person
So that I can get have quick information at a glance
I would like to easily see the overall conditions of the elderly relative

As a relative of an elderly person
So that I can get more detailed information about their health on that day
I would like to see their heart rate values

As a relative of an elderly person
So that I can see if they have done any physical activity
I would like to see the amount of physical activity they have done

As a relative of an elderly person
So that I can see if they are sleeping properly
I would like to see how much they have slept

As a relative of an elderly person
So that I can monitor their health over a wider range of time
I would like to see a weekly summary of their vital stats

As a relative of an elderly person
So that I can help them to remember to take medications
I would like to be able to set reminders for their device

As a relative of an elderly person
So that I can protect my elderly relative privacy
I would like to unlink my phone to the connected account (logout)

```

## Future improvements

This project wants to be an exploration into a field, that of wearable technology for the elderly, that could have
```
As an elderly user
So that I don't have to worry about syncing my device
I would like to have a device that easily syncs data to Fitbit continuously

As a relative of an elderly person
So that I can act on a health issue
I would like to receive an alert if their vital stats are outside the normal range

As a relative of an elderly person
So that I can find them if they are lost
I would like to see what their GPS location is
```
