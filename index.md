---
title: Rainbow Clubs
---

# Table of contents

* [About Rainbow Clubs](#about-rainbow-clubs)
* [Approach](#approach)
* [Use Case Ideas](#use-case-ideas)
* [Advanced Features](#advanced-features)
* [User Guide](#user-guide)
* [Developer Guide](#developer-guide)
* [Our Team](#our-team)

# About Rainbow Clubs

* [Live Demo](http://rainbowclubs.meteorapp.com)
* [Github Repository](https://github.com/rainbowclubs/rainbowclubs)
* [Project Board Milestone 1 (Completed)](https://github.com/rainbowclubs/rainbowclubs/projects/1)
* [Project Board Milestone 2 (In Progress)](https://github.com/rainbowclubs/rainbowclubs/projects/2)
* [Project Board Milestone 3 (In Progress)](https://github.com/rainbowclubs/rainbowclubs/projects/3)

The problem: UH Manoa has over 200 Registered Independent Organizations, plus many more that do not have this “official” status but are nonetheless active organizations. Unfortunately, there is no easy way for students to learn (a) what student clubs (both registered and unregistered) exist, what they do, and how to get further involved.

The solution: The Rainbow Clubs application will provide a centralized directory for UH Manoa student clubs. UH Manoa students can login to browse a well organized directory of all current student clubs, with brief descriptions, meeting times and locations, URLs to their websites (if any), contact information for officers, and a few select photos.

# Approach

Rainbow Clubs has three user roles, all of whom login with their UH ID. Regular users browse the directory. Club Admins have the ability to edit the data associated with their club. Super Admins make sure site content is appropriate and grant “club admin” privileges to selected users.

The site should not simply support browsing by a list of clubs in alphabetical order, but should also allow filtering by interest area. For example, “athletic” clubs, “art” clubs, “music” clubs, etc. A club can belong to multiple interest areas.

Users can specify interest areas, and be notified when a new club is created matching that interest area (or an existing club adds that interest area).

Admins can monitor the site for inappropriate content, and create new categories of musical tastes, capabilities, and goals.

# Use Case Ideas

* New user goes to landing page, logs in, gets home page, sets up profile.
* Admin goes to landing page, logs in, gets home page, edits site.
* User goes to landing page, logs in, looks for clubs of interest.
* Club admin goes into site, updates their club profile.

# Advanced Features

* Upload club data from the CSV version of the RIO spreadsheet.
* Notify admins when club data changes so they can review for appropriateness.
* Provide “expiration date” for club listings (either one semester or one academic year). To retain a listing, the club admin or admin must login and click a “renew” button for the club to re-list it in the site.
* Allow students to rate clubs.

# User Guide
The following sections describe the main features of this application as of Milestone 1.

## Landing Page
The goal of this page is to describe the function of the website.
When you retrieve the application at [http://localhost:3000](http://localhost:3000), you will receive the following page:

<img src="doc/m1/landing.png">

## Login Page
Clicking on the Login link and then on the Sign In menu item, you will receive the following page:

<img src="doc/m1/login.png">

## Register Page
Clicking on the Login link and then on the Sign Up menu item, you will receive the following page:

<img src="doc/m1/register.png">

## Landing Page After Login (Non Admin User)
Once a non admin user logs in or registers, the top navbar changes as follows:

<img src="doc/m1/landing_user.png">

## Landing Page After Login (Admin User)
Note that we did not have any admin functionality for the first milestone, therefore the landing page is the same as the non admin user.
Once an admin logs in, the top navbar changes as follows:

<img src="doc/m1/landing_admin.png">

## Listing Page
The purpose of this page is to list all registered RIOs and clubs in the UH database.  Each club will have a card that will contain a description, tags, a link to the RIO/club website (if they have one), and a link to a seperate page that will have further descriptions of the RIO/club.

<img src="doc/m1/club_listing.png">

# Developer Guide

## Backend System

This application was built on meteor-application-template-react.  For information regarding this template, please refer to [https://ics-software-engineering.github.io/meteor-application-template-react/](https://ics-software-engineering.github.io/meteor-application-template-react/)

## Installation

First, [install Meteor](https://www.meteor.com/install)

Optionally, create a new GitHub repository and clone it to your local machine.

Second, [download a copy of Rainbow Clubs](https://rainbowclubs.github.io/).

Third, uncompress the zip file and copy the files and directories into your working directory.

Fourth, in a terminal window, change to the app directory and install the required libraries:

```
cd /path/to/project
cd /app
meteor npm install
```

## Running the Application

Once you have completed the installation, you can start the application:

```
meteor npm run start
```

The first time you run the application, it will create some default users and date. Note that you can safely ignore warning about bcrypt.

## Viewing the Application

Once you have completed the installation and started up the application, you should be able to access it at [http://localhost:3000](http://localhost:3000). You can login using the default users, or register a new account.

# Our Team

* Audrey Ford
* John Dobbs
* Anthony Cathers
* Leland Machii
