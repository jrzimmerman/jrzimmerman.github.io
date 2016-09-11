---
title: Geolocation on Page Load
slug: geolocation-on-page-load
date_published: 2015-11-12T08:19:00.000Z
date_updated:   2016-06-13T07:18:58.000Z
---

While building [Geotinerary](https://geotinerary.herokuapp.com/), I wanted the map to zoom relatively close to the users location. Surprisingly enough, this was quite hard to find an example of.

#### HTML5 and IPs
Traditionally, when a webpage wants your location, we use the native HTML5. While this isn't a terrible idea and can have much more accurate results, there is another method to find your users location that doesn't require the use of HTML5 geolocation, the users IP address.


#### HTML5 Geolocation

The most accurate approach to locating your users is to use HTML 5's built in geolocation feature. Due to the accuracy, this is the approach I opted to use for Geotinerary.

Here is a code snippet for HTML 5 Geolocation:

<script src="https://gist.github.com/jrzimmerman/c4039796cfaa84980cbe.js"></script>

#### Geolocating IP Addresses

If you are concerned with There are a swath of many great GeoIP providers, but for this project I decided upon [Free GeoIP](http://freegeoip.net/) for its open data and ease of use. While the location is not as great, it's all about what you need from your data.

Here is a code snippet for Geolocating IP Addresses:

<script src="https://gist.github.com/jrzimmerman/0453bdfd552de42f30f6.js"></script>

Deciding upon which method to use depends on use case. Since I had a need for specific locations, I went with the traditional HTML 5 geolocation. If I were to aggregate data at a national (or global) scale, then GeoIP is a fantastic use.

