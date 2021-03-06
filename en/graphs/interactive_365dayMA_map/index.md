
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
  <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
  <meta http-equiv="Content-Style-Type" content="text/css" />
  <meta name="generator" content="pandoc" />
  <title></title>
  <style type="text/css">code{white-space: pre;}</style>
</head>
<body>
<h1 id="entrance-page">365-day moving averages temperatures interactive map</h1>
<p><strong>PÁGINA EN MANTENIMIENTO</strong></p>
<p>In this page you will find an interactive map with numerous climate data locations.</p>
<p>If you click on each marker, it'll open a popup with interesting graphs about climate evolution on that specific location. </p>
<p>Left hand graphs are 365-day moving averages temperatures while right hand graphs are the anomalies between each moving average temperature and the mean of all 365-day moving average temperatures .</p>
<p>You can close the popup either clicking on the right-hand top cross or just clicking anywhere on the map. </p>
<p class="powered-by">
    &copy; 2020 Alejandro Rodríguez Sánchez. All rights reserved. &middot; 
</p>
<p>Last updated: 24-oct-2020</p>
  
<!-- AddToAny BEGIN -->
<div class="a2a_kit a2a_kit_size_32 a2a_default_style" data-a2a-url="https://alexrsanchez.github.io/en/graphs/interactive_365dayMA_map/" data-a2a-title="365-day moving average temperatures">
<a class="a2a_dd" href="https://www.addtoany.com/share"></a>
<a class="a2a_button_twitter"></a>
<a class="a2a_button_facebook"></a>
<a class="a2a_button_linkedin"></a>
<a class="a2a_button_email"></a>
</div>
<script async src="https://static.addtoany.com/menu/page.js"></script>
<!-- AddToAny END -->
  
</body>

<head>
        <meta charset="utf-8">
        <title>Mapa de prueba. Alejandro Rodríguez Sánchez</title>
        
<link rel="stylesheet" href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css"
   integrity="sha512-xodZBNTC5n17Xt2atTPuE1HxjVMSvLVW9ocqUKLsCC5CXdbqCmblAshOMAS6/keqq/sMZMZ19scR4PsZChSR7A=="
   crossorigin=""/>
   
<!-- Make sure you put this AFTER Leaflet's CSS -->
 <script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js"
   integrity="sha512-XQoYMqMTK8LvdxXYG3nZ448hOEQiglfqkJs1NOQV44cWnUrBc8PkAOcXy20w0vlaXaVUearIOBhiXZ5V3ynxwA=="
   crossorigin=""></script>
   
</script>
        <style>
          html {
            width: 100%;
            height: 100%;
          }
          body {
            width: 90%;
            height: 100%;
            margin: 10px;
          }
          #map {
           width: 960px;
           height:500px;
          }
        </style>
    </head>
<body>

    <div id="map"></div>

<script>

    var map = L.map('map',{
    center: [40.416829, -3.7035935],
    zoom: 10
    });

    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
    }).addTo(map);
  
    var marker = L.marker([40.416829, -3.7035935]).bindPopup('Puerta del Sol. Km 0').addTo(map);
    
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/alexrsanchez.github.io/main/es/graphs/interactive_maps_tests/images/Temperaturasmoviles365yanomalias_Campillos.png";
    var marker = L.marker([37.0490398, -4.8825273]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Adamuz.png";
    var marker = L.marker([37.99823, -4.4466269]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Adra.png";
    var marker = L.marker([36.7473572, -2.9934895]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Aguilas.png";
    var marker = L.marker([37.4186559, -1.5922917]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Alcaudete.png";
    var marker = L.marker([37.5772754, -4.0784157]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Almeria.png";
    var marker = L.marker([36.8354149, -2.4026462]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Aroche.png";
    var marker = L.marker([37.95807696, -6.94499151]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Baena.png";
    var marker = L.marker([37.6916526, -4.3061329]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_BasurtaJerez.png";
    var marker = L.marker([36.75706775, -6.0172463]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Baza.png";
    var marker = L.marker([37.5645067, -2.7678333]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Belmez.png";
    var marker = L.marker([38.254392, -5.2096614]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
    
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Beniel.png";
    var marker = L.marker([38.0344358, -0.9998293]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Cadiar.png";
    var marker = L.marker([36.9231625, -3.1841055]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Cartama.png";
    var marker = L.marker([36.7169, -4.6783312]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Caudete.png";
    var marker = L.marker([38.7347431, -0.9799931]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_CharcodeTaray.png";
    var marker = L.marker([38.1610173, -1.1528781]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_ChiclanadeSegura.png";
    var marker = L.marker([38.3028651, -2.9965352]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Churriana.png";
    var marker = L.marker([36.6737823, -4.503177]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Cordoba.png";
    var marker = L.marker([37.8569095, -4.8028768]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_CuevasdeAlmanzora.png";
    var marker = L.marker([37.3890757, -1.7705019]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_ElCampillo.png";
    var marker = L.marker([37.66098933, -6.59927192]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
    
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_ElCarpio.png";
    var marker = L.marker([37.9139388, -4.5041648]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
    
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Estepona.png";
    var marker = L.marker([36.4446994, -5.2099127]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
    
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_FincaTaray.png";
    var marker = L.marker([38.0069893, -1.30254717]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
    
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Fiñana.png";
    var marker = L.marker([37.15671804, -2.83882767]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
    
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_FuenteAlamo.png";
    var marker = L.marker([37.74824134, -1.12925196]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
    
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Gibraleon.png";
    var marker = L.marker([37.41235429, -7.05984095]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
    
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Hornachuelos.png";
    var marker = L.marker([37.71986103, -5.16011561]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
    
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Huercal-Overa.png";
    var marker = L.marker([37.41242763, -1.88428316]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
    
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Huesa.png";
    var marker = L.marker([37.74739173, -3.06167021]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);

    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Iznalloz.png";
    var marker = L.marker([37.41640639, -3.55145914]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Jerez.png";
    var marker = L.marker([36.64272178, -6.0134027]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_JerezdelMarquesado.png";
    var marker = L.marker([37.19053597, -3.14986436]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);

    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_JimenadelaFrontera.png";
    var marker = L.marker([36.41364898, -5.38379992]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_LaAljorra.png";
    var marker = L.marker([37.6766591, -1.06290601]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_LaHigueradeArjona.png";
    var marker = L.marker([37.94877184, -4.00771137]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_LaLuisiana.png";
    var marker = L.marker([37,52511272, -5.22813537]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_LaMojonera.png";
    var marker = L.marker([36.78731768, -2.70438243]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_LaPuebladeGuzman.png";
    var marker = L.marker([37.55217633, -7.24836548]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_LaPuebladelRio.png";
    var marker = L.marker([37.08017447, -6.04656909]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_LasCabezasdeSanJuan.png";
    var marker = L.marker([37.01555974, -5.88472195]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Loja.png";
    var marker = L.marker([37.16929992, -4.13812795]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_LoradelRio.png";
    var marker = L.marker([37.66090609, -5.54070374]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Lorca.png";
    var marker = L.marker([37.60172439, -1.62945522]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Malaga.png";
    var marker = L.marker([36.7565627, -4.53770948]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_ManchaReal.png";
    var marker = L.marker([37.91642523, -3.59648044]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_MonterrubiodelaSerena.png";
    var marker = L.marker([38.59158204, -5.38361342]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Moratalla.png";
    var marker = L.marker([38.19665256, -1.81318598]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Niebla.png";
    var marker = L.marker([37.34712492, -6.73534784]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Olivenza.png";
    var marker = L.marker([38.72092072, -7.05782506]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Ontur.png";
    var marker = L.marker([38.62286562, -1.49576881]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Osuna.png";
    var marker = L.marker([37.25502961, -5.13483774]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Padul.png";
    var marker = L.marker([37.0187427, -3.60031696]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_PilardelaHoradada.png";
    var marker = L.marker([37.86858793, -0.81252839]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Pizarra.png";
    var marker = L.marker([36.76666516, -4.71518482]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_PuebladeDonFabrique.png";
    var marker = L.marker([37.87611505, -2.38171756]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_PuertoLumbreras.png";
    var marker = L.marker([37.50376296, -1.69387844]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Sabiote.png";
    var marker = L.marker([38.07948243, -3.23550058]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_SanJosedelosPropios.png";
    var marker = L.marker([37.85795493, -3.23029231]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_SanlucarLaMayor.png";
    var marker = L.marker([37.42179036, -6.25507492]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Santaella.png";
    var marker = L.marker([37.52243056, -4.88550616]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_SierradeYeguas.png";
    var marker = L.marker([37.1250513, -4.8680497]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Tabernas.png";
    var marker = L.marker([37.09131542, -2.30237549]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Torreblascopedro.png";
    var marker = L.marker([37.98874154, -3.68933067]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
   
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Totana.png";
    var marker = L.marker([37.73244087, -1.5131051]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
    
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Turilla.png";
    var marker = L.marker([37.85557972, -1.8177666]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Ubeda.png";
    var marker = L.marker([37.9428797, -3.30047066]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_VejerdelaFrontera.png";
    var marker = L.marker([36.28506429, -5.84003732]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_VelezMalaga.png";
    var marker = L.marker([36.79609353, -4.13166266]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Villamartin.png";
    var marker = L.marker([36.84309608, -5.62372825]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Yecla.png";
    var marker = L.marker([38.65892926, -1.18588065]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
  
    var icon_url = "https://raw.githubusercontent.com/alexrsanchez/GraficosMapa/master/Temperaturasmoviles365yanomalias_Zafarraya.png";
    var marker = L.marker([36.99031408, -4.15383888]).bindPopup("<img src='" + icon_url + "' width=550 height=400/>",
                                                              {maxWidth: "auto", maxHeight: "auto"}).addTo(map);
 

  </script>
</body>
   

</html>
