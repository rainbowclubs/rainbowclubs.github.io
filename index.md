---
title: Rainbow Clubs
---

# Table of contents

* [About Rainbow Clubs](#about-rainbow-clubs)
* [Approach](#approach)
* [Use Case Ideas](#use-case-ideas)
* [Advanced Features](#advanced-features)
* [Our Team](#our-team)

# About Rainbow Clubs

* [Live Demo](http://rainbowclubs.meteorapp.com)
* [Project Board](https://github.com/rainbowclubs/rainbowclubs/projects/1)
* [Github Repository](https://github.com/rainbowclubs/rainbowclubs)

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

* Landing Page

This is the main page that users will be directed to.  The goal of this page is to describe the function of the website as a whole.  Normal users and admin users will have different landing pages and tabs however the admin user currently does not have any different functions yet.
![landing page](https://github.com/rainbowclubs/rainbowclubs.github.io/blob/master/images/landing.png?raw=true)

* Sign in/up Page

These are the pages that users will be able to either sign in or register for an account.  These pages will store and pull the account information from a mongoDB.
![Sign in page](https://github.com/rainbowclubs/rainbowclubs.github.io/blob/master/images/signin.png?raw=true)
![Sign up page](https://github.com/rainbowclubs/rainbowclubs.github.io/blob/master/images/signup.png?raw=true)

* Listing Page

The purpose of this page is to list all registered RIOs and clubs in the UH database.  Each club will have a card that will contain a description, tags, a link to the RIO/club website (if they have one), and a link to a seperate page that will have further descriptions of the RIO/club.
![Listing page](https://github.com/rainbowclubs/rainbowclubs.github.io/blob/master/images/listing.png?raw=true)

# Our Team

* Audrey Ford
* John Dobbs
* Anthony Cathers
* Leland Machii
