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
    <script src="gmaps.js"></script>
    <script>
        window.onload = function(){
            var lat = 35.170694;//緯度
            var lng = 136.88163699999995;//経度
            var map = new GMaps({
                div: "#map",//id名
                lat: lat,
                lng: lng,
                zoom: 14//縮尺
            });
            map.addMarker({
                lat: lat,
                lng: lng,
                title: "名古屋駅",
                icon: "finger.png",//任意の画像名
                infoWindow: {
                    content: "<p>名古屋駅へようこそ</p>"
                }
            });
        };
    </script>
</body>
</html>
