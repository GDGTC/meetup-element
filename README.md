meetup-element
============

This is a test run of creating a custom element from the [Polymer Seed Element](http://polymerlabs.github.io/seed-element).

This repo may well be broken up into separate repos at some point, but right now it consists of three components: meetup-element, meetup-card, and meetup-service.

The meetup-element is declared with the type of data that it wants to retrieve. It then
it calls the meetup-service, which then populates a page of meetup-cards.


## Setup
All dependencies are currently managed through Bower. To get started, simply fork the project into your own repository, clone it to your local machine,
clone the project, then run:

```
bower install

```
**NOTE** The .bowerrc file will route all bower dependencies the directory immediately outside (i.e. one level above) of the development directory. This is because all imports of external dependencies are prefixed with "../".

Because of this, we recommend keeping a parent directory for the project that itself includes the development directory. For example:

--> MeetupElement  
------> meetup-element (the files in this repo)  
------> polymer  
------> webcomponentsjs  
------> .....[another dependency].....

## Usage

As of now, meetup-element takes the following attributes as configuration options:

- urlName (required): The path to a meetup group from meetup.com, no slashes
    - e.g: "gdg-tc"
- sig (required): Meetup API key
- sigid (required): Meetup API key
- dataFormat (required): The type of data to be retreived (see options below)
- limit (optional): The number of data items to fetch. Used when retreiving a list.
    - default: undefined

**dataFormat Options**
- upcoming-meetups: Tells meetup-element to fetch a list of upcoming meetups
- past-meetups: Tells meetup-element to fetch a list of past-meetups

## Demo

http://dev.gdgtc.com/webcomponents/meetup-element/demo.html
