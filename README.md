# Senior Project Proposal

**rifffz**, a music player that's accessible on your web browser

## The Problem

Many desktop focused applications are moving to the web, however media players (think iTunes) have not yet made this shift. With the emergence of the node.js platform, I think that there is an opportunity to bring the experience of browsing and listening to local mp3s to the browser.

I plan to create a lightweight media player web application that users can install on their machine for a (hopefully) visually appealing interface to their music library.

Some of the advantages of a browser based media player are as follows:

* **lightweight**: users can control their music experience from within their web browser
* **interactive**: by using web technology such as css3 transitions, the player's controls can be enhanced by subtle animations that make for a more enjoyable experience than what's possible with desktop software
* **portable**: as long as the user has node.js installed on their system (cross-platform), none of the back-end or front-end code will have to be re-written to work on different platforms (mac, linux, windows)

## Outline

### Expected Deliverable

The end product will be made up of file server using the node.js platform and a browser based web client for the front end interface.

### Technology

Here is a list of some specific technology that will be used heavily:

* [coffee-script](http://jashkenas.github.com/coffee-script/)
* [css3](http://www.w3.org/TR/2011/WD-css3-text-20110901/) and [html5](http://dev.w3.org/html5/spec/Overview.html)
* [node.js](http://nodejs.org/)
* [batman.js](http://batmanjs.org/) or [backbone.js](http://documentcloud.github.com/backbone/)

Here's a little background as to why I'm looking to use this technology:

Firstly, coffee-script is a language that compiles directly to javascript. It allows for a higher level of abstraction and has a very clean syntax that is easy to read and write for someone who has a background in ruby (me). I've worked with it before, and it is much easier to work with when writing large programs in javascript with extensive use of classes.

By using transitions and other effects that are possible with css3, the player will be able to behave in a way that is natural and visually appealing. The `audio` element from html5 allows web browsers play audio files natively, which is perfect for this project. Users won't have to install any additional plugins to their browser in order to use the player.

Using node.js for the server will give me a nice framework for writing the server. Node.js is a platform for writing realtime networked applications. It also has an extensive filesystem api, which will allow me to access the users' music wherever it is on their machine. It can also be used to read specific information encoded in the mp3 files through ID3 tags. Writing the server using node.js will also allow for asynchronous access to the music, which will be perfect for a single page application.

Batman.js and backbone.js are client side mvc frameworks that are perfect for single page applications. When a user is using the player, he/she will never have to visit different pages to access different functionality. This will make the player seem as interactive as possible and will be more natural for users of desktop media players. The listed frameworks both have extensive apis for handling events in realtime, which will be essential for designing the player functionality.

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
