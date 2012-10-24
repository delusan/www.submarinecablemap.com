
Submarine Cable Map
===================

[![Submarine Cable Map](http://26.media.tumblr.com/tumblr_lru2g8MJaV1qcsswzo1_500.png)](http://www.submarinecablemap.com)

[TeleGeography's](http://www.telegeography.com) submarine cable map is based on our authoritative [Global Bandwidth](http://www.telegeography.com/research-services/global-bandwidth-research-service/) research and depicts international active and planned submarine cable systems and their landing stations. The map presents data about each cable, including landing points, owners, length, ready-for-service (RFS) date, and website. Try it today! Visit [http://www.submarinecablemap.com](http://www.submarinecablemap.com).


Installation
------------

    $ git clone git://github.com/telegeography/www.submarinecablemap.com.git

Point your webserver's document root to the public directory and that's it.


Updates
-------

To make sure you get any updates, just watch this repository and perform a pull when you see any new commits:

    $ cd www.submarinecablemap.com
    $ git pull


How did you make the Submarine Cable Map?
-------------------------------

[TeleGeography](http://www.telegeography.com) draws the cable routes and plots the landing points with [Adobe Illustrator](http://www.adobe.com/products/illustrator.html). Using [Avenza's MAPublisher](http://www.avenza.com/mapublisher) plug-in, which works with Illustrator, two sets of data are exported as KML files: the cable routes (as MultiLineStrings) and landing points (as Points). These KML files are then parsed to create CSV files that are uploaded to Google Fusion Tables.

We use [Google's Maps API v3.](http://code.google.com/apis/maps/documentation/javascript/) to transform the [Google Fusion Tables](http://www.google.com/fusiontables) into two separate map layers of cable routes and landing points. The interactivity on the map is driven by javascript and was written in-house at TeleGeography.


How can I download the KML or a CSV of the dataset?
--------------------------------------------------

Below are links to both of the datasets used for the [http://www.submarinecablemap.com](Submarine Cable Map).

__Submarine Cables:__

[https://www.google.com/fusiontables/DataSource?docid=1BVxUz5t3qDmHJApb6FVckR5mJDOn_xYFocOKWnA](https://www.google.com/fusiontables/DataSource?docid=1BVxUz5t3qDmHJApb6FVckR5mJDOn_xYFocOKWnA)

__Landing points:__

[https://www.google.com/fusiontables/DataSource?docid=1viJdQy7bRfdGlFuVAEYLrTQ7TClIwtPKCdcpCYY](https://www.google.com/fusiontables/DataSource?docid=1viJdQy7bRfdGlFuVAEYLrTQ7TClIwtPKCdcpCYY)


__To download as KML try the following steps:__

1. Click 'Visualize' then select 'Map'.
2. Then click the 'Download KML' link available above the map.

__Note:__ For landing points, modify the 'Location' dropdown menu to 'coordinates' from 'name', then click 'Download KML' to get the landing point data.


Questions? Corrections?
------------------------

[cablemap@telegeography.com](mailto:cablemap@telegeography.com)
