# raster-collection
A collection of raster tile service's urlTemplates and subDomains.

What is urlTemplate and subdomains? e.g.

```javascript
'http://{s}.somedomain.com/blabla/{z}/{x}/{y}.png'
```
{s} means one of the available subdomains of the tile service, (used sequentially to help with browser parallel requests per domain limitation), {z} — zoom level, {x} and {y} — tile coordinates.

# World
* [Open Street Map Default Style](http://www.openstreetmap.org) 
```javascript
'urlTemplate' : 'http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png',
'subdomains' : ['a','b','c']
```
