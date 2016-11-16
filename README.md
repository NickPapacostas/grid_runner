Grid Runner
===========

A command line tool for running Grid microservices:

Install
-------

``` gem install grid_runner ```


Requirements
------------

grid_runner uses a Procfile at the root of your project similar to [Foreman](https://github.com/ddollar/foreman)


Commands
--------

* ``` grid_runner list ```
* ``` grid_runner run <APP_NAME || 'all' >  ```
* ``` grid_runner kill <APP_NAME || 'all' >  ```
* ``` grid_runner restart <APP_NAME || 'all' >  ```
* ``` grid_runner running ```
* ``` grid_runner not_running ```

All commands that take an app name can take a space delimited list of app names:

e.g.
``` gr log media-api cropper thrall ```

Logs
----

Currently grid_runner will put all logs in ./logs/APPNAME.log

* To watch all logs I use ``` tail -f logs/* ```

Other
-----

I added "alias gr=grid_runner" to my .bash\_profile

e.g.

* ``` gr run all ```
* ``` gr list ```


Troubleshooting:
----------------

*** warning ***

run:
``` gem uninstall grid_runner ```
``` gem install grid_runner -v 0.1.0 ```

not sure what i did to rubygems to bork this. but it was borked for me ^_^

