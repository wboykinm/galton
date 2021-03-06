# isochrone

Build isochrone using source point and options

**Parameters**

-   `point` **[Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array).&lt;float>** source point [lng, lat]
-   `options` **isochroneOptions** object

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)** promise with GeoJSON when resolved

# isochroneOptions

Isochrone options

**Properties**

-   `osrm` **[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)** node-osrm instance
-   `bufferSize` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** buffer size
-   `cellWidth` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** cellWidth as in
    [turf-point-grid](https://github.com/Turfjs/turf-point-grid)
-   `intervals` **[Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array).&lt;[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)>** intervals for isochrones in minutes
-   `concavity` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** relative measure of concavity as in
    [concaveman](https://github.com/mapbox/concaveman)
-   `lengthThreshold` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** length threshold as in
    [concaveman](https://github.com/mapbox/concaveman)
-   `resolution` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** turf-bezier time in milliseconds between points as in
    [turf-bezier](https://github.com/Turfjs/turf-bezier)
-   `sharpness` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** a measure of how curvy the path should be between splines as in
    [turf-bezier](https://github.com/Turfjs/turf-bezier)
-   `units` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** either `kilometers` or `miles` as in
    [turf-point-grid](https://github.com/Turfjs/turf-point-grid)

# server

Isochrone server

**Parameters**

-   `config` **serverConfig** default isochrone options

Returns **Koa** Koa instance

# serverConfig

Server configuration

**Properties**

-   `osrmPath` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** path to \*.osrm file
-   `bufferSize` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** buffer size
-   `cellWidth` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** cellWidth as in
    [turf-point-grid](https://github.com/Turfjs/turf-point-grid)
-   `intervals` **[Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array).&lt;[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)>** intervals for isochrones in minutes
-   `concavity` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** relative measure of concavity as in
    [concaveman](https://github.com/mapbox/concaveman)
-   `lengthThreshold` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** length threshold as in
    [concaveman](https://github.com/mapbox/concaveman)
-   `resolution` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** turf-bezier time in milliseconds between points as in
    [turf-bezier](https://github.com/Turfjs/turf-bezier)
-   `sharpness` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** a measure of how curvy the path should be between splines as in
    [turf-bezier](https://github.com/Turfjs/turf-bezier)
-   `units` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** either `kilometers` or `miles` as in
    [turf-point-grid](https://github.com/Turfjs/turf-point-grid)
