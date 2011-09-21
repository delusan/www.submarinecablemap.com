
Submarine Cable Map
===================

[![Submarine Cable Map](http://www.telegeography.com/assets/website/images/icons/interactive-cable-map.jpg)](http://www.submarinecablemap.com)

TeleGeography's online map is based on our authoritative [Global Bandwidth](http://www.telegeography.com/research-services/global-bandwidth-research-service/) research and depicts international active and planned submarine cable systems and their landing stations. The map presents data about each cable, including landing points, owners, length, ready-for-service (RFS) date, and website. Try it today! Visit [http://www.submarinecablemap.com](http://www.submarinecablemap.com).


Installation
------------

    $ git clone git://github.com/telegeography/www.submarinecablemap.com.git

Point your webserver's document root to the public directory and that's it.


Updates
-------

To make sure you get any updates, just watch this repository and perform a pull when you see any new commits:

    $ cd www.submarinecablemap.com
    $ git pull


How did you make the Cable Map?
-------------------------------

[TeleGeography](http://www.telegeography.com) draws the cable routes and plots the landing points with [Adobe Illustrator](http://www.adobe.com/products/illustrator.html). Using [Avenza's MAPublisher](http://www.avenza.com/mapublisher) plug-in, which works with Illustrator, two sets of data are exported as KML files: the cable routes (as MultiLineStrings) and landing points (as Points). These KML files are then parsed to create CSV files that are uploaded to Google Fusion Tables.

We use [Google's Maps API v3.](http://code.google.com/apis/maps/documentation/javascript/) to transform the [Google Fusion Tables](http://www.google.com/fusiontables) into two separate map layers of cable routes and landing points. The interactivity on the map is driven by javascript and was written in-house at TeleGeography.

Questions? Corrections?
------------------------

[cablemap@telgeography.com](mailto:cablemap@telgeography.com)