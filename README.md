# mdwxessex
Essex, Maryland Weather
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8" />
  <title>Aeris Maps - Visualizer Demo</title>
  
  <!-- Load AerisMaps.Visualizer from a CDN -->
<script type="text/javascript" src="https://cdn.aerisapi.com/js/aerismaps-visualizer.min.js"></script>
</head>
<body>
  <div id="map-canvas"></div>
  
  <script type="text/javascript">
    // See AerisMaps.Visualizer docs at 
    // https://github.com/aerisweather/aerismaps-visualizer
    new AerisMaps.Visualizer('#map-canvas', {
      loc: '39.3003,-76.4594',
      keys: {
        id: 'r1Y73vMUGNnles5c2FJ00',
        secret: 'GTiRSLGaTQeAaHDjSxWSxH7h8T2iw7Ol0J3iVHnR'
      },
      map: {
      zoom: 9,
      size: {
        width: 500,
        height: 500
      },
      layers: ["admin-cities-dk","temperatures-outlook-6-10d-cpc","land-flat","water-flat-dk","temperatures-text"]
      },
      animation: {
        from: 60 * 60 * 2 * -1,  // 2 hours ago
        to: 0
      },
      autoplay: true
    });
  </script>
</body>
</html>
