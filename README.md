<h1> Taxi Management System </h1>

A PBL (Project Based Learning) project for the course DBE (Database Engineering) at Kolhapur Institute of Technology.  
A simple Taxi Management System.

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**

- [Features](#features)
- [User Interface](#user-interface)
  - [Home Screen](#home-screen)
  - [Registration](#registration)
    - [User Registration](#user-registration)
    - [Driver Registration](#driver-registration)
  - [Login](#login)
    - [Admin Login](#admin-login)
    - [User-Driver Login](#user-driver-login)
  - [Dashboard](#dashboard)
    - [Admin Dasboard](#admin-dasboard)
    - [User Dashboard](#user-dashboard)
    - [Driver Dashboard](#driver-dashboard)
- [Technical Details](#technical-details)
- [Requirements](#requirements)
- [Database](#database)
- [Database Schema](#database-schema)
- [Dependencies](#dependencies)
- [How to Run](#how-to-run)
- [Application Pages](#application-pages)
- [Our APIs](#our-apis)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


## Features

- User and Driver Registration.
- User can book a trip and Driver can accept the booking.
- User and Driver can view his/her booked/accepted trips.
- Driver can view the available trips along with the distance and fare.
- User can see the Driver's details when he/she accepts the booking.

## User Interface

### Home Screen
> <img height="auto" src="./Documentation\UI\Home.jpg" />

<hr>

### Registration
> 
> #### User Registration 
> > <img  src="./Documentation\UI\registration-user.jpg"/>
> 
> #### Driver Registration 
> > <img  src="./Documentation\UI\registration-driverLicenceInfo.jpg"/>
> 
<hr>

> ### Login
> 
> #### Admin Login
> > <img  src="./Documentation\UI\login-admin.jpg"/>
> 
> #### User-Driver Login 
> > <img  src="./Documentation\UI\login-userDriver.jpg"/>
> 
<hr>

### Dashboard
> 
> #### Admin Dasboard
> > <img  src="./Documentation\UI\admin1.jpg"/>
> > <img  src="./Documentation\UI\Admin2.jpg"/>
> > <img  src="./Documentation\UI\Admin3.jpg"/>
> > <img  src="./Documentation\UI\Admin4.jpg"/>
> 
> #### User Dashboard 
> > <img  src="./Documentation\UI\dashboard-user.jpg"/>
> 
> #### Driver Dashboard 
> > <img  src="./Documentation\UI\dashboard-driver.jpg"/>
> 
## Technical Details

- Frontend: Bootstrap, HTML, CSS, JavaScript
- Backend: NodeJS, ExpressJS
- Database: MySQL

## Requirements

- [NodeJS](https://nodejs.org/en/)
- [MySQL](https://www.mysql.com/)
- [Below DataBase Structure](#database "Database & Database Structure")

## Database

- Name: taxi_management_system
- Tables:
  - user
  - driver
  - admin
  - taxi
  - trip

## Database Schema

- user:  
![image](https://user-images.githubusercontent.com/66154908/144718389-f33644cc-db92-4d83-a423-b0d74cbdbaa1.png)

- driver:  
![image](https://user-images.githubusercontent.com/66154908/144718410-7401f1c3-b3fe-479d-9226-2d8a9b7a2e53.png)

- admin:  
![image](https://user-images.githubusercontent.com/66154908/144718433-06abc683-b65e-48e0-836f-f31179d2c751.png)

- taxi:  
![image](https://user-images.githubusercontent.com/66154908/144718471-236f7daa-728e-499c-b0ec-fcaf733f969d.png)

- trip:  
![image](https://user-images.githubusercontent.com/66154908/144718450-6b083140-6987-4ae8-9ad5-c32c16ca65c9.png)

## Dependencies

- express
- mysql
- nodemon

## How to Run

- cd <root_directory>
> ```sh
> npm install
> npm start
> ```
- Click on the link to open the application: http://localhost:1412/

## Application Pages

- Home Page: http://localhost:1412/
- User Registration Page: http://localhost:1412/signup-user/
- Driver Registration Page: http://localhost:1412/signup-driver/
- Login Page: http://localhost:1412/login/
- User Dashboard Page: http://localhost:1412/user/
- Driver Dashboard Page: http://localhost:1412/driver/
- Admin Login Page: http://localhost:1412/admin-login/
- Admin Dashboard Page: http://localhost:1412/admin/

## Our APIs

- Registration:
  - User: `/api/registration/user`
  - Driver: `/api/registration/driver`

- Login: `/api/login/:role`

- Session-End: `/api/session-end/:role`

- Credentials: `/api/credentials/:role`

- Admin Queries:
  - User: `/api/query/user`
  - Driver: `/api/query/driver`
  - Trip: `/api/query/trip`
  - Custom: `/api/query/custom`

- Trip:
  - Booking: `/api/trip/booking`
  - History: `/api/trip/history/:role`
  - Accepting: `/api/trip/accepting`
  - Available: `/api/trip/available`
