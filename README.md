# NASA-Pioneers

Original App Design Project - README Template
===

# NASA Pioneers

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
2. [Schema](#Schema)

## Overview
### Description
The NASA Pioneers will create an interface allowing users to keep up-to-date and refreshed on information and imagery of the celestial bodies orbiting the nearest parts of our solar system. Our application will include astronomy photos of the day taken by NASA satellites, insights and updates on the Mars weather, images provided by the Mars rover, and access to a wide array of NASA images and video libraries accumulated by NASA projects over the years. The ultimate of our app is to inform the general public on and celebrate the day-to-day accomplishments of space exploration.

### App Evaluation
[Evaluation of your app across the following attributes]
- **Category:** Science/Astronomy
- **Mobile:** This app will be primarily developed for a mobile interface, but can be expanded for computer use
- **Story:** Provided daily images from oribiting satellites and Mars Rover, provide weather updates and information on Mars, and provide users access to a gallery of NASA images and video archives 
- **Market:** This app is open to any individuals who share an enthusiasm for the final frontier
- **Habit:** The usage of this app relies pirmairly on user interests in space exploration and updates, but can also be used casually for the casual audience 
- **Scope:** As of right now this is just formatted like a image based app, in which we provide users with various media revolving around oribiting bodies and weather. In the future, we hope to make this app more educational and news based. 

## Product Spec

### 1. User Stories (Required and Optional)

**Required Must-have Stories**

* Users can view astronomy picture of the day
* Users can access a limited version of the NASA image and video gallery
* Users can see information regarding the weather and objects found on Mars 

**Optional Nice-to-have Stories**

* Users will have access to a general space weather database which will include models and forecasts
* Users can favorite and save/download images 


### 2. Screen Archetypes

* Picture of the Day
   * Users can view astronomy picture of the day
* NASA Gallery
   * Users can access a limited version of the NASA image and video gallery
* Mars Exploration 
   * Users can see information regarding the weather and objects found on Mars 

### 3. Navigation

**Tab Navigation** (Tab to Screen)

* Picture of the Day
* Gallery
* MARS

**Flow Navigation** (Screen to Screen)

* Image Selection -> Open image on a larger scale on a new tab
* Download -> Users will be able to save an image from the app to their phone


## Schema 
### Models
#### Post

   | Property      | Type     | Description |
   | ------------- | -------- | ------------|
   | APOD          | JSON Object | Astronomy Picture of the Day pulled from NASA API |
   | weatherInfo   | JSON Object | information of Mar's climate/weather |
   | MARSImage     | JSON Object | images of MARS taken by Mar's Rovers |
   | gallery       | JSON Object | general image media relating to space taken by NASA |

### Networking
#### Network requests by screen 
  - Home Screen
    - (Read/GET) Obtain Astonomy Picture of the Day
  - Gallery
    - (Read/GET) Recieve NASA image Library
  - MARS
    - (Read/GET) Recieve Mar's Rover images
    - (Read/GET) Recieve Mar's weather data  
  
