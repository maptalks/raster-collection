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
'subdomains' : ['a','b','c'],
'attribution' : '&copy; <a href="http://www.osm.org" target="_blank">OpenStreetMap</a> contributors'
```

* [Open Street Map Bicycle](http://www.openstreetmap.org/#layers=C) 

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/osm-cycle.png)
```javascript
'urlTemplate' : 'http://{s}.tile.thunderforest.com/cycle/{z}/{x}/{y}.png',
'subdomains' : ['a','b','c'],
'attribution' : '&copy; <a href="http://www.osm.org" target="_blank">OpenStreetMap</a> contributors'
```

* [Open Street Map Transport](http://www.openstreetmap.org/#layers=T) 

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/osm-transport.png)
```javascript
'urlTemplate' : 'http://{s}.tile.thunderforest.com/transport/{z}/{x}/{y}.png',
'subdomains' : ['a','b','c'],
'attribution' : '&copy; <a href="http://www.osm.org" target="_blank">OpenStreetMap</a> contributors'
```

* [Open Street Map Humanitarian](http://www.openstreetmap.org/#layers=H) 

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/osm-human.png)
```javascript
'urlTemplate' : 'http://tile-{s}.openstreetmap.fr/hot/{z}/{x}/{y}.png',
'subdomains' : ['a','b','c'],
'attribution' : '&copy; <a href="http://www.osm.org" target="_blank">OpenStreetMap</a> contributors'
```

* [Carto.com Light](http://www.carto.com) 

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/carto-light.png)
```javascript
'urlTemplate' : 'http://{s}.basemaps.cartocdn.com/light_all/{z}/{x}/{y}.png',
'subdomains' : ['a','b','c','d','e'],
'attribution' : '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors, &copy; <a href="https://carto.com/attributions">CARTO</a>'
```

* [Carto.com Light No-Label](http://www.carto.com) 

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/carto-light-nolabel.png)
```javascript
'urlTemplate' : 'http://{s}.basemaps.cartocdn.com/light_nolabels/{z}/{x}/{y}.png',
'subdomains' : ['a','b','c','d','e'],
'attribution' : '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors, &copy; <a href="https://carto.com/attributions">CARTO</a>'
```

* [Carto.com Dark](http://www.carto.com) 

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/carto-dark.png)
```javascript
'urlTemplate' : 'http://{s}.basemaps.cartocdn.com/dark_all/{z}/{x}/{y}.png',
'subdomains' : ['a','b','c','d','e'],
'attribution' : '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors, &copy; <a href="https://carto.com/attributions">CARTO</a>'
```

* [Carto.com Dark No-Label](http://www.carto.com) 

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/carto-dark-nolabel.png)
```javascript
'urlTemplate' : 'http://{s}.basemaps.cartocdn.com/dark_nolabels/{z}/{x}/{y}.png',
'subdomains' : ['a','b','c','d','e'],
'attribution' : '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors, &copy; <a href="https://carto.com/attributions">CARTO</a>'
```

#China

* [Gaode Standard](http://www.gaode.com)

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/gaode-standard.png)
```javascript
'urlTemplate' : 'http://webrd{s}.is.autonavi.com/appmaptile?lang=zh_cn&size=1&scale=1&style=8&x={x}&y={y}&z={z}',            
'subdomains'  : ['01','02','03','04'],
'attribution' : '&copy; <a href="http://www.gaode.com/">Gaode.com</a>'
```

* [Gaode Satelite](http://www.gaode.com)

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/gaode-sat.png)
```javascript
'urlTemplate' : 'http://webst{s}.is.autonavi.com/appmaptile?style=6&x={x}&y={y}&z={z}',            
'subdomains'  : ['01','02','03','04'],
'attribution' : '&copy; <a href="http://www.gaode.com/">Gaode.com</a>'
```

* [Gaode Road](http://www.gaode.com)

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/gaode-road.png)
```javascript
'urlTemplate' : 'http://webst{s}.is.autonavi.com/appmaptile?x={x}&y={y}&z={z}&lang=zh_cn&size=1&scale=1&style=8',            
'subdomains'  : ['01','02','03','04'],
'attribution' : '&copy; <a href="http://www.gaode.com/">Gaode.com</a>'
```

* [Tianditu Standard Mercator](http://www.tianditu.cn)

```javascript
'urlTemplate' : 'http://t{s}.tianditu.com/DataServer?T=vec_w&x={x}&y={y}&l={z}',
'subdomains'  : ['1','2','3','4','5'],
'attribution' : '&copy; <a href="http://www.tianditu.cn/">天地图</a>'
```

* [Tianditu Road Mercator](http://www.tianditu.cn)

```javascript
'urlTemplate' : 'http://t{s}.tianditu.com/DataServer?T=cva_w&x={x}&y={y}&l={z}',
'subdomains'  : ['1','2','3','4','5'],
'attribution' : '&copy; <a href="http://www.tianditu.cn/">天地图</a>'
```

* [Tianditu Standard LonLat](http://www.tianditu.cn)

Projection : **EPSG:4326**

```javascript
'urlTemplate' : 'http://t{s}.tianditu.com/DataServer?T=vec_c&x={x}&y={y}&l={z}',
'subdomains'  : ['1','2','3','4','5'],
'attribution' : '&copy; <a href="http://www.tianditu.cn/">天地图</a>'
```

* [Tianditu Road LonLat](http://www.tianditu.cn)

Projection : **EPSG:4326**

```javascript
'urlTemplate' : 'http://t{s}.tianditu.com/DataServer?T=cva_c&x={x}&y={y}&l={z}',
'subdomains'  : ['1','2','3','4','5'],
'attribution' : '&copy; <a href="http://www.tianditu.cn/">天地图</a>'
```