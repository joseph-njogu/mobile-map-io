# mobile-map-io

![Screenshot of report screen](https://andyhub.com/wordpress/wp-content/uploads/mobilemapio-square-350x350.png)

This is a boilerplate mobile hybrid app for I/O with maps. The idea is that many civic apps have to do with reporting things as people see them. That means people are **mobile**, they're talking about things that are **map**pable, and they're reporting those things and getting those reports **(I/O)**. These were the three key things that drove this project, in addition to the frequent reinvention of this sort of generic app infrastructure ad-hoc.

Now, if you want to make an app for your neighbors to report broken streetlights, fork this repo. If you want to make an app for your community to report code violations, fork this repo. If you want to make an app to post all your favorite resturants, fork this repo. You can do all those things out of the box. If you want to make this into something slightly different, like a [system that connects businesses and hungry people](https://github.com/werdnanoslen/mobile-map-io), follow these instructions to start developing:

1. Install [npm](https://www.npmjs.com/get-npm), [mysql](https://mariadb.org/download/), and [a web server](https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-14-04#step-1-install-apache)
1. Run ```npm install```
1. Run ```bower install```
1. Copy .env.example to just .env and add your secret keys/config
1. Import api/reports.sql ```mysql -u[username] -p[password] -h[hostname] [database] < api/reports.sql```
1. Update ionic.config.json ```proxyUrl``` variable to point to your API (ignore if using defaults)
1. Run ```sudo npm start``` to run server
1. Run ```ionic serve``` to run app
1. Build app for android ```ionic build android```, usually saving to ```platforms/android/build/outputs/apk/android-debug.apk```
1. Check out the [CONTRIBUTING.md](https://github.com/werdnanoslen/mobile-map-io/blob/master/CONTRIBUTING.md) file for how to contribute back

### This project
This software is licensed to Andrew Nelson, see the LICENSE file. If you would like an exception to this license for commercial/proprietary derivative work, please email me.
