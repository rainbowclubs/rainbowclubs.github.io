# Table of contents

* [About Rainbow Clubs](#about-rainbowclubs)
* [Installation](#installation)
* [Application design](#application-design)
  * [Directory structure](#directory-structure)
  * [Import conventions](#import-conventions)
  * [Naming conventions](#naming-conventions)
  * [Data model](#data-model)
  * [CSS](#css)
  * [Routing](#routing)
  * [Authentication](#authentication)
  * [Authorization](#authorization)
  * [Configuration](#configuration)
  * [Quality Assurance](#quality-assurance)
    * [ESLint](#eslint)
    * [Data model unit tests](#data-model-unit-tests)
    * [JSDoc](#JSDoc)
* [Development history](#development-history)
  * [Milestone 1: Mockup development](#milestone-1-mockup-development)
  * [Milestone 2: Data model development](#milestone-2-data-model-development)
  * [Milestone 3: Connect UI to data model](#milestone-3-connect-ui-to-data-model)
  * [Milestone 4: Authentication](#milestone-4-authentication)
  * [Milestone 5: Administration](#milestone-5-administration)
* [Walkthrough videos](#walkthrough-videos)
* [JSDocs](/jsdocs)

# About Rainbow Clubs

The problem: UH Manoa has over 200 Registered Independent Organizations, plus many more that do not have this “official” status but are nonetheless active organizations. Unfortunately, there is no easy way for students to learn (a) what student clubs (both registered and unregistered) exist, what they do, and how to get further involved.

The solution: The Rainbow Clubs application will provide a centralized directory for UH Manoa student clubs. UH Manoa students can login to browse a well organized directory of all current student clubs, with brief descriptions, meeting times and locations, URLs to their websites (if any), contact information for officers, and a few select photos.

# Approach

Rainbow Clubs has three user roles, all of whom login with their UH ID. Regular users browse the directory. Club Admins have the ability to edit the data associated with their club. Super Admins make sure site content is appropriate and grant “club admin” privileges to selected users.

The site should not simply support browsing by a list of clubs in alphabetical order, but should also allow filtering by interest area. For example, “athletic” clubs, “art” clubs, “music” clubs, etc. A club can belong to multiple interest areas.

Users can specify interest areas, and be notified when a new club is created matching that interest area (or an existing club adds that interest area).

Admins can monitor the site for inappropriate content, and create new categories of musical tastes, capabilities, and goals.

# Use Case Ideas

New user goes to landing page, logs in, gets home page, sets up profile.
Admin goes to landing page, logs in, gets home page, edits site.
User goes to landing page, logs in, looks for clubs of interest.
Club admin goes into site, updates their club profile.

# Advance Features

Upload club data from the CSV version of the RIO spreadsheet.
Notify admins when club data changes so they can review for appropriateness.
Provide “expiration date” for club listings (either one semester or one academic year). To retain a listing, the club admin or admin must login and click a “renew” button for the club to re-list it in the site.
Allow students to rate clubs.

