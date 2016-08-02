# raster-collection
A collection of raster tile service's urlTemplates and subDomains.

[What is urlTemplate and subdomains?](http://leafletjs.com/reference.html#url-template) e.g.

```javascript
'http://{s}.somedomain.com/blabla/{z}/{x}/{y}.png'
```
{s} means one of the available subdomains of the tile service, (used sequentially to help with browser parallel requests per domain limitation), {z} — zoom level, {x} and {y} — tile coordinates.

# World

## openstreetmap.org

* [Open Street Map Standard](http://www.openstreetmap.org) 

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/osm-standard.png)

```javascript
'urlTemplate' : 'http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png',
'subdomains'  : ['a','b','c'],
'attribution' : '&copy; <a href="http://www.osm.org" target="_blank">OpenStreetMap</a> contributors'
```

* [Open Street Map Bicycle](http://www.openstreetmap.org/#layers=C) 

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/osm-cycle.png)

```javascript
'urlTemplate' : 'http://{s}.tile.thunderforest.com/cycle/{z}/{x}/{y}.png',
'subdomains'  : ['a','b','c'],
'attribution' : '&copy; <a href="http://www.osm.org" target="_blank">OpenStreetMap</a> contributors'
```

* [Open Street Map Transport](http://www.openstreetmap.org/#layers=T) 

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/osm-transport.png)
```javascript
'urlTemplate' : 'http://{s}.tile.thunderforest.com/transport/{z}/{x}/{y}.png',
'subdomains'  : ['a','b','c'],
'attribution' : '&copy; <a href="http://www.osm.org" target="_blank">OpenStreetMap</a> contributors'
```

* [Open Street Map Humanitarian](http://www.openstreetmap.org/#layers=H) 

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/osm-human.png)
```javascript
'urlTemplate' : 'http://tile-{s}.openstreetmap.fr/hot/{z}/{x}/{y}.png',
'subdomains'  : ['a','b','c'],
'attribution' : '&copy; <a href="http://www.osm.org" target="_blank">OpenStreetMap</a> contributors'
```

## carto.com

* [Carto.com Light](http://www.carto.com) 

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/carto-light.png)
```javascript
'urlTemplate' : 'http://{s}.basemaps.cartocdn.com/light_all/{z}/{x}/{y}.png',
'subdomains'  : ['a','b','c','d','e'],
'attribution' : '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors, &copy; <a href="https://carto.com/attributions">CARTO</a>'
```

* [Carto.com Light No-Label](http://www.carto.com) 

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/carto-light-nolabel.png)
```javascript
'urlTemplate' : 'http://{s}.basemaps.cartocdn.com/light_nolabels/{z}/{x}/{y}.png',
'subdomains'  : ['a','b','c','d','e'],
'attribution' : '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors, &copy; <a href="https://carto.com/attributions">CARTO</a>'
```

* [Carto.com Dark](http://www.carto.com) 

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/carto-dark.png)
```javascript
'urlTemplate' : 'http://{s}.basemaps.cartocdn.com/dark_all/{z}/{x}/{y}.png',
'subdomains'  : ['a','b','c','d','e'],
'attribution' : '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors, &copy; <a href="https://carto.com/attributions">CARTO</a>'
```

* [Carto.com Dark No-Label](http://www.carto.com) 

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/carto-dark-nolabel.png)
```javascript
'urlTemplate' : 'http://{s}.basemaps.cartocdn.com/dark_nolabels/{z}/{x}/{y}.png',
'subdomains'  : ['a','b','c','d','e'],
'attribution' : '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors, &copy; <a href="https://carto.com/attributions">CARTO</a>'
```

# China

## map.baidu.com (Projection : **baidu**)

* [Baidu Standard](http://map.baidu.com)

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/baidu-standard.png)
```javascript
'urlTemplate' : 'http://online{s}.map.bdimg.com/onlinelabel/?qt=tile&x={x}&y={y}&z={z}&styles=pl&scaler=1&p=1',
'subdomains'  : [0,1,2,3,4,5,6,7,8,9],
'attribution' : '&copy; <a href="http://map.baidu.com/">Baidu</a>'
```

* [Baidu Road](http://map.baidu.com)

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/baidu-road.png)
```javascript
'urlTemplate' : 'http://online{s}.map.bdimg.com/tile/?qt=tile&x={x}&y={y}&z={z}&styles=sl&v=020',
'subdomains'  : [0,1,2,3,4,5,6,7,8,9],
'attribution' : '&copy; <a href="http://map.baidu.com/">Baidu</a>'
```

* [Baidu Satelite](http://map.baidu.com)

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/baidu-sat.png)
```javascript
'urlTemplate' : 'http://shangetu{s}.map.bdimg.com/it/u=x={x};y={y};z={z};v=009;type=sate&fm=46',
'subdomains'  : [0,1,2,3,4,5,6,7,8,9],
'attribution' : '&copy; <a href="http://map.baidu.com/">Baidu</a>'
```

* [Baidu Custom](http://map.baidu.com)

  Baidu Custom's style is decided by customid in URL, screen shots for different customid is as below:

```javascript
'urlTemplate' : 'http://api{s}.map.bdimg.com/customimage/tile?&x={x}&y={y}&z={z}&scale=1&customid={customid}',
'subdomains'  : [0, 1, 2],
'attribution' : '&copy; <a href="http://map.baidu.com/">Baidu</a>'
```

<div>
<table><tbody>
    <tr>
        <td>dark</td>
        <td>midnight</td>
        <td>grayscale</td>
        <td>hardedge</td>
    </tr>
    <tr>
        <td><img src="https://github.com/MapTalks/raster-collection/raw/master/screenshots/bd-c-dark.png"></td>
        <td><img src="https://github.com/MapTalks/raster-collection/raw/master/screenshots/bd-c-midnight.png"></td>
        <td><img src="https://github.com/MapTalks/raster-collection/raw/master/screenshots/bd-c-grayscale.png"></td>
        <td><img src="https://github.com/MapTalks/raster-collection/raw/master/screenshots/bd-c-hardedge.png"></td>
    </tr>
    <tr>        
        <td>light</td>
        <td>redalert</td>
        <td>googlelite</td>
        <td>grassgreen</td>
    </tr>
    <tr>
        <td><img src="https://github.com/MapTalks/raster-collection/raw/master/screenshots/bd-c-light.png"></td>
        <td><img src="https://github.com/MapTalks/raster-collection/raw/master/screenshots/bd-c-redalert.png"></td>
        <td><img src="https://github.com/MapTalks/raster-collection/raw/master/screenshots/bd-c-googlelite.png"></td>
        <td><img src="https://github.com/MapTalks/raster-collection/raw/master/screenshots/bd-c-grassgreen.png"></td>
    </tr>
    <tr>        
        <td>pink</td>
        <td>darkgreen</td>
        <td>bluish</td>
        <td></td>
    </tr>
    <tr>
        <td><img src="https://github.com/MapTalks/raster-collection/raw/master/screenshots/bd-c-pink.png"></td>
        <td><img src="https://github.com/MapTalks/raster-collection/raw/master/screenshots/bd-c-darkgreen.png"></td>
        <td><img src="https://github.com/MapTalks/raster-collection/raw/master/screenshots/bd-c-bluish.png"></td>
        <td></td>
    </tr>
</tbody></table>
</div>


## gaode.com

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

## tianditu

* [Tianditu Standard Mercator](http://www.tianditu.cn)

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/tdt-standard.png)

```javascript
'urlTemplate' : 'http://t{s}.tianditu.com/DataServer?T=vec_w&x={x}&y={y}&l={z}',
'subdomains'  : ['1','2','3','4','5'],
'attribution' : '&copy; <a href="http://www.tianditu.cn/">天地图</a>'
```

* [Tianditu Label Mercator](http://www.tianditu.cn)

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/tdt-label.png)

```javascript
'urlTemplate' : 'http://t{s}.tianditu.com/DataServer?T=cva_w&x={x}&y={y}&l={z}',
'subdomains'  : ['1','2','3','4','5'],
'attribution' : '&copy; <a href="http://www.tianditu.cn/">天地图</a>'
```

* [Tianditu Standard LonLat](http://www.tianditu.cn) (Projection : **EPSG:4326**)

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/tdt-4326-standard.png)

```javascript
'tileSystem' : [1, -1, -180, 90],
'urlTemplate' : 'http://t{s}.tianditu.com/DataServer?T=vec_c&x={x}&y={y}&l={z}',
'subdomains'  : ['1','2','3','4','5'],
'attribution' : '&copy; <a href="http://www.tianditu.cn/">天地图</a>'
```

* [Tianditu Label LonLat](http://www.tianditu.cn) (Projection : **EPSG:4326**)

![image](https://github.com/MapTalks/raster-collection/raw/master/screenshots/tdt-4326-label.png)

```javascript
'tileSystem' : [1, -1, -180, 90],
'urlTemplate' : 'http://t{s}.tianditu.com/DataServer?T=cva_c&x={x}&y={y}&l={z}',
'subdomains'  : ['1','2','3','4','5'],
'attribution' : '&copy; <a href="http://www.tianditu.cn/">天地图</a>'
```
