#Forecast Search

Forecast Search is a weather forecast search web application provide an interface to perform weather forecast search and share weather information to Facebook.
 
 This web application has been deployed on **Amazon Web Services(AWS)**: 
 [http://glistenlau.com/forecast/](http://glistenlau.com/forecast/).
 
##How to Setup
You need to extract the zip package, and type the command below to install.

```bash
$ npm install
```

In this website, [The Google Maps Geocoding API](https://developers.google.com/maps/documentation/geocoding/intro), [The Dark Sky Forecast API](https://developer.forecast.io/) and [Facebook SDK for JavaScript](https://developers.facebook.com/docs/javascript/) are used, so developer keys for these three API are required, after got the keys, create a "keys.json" file under the "exclude" folder.

```bash
$ vi ./exclude/keys.json
```

```js
{
  "GOOGLE_KEY": YOUR_GOOGLE_KEY,
  "FORECAST_KEY": YOUR_FORECASTIO_KEY,
  "FACEBOOK_APPID": YOUR_FACEBOOK_APPID
}
```
Run:

```bash
$ node app.js
```
Now Forecast Search is ready on [http://localhost:3000/forecast/](http://localhost:3000/forecast/).

 
##Applied Technology Stacks and APIs

###[Node.js](https://nodejs.org/en/)

The server side was built to provide RESTful web service for web and mobile applications using Node.js, which uses an efficient event-driven, non-blocking I/O model.
###[jQuery](https://jquery.com/)

jQuery was applied on the front-end to validate inputs, manipulate HTML DOM, handle event and Perform Ajax.

###[The Google Maps Geocoding API](https://developers.google.com/maps/documentation/geocoding/intro)

The Google Maps Geocoding API was used to convert addresses (like "1600 Amphitheatre Parkway, Mountain View, CA") into geographic coordinates (like latitude 37.423021 and longitude -122.083739).

###[The Dark Sky Forecast API](https://developer.forecast.io/)

The Dark Sky Forecast API provides the current and future weather infomation for a geoparphic coordinates.

###[Facebook SDK for JavaScript](https://developers.facebook.com/docs/javascript/)

Facebook SDK for JavaScript helps adding Facebook Login and Feed on the client-side.

###[OpenLayers API](http://openlayers.org/) & [OnpenWeatherMap API](http://openlayers.org/)

OpenWeatherMap API provides precipitation and clouds weather map layers, which was used in OpenLayers.

###[Bootstrap](http://getbootstrap.com/)

Bootstrap was applied on front end to build a sleek, intuitive and mobile device friendly website interfaces.

##Demo

###Validation
![](https://googledrive.com/host/0B6oQwX6qlmnZMS0yano1MTg2NWc)
If the user did not enter a street address, city and/or state, then a message will be shown with appropriate text requesting the user to provide the missing information.

###Right Now Tab
![](https://googledrive.com/host/0B6oQwX6qlmnZNnR3WkNVQk5UMlE)
This area is divided into two sections: Current Weather Table and Cloud Map.

#####Current Weather Table
To the left, the current weather data is displayed. The top part consists for two subsections with background color. The left subsection displays the icon image whereas the right subsection displays the "current" weather condition and location, current temperature and High/Low temperature for the day. The table below it displays additional weather data.

#####Cloud Map
To the right, the cloud map is displayed.

###Facebook post
![](https://googledrive.com/host/0B6oQwX6qlmnZa3hBU2V5UW81cDA/)
On click of the Facebook post button, there will be a popup to authorize the user to Facebook if the user is not already logged in to Facebook. And then a feed can be posted.

###Next 24 Hours Tab
![](https://googledrive.com/host/0B6oQwX6qlmnZbWFuRlBIZFZmbnM)
This tab displays the weather information for the next 24 hours.

###Next 7 Days Tab
![](https://googledrive.com/host/0B6oQwX6qlmnZNWRiajhIQVRXc0E)
This tab displays the forecast for the next 7 days. 
If a particular column is clicked, it will display a modal window.

###Response to Devices
![](https://googledrive.com/host/0B6oQwX6qlmnZdmVhVDkzYmpwcms)
If the page is loading on a smart phone or a tablet, the form will bedisplay according to the width of the devices.


