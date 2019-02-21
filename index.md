<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="utf-8">
    <title>gmaps.jsサンプル</title>
    <style type="text/css">
        #map {
            width: 400px;
            height: 400px;
        }
    </style>
</head>
<body>
    <div id="map"></div>
    <script src="//maps.google.com/maps/api/js?sensor=true"></script>
    <script src="//raw.githubusercontent.com/HPNeo/gmaps/master/gmaps.js"></script>
　  <script>
        window.onload = function(){
          var map = new GMaps({
              div: "#map",//id名
              lat: 35.170694,//緯度
              lng: 136.88163699999995,//経度
              zoom: 14//縮尺
          });
        };
   </script>
</body>
</html>
