# Slim Framework for PHP 5

Thank you for choosing Slim, a micro-framework for PHP 5 inspired by [Sinatra](http://sinatrarb.com).

## Features

Slim provides the following notable features out-of-the-box:

* Clean and simple DSL for writing powerful web applications
* RESTful routes (GET, POST, PUT, DELETE)
  * Named routes w/ `urlFor()` helper
  * Route passing
  * Route redirects
  * Route halting
  * Custom 404 and Error handlers
* Easy templating with custom Views (ie. Twig, Smarty, Mustache, ...)
* HTTP Caching
* Session handling
* Logging
* Error handling
* Supports PHP 5+

## "Hello World" application (PHP 5 >= 5.3)

    <?php
    require('slim/Slim.php');
    Slim::init();
    Slim::get('/hello/:name', function ($name) {
        echo "Hello, $name!";
    });
    Slim::run();
    ?>

## "Hello World" application (PHP 5 < 5.3)

    <?php
    require('slim/Slim.php');
    Slim::init();
    Slim::get('/hello/:name', 'hello');
    function hello($name) {
        echo "Hello, $name!";
    }
    Slim::run();
    ?>

## About the Author

Slim is created and maintained by Josh Lockhart, a web developer by day at [New Media Campaigns](http://www.newmediacampaigns.com), and a [hacker by night](http://github.com/codeguy).

Slim is in active development, and test coverage is improving  rapidly as Slim nears its official 1.0 release.

## Links and Resources

* Road Map:       <http://github.com/codeguy/Slim/wiki/Road-Map>
* Documentation:  <http://github.com/codeguy/Slim/wiki/Slim-Framework-Documentation>
* Source Code:    <http://github.com/codeguy/Slim/>
* Twitter:        <http://www.twitter.com/codeguy>
* LinkedIn:       <http://www.linkedin.com/in/joshlockhart>
* Email:          [info@joshlockhart.com](info@joshlockhart.com)

## Open Source License

Slim is released under the MIT public license.

<http://slim.joshlockhart.com/license.txt>