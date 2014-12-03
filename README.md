meetup-element
============

This is a test run of creating a custom element from the [Polymer Seed Element](http://polymerlabs.github.io/seed-element).

## Usage
All dependencies are currently managed through Bower. To get started, simply fork the project into your own repository, clone it to your local machine,
clone the project, then run:

```
bower install

```
**NOTE** The .bowerrc file will route all bower dependencies the directory immediately outside (i.e. one level above) of the development directory. This is because all imports of external dependencies are prefixed with "../".

Because of this, we recommend keeping a parent directory for the project that itself includes the development directory. For example:

-- MeetupElement
------ meetup-element (the files in this repo)
------ polymer
------ webcomponentsjs
------ .....[another dependency].....

## Demo

http://dev.gdgtc.com/webcomponents/meetup-element/demo.html
