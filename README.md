# raster-collection
A collection of raster tile service's urlTemplates and subDomains.

[What is urlTemplate and subdomains?](http://leafletjs.com/reference.html#url-template) e.g.

```javascript
'http://{s}.somedomain.com/blabla/{z}/{x}/{y}.png'
```
{s} means one of the available subdomains of the tile service, (used sequentially to help with browser parallel requests per domain limitation), {z} — zoom level, {x} and {y} — tile coordinates.

# World
* [Open Street Map Standard](http://www.openstreetmap.org) 
![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/osm-standard.png)
```javascript
'urlTemplate' : 'http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png',
'subdomains' : ['a','b','c']
```

* [Open Street Map Bike](http://www.openstreetmap.org/#layers=C) 
![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/osm-bike.png)
```javascript
'urlTemplate' : 'http://{s}.tile.thunderforest.com/cycle/{z}/{x}/{y}.png',
'subdomains' : ['a','b','c']
```