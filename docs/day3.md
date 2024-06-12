# 🍁 June 12

<hr>

## ☕ Coffee
_9:00 - 10:00 am_ 

<hr>

## 🍃 Hello Leaflet
_10:00 am - 12:00 pm_ 

- [How to Use Glitch](https://help.glitch.com/hc/en-us/sections/16285895402765-Getting-Started)
- [Hello Leaflet!](https://hexagonal-sapphire-dress.glitch.me/)
- [Hello Leaflet! Code](https://glitch.com/edit/#!/hexagonal-sapphire-dress)
    - [HyperText Markup Language (HTML) -- index.html](https://developer.mozilla.org/en-US/docs/Web/HTML) essentials
    - [JavaScript -- script.js](https://developer.mozilla.org/en-US/docs/Web/JavaScript) 
    - [Debugging with Browser Console](https://firefox-source-docs.mozilla.org/devtools-user/browser_console/index.html)
    
    
<hr>

## 😋 Lunch

<hr>

## 🌐 Minimal Maps 
_1:30 - 3:00 pm_ 

- [Make a Web Map with Leaflet](https://blog.glitch.com/post/make-a-web-map-with-leaflet)
- [CSS -- style.css](https://developer.mozilla.org/en-US/docs/Web/CSS)
- Loading data into your map (CSV, [GeoJSON](https://leafletjs.com/examples/geojson/))

1. Download a CSV file from [here](https://github.com/AccessibilityMapping/AMP/tree/master/Data)
2. Change the 'x' and 'y' column to 'lat' and 'long'
3. Convert the CSV to geoJSON using [geojson.io](http://geojson.io)
4. Copy the geoJSON data into the script below

```js
let map = L.map('map').setView([39.952, -75.1932], 18); 
L.tileLayer(
  "https://tile.openstreetmap.org/{z}/{x}/{y}.png" 
).addTo(map);

let data = <paste date here>

L.geoJSON(data, {
  onEachFeature: function (feature, layer) {
    layer.bindPopup('<h1>'+feature.properties["Building name"] + '</h1>');
  }
}).addTo(map);
```

- [Leaflet Overpass Layer](https://github.com/GuillaumeAmat/leaflet-overpass-layer)
- [Demo](https://stackblitz.com/edit/leaflet-overpass-layer-demo?file=index.js)

<hr>

## ☕ Coffee Break

<hr>

## 🍭 Customizing Your Map
_3:30 pm - 5:00 pm_ 


- [Markers](https://leafletjs.com/examples/custom-icons/)
- [Tooltips](https://leafletjs.com/reference.html#tooltip)
- [Popups](https://leafletjs.com/reference.html#popup)


- [Map base layers](https://leaflet-extras.github.io/leaflet-providers/preview/), [more info here](https://github.com/leaflet-extras/leaflet-providers)
- [Panes](https://leafletjs.com/examples/map-panes/)
- [Historical Basemaps](https://github.com/aourednik/historical-basemaps)
- [Georectifying historical maps](https://www.davidrumsey.com/view/georeferencer)
- [MapWarper](https://mapwarper.net/)

<hr>

## 🏞️ Happy Hour
_5:15 - 7:00 pm_ 
