<html>
  <head>
    <script src="https://aframe.io/releases/1.7.0/aframe.min.js"></script>
  </head>
  <body>
    <a-scene>
      <!-- Pirámide -->
      <a-cone position="-1 0.75 -4" radius-bottom="1" radius-top="0" height="1.5" color="#D65DB1"></a-cone>

      <!-- Anillo -->
      <a-ring position="1 1.5 -5" radius-inner="0.3" radius-outer="0.7" color="#FF6F91" rotation="90 0 0"></a-ring>

      <!-- Caja animada que flota hacia arriba y hacia abajo -->
      <a-box position="0 1 -3" color="#845EC2">
        <a-animation attribute="position" from="0 1 -3" to="0 1.5 -3" direction="alternate" dur="1000" repeat="indefinite"></a-animation>
      </a-box>

      <!-- Suelo -->
      <a-plane position="0 0 -4" rotation="-90 0 0" width="10" height="10" color="#2C73D2"></a-plane>

      <!-- Cielo nocturno con estrellas -->
      <a-sky color="#0D1B2A"></a-sky>
    </a-scene>
  </body>
</html>
