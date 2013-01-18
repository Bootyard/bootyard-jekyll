# Bootyard Flavored Jekyll #

How to install
------

    git clone https://github.com/Bootyard/bootyard-jekyll

Compiling Haml to HTML

------
In the terminal, type in this command:

    rake preview

You may need to repeat this command when editing haml pages in _layouts/haml and _includes/haml.

Running Server
------
Open an new tab in terminal and type in this command:

    jekyll --server --auto

Then visit http://localhost:4000 in your server.

Adding JS and Sass on Assets
------
On _assets.yaml, specify your JS and Sass files.
Sample _assets.yaml file:

    javascript_compressor: closure

    javascripts:
      application:
        - assets/js/app.js
        - assets/js/foundation.js
        - assets/js/jquery.js
    stylesheets:
      screen:
        - assets/css/app.css
        - assets/css/foundation.css



Notes
------
* This uses foundation as front-end framework
* Uses sass, haml & javascript (and installed jquery as default)


To do
------
* Add a rake command to choose foundation or boostrap as front-end framework

Based from
------
* https://github.com/groovemonkey/jekyll-foundation-base
* http://mikeferrier.com/2011/04/29/blogging-with-jekyll-haml-sass-and-jammit/