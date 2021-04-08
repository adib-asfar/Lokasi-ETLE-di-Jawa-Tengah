<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8" />
    <title>Display a map</title>
    <meta name="viewport" content="initial-scale=1,maximum-scale=1,user-scalable=no" />
    <script src="https://api.mapbox.com/mapbox-gl-js/v1.12.0/mapbox-gl.js"></script>
    <link href="https://api.mapbox.com/mapbox-gl-js/v1.12.0/mapbox-gl.css" rel="stylesheet" />
    <style>
        body {
            margin: 0;
            padding: 0;
        }

        #map {
            height: 80vh;
            width: 80%;
            left: 5rem;
        }

        h1 {

            padding-left: 5rem;
            color: red;
        }
    </style>
</head>

<body>
    <h1>Lokasi ETLE di Jawa Tengah</h1>

    <div id="map"></div>
    <script>
        mapboxgl.accessToken =
            'pk.eyJ1IjoiYWRpYm1hc2ZhciIsImEiOiJja2hwdnZkc3kxZXY3MzhteGdkM2hoYjA0In0.D5p4SAmaOvQBfVf6pfo3sw';
        var map = new mapboxgl.Map({
            container: 'map', // container id
            style: 'mapbox://styles/adibmasfar/ckn8bncpc1ato17qxj0sroczc', // style URL
            center: [110.249, -7.307], // starting position [lng, lat]
            zoom: 16, // starting zoom
            pitch: 200,

        });
    </script>

</body>

</html>
