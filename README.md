Tangram: WebGL for OpenStreetMap
===

Tangram is a library for dynamic client-side map rendering with WebGL (with a less-maintained Canvas option), using GeoJSON or binary vector tiles.

## Vector Tiles

Instead of using traditional image tiles, we render from **vector tiles** that contain the underlying source geometry for each tile's bounding box.

Mapzen provides a free [vector tile service](http://mapzen.com/vector/) that can be used with Tangram for OpenStreetMap base layer data, with worldwide coverage updated daily. There is also an [OSM.US-hosted](http://openstreetmap.us/~migurski/vector-datasource/) alternative.

Tangram currently supports GeoJSON tiles as well as [Mapbox's binary format](https://github.com/mapbox/vector-tile-spec), both of which can be generated by the [Mapzen vector tile service](http://mapzen.com/vector/).

Here's an [example GeoJSON tile](http://vector.mapzen.com/osm/all/14/4826/6161.json).

The library also includes a [Leaflet](http://leafletjs.com) plugin, `Tangram.LeafletLayer`, to provide basic web map pan/zoom functionality.

## Installation

```
npm install
make
```

The library will be minified in `dist/`, and `index.html` provides an example for rendering from different sources and simple Leaflet integration.

## Examples

- [**NYC / Lower Manhattan**](http://vector.io/vector-map/#mapzen,40.70479834544056,-74.0057945251465,15)
- [**NYC / Central Park**](http://vector.io/vector-map/#mapzen,40.78004586258099,-73.96652698516847,16)
- [**Berlin**](http://vector.io/vector-map/#mapzen,52.52177659937554,13.373343944549562,16)
- [**Colosseum & Roman ruins**](http://vector.io/vector-map/#mapzen,41.889367479706124,12.488912343978884,17)
