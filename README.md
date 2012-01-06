# Senior Project Proposal

**rifffz**, a music player that's accessible on your web browser

## The Problem

Many desktop focused applications are moving to the web, however media players (think iTunes) have not yet made this shift. With the emergence of the node.js platform, I think that there is an opportunity to bring the experience of browsing and listening to local mp3s to the browser.

I plan to create a lightweight media player web application that users can install on their machine for a (hopefully) visually appealing interface to their music library.

## Outline

### Expected Deliverable

The end product will be made up of file server using the node.js platform and a browser based web client for the front end interface.

### Technology

Here is a list of some specific technology that will be used heavily:

* **javascript** (through coffee-script) -- the programming language
* **html5** -- specifically, the `<audio>` element
* **node.js** -- a platform for "easily building fast, scalable network applications"
* **batman.js** or **backbone.js** -- client side mvc frameworks for a single page highly interactive front end

### Winter Schedule/Milestones

here's my *rough* ideas as to how the work will be split up for the quarter

#### Week 1

* build a prototype (functioning but basic) mp3 server
* design html/css view for listening to an album
* research server design for more efficient streaming of whole albums

#### Week 2

* work on html5 `audio` element with custom controls for controlling playback

#### Weeks 3-4

* start work on database to keep track of file locations and id3 tags in a library for the app
* implement ability to import music to library by adding folders containing songs

#### Weeks 4-5

* design html/css views for adding albums and viewing album library
* research retrieving album artwork from mp3 files and api fallback for retrieving artwork for mp3s that don't have this information yet

#### Weeks 6-7

* implement search functionality for locating specific songs/artists/albums

#### Weeks 8-9

* implement ability to create/listen to playlists

### Spring Schedule/Milestones

I'm hoping to have a much better sense of exact milestones for the Spring by the end of Winter.

## Equipment

No special equipment will be needed--most of the technology that will be used is open-source and freely available.

## Criteria Satisfaction

### Independence

I will be working on this project by myself for my senior project. The web application is the discrete measure of the project's progress. Criteria for success will be met if I have met the goal of establishing a functioning browser based music player. Failure will be the result of not meeting this goal.

### Ownership

The success and failure of this project is solely dependent on me.

### Background Research

When writing this proposal, I discovered [a similar project](http://www.omgubuntu.co.uk/2011/03/html5-browser-based-media-player-plays-your-mp3s-works-offline/) that attempts to solve this problem. It does provide a web based media player for your local files, but it is missing essential functionality like the ability to create playlists and display album artwork, and it isn't taking advantage of the design capabilities that a browser based app can with css (in my opinion). Also, I'm planning to implement a user friendly search feature, which this project is missing. It's definitely a good start at what I'm aiming to achieve with this project though.

There are also addons/extensions for browsers that can interface with desktop media players (windows media player/itunes, etc), but these are meant as plugins that merely control those players.

### Creativity

Currently, there is no application like this that I'm aware of. I am attempting to do something that hasn't done before in a hopefully inventive way.
