# Earthquake data 5 februari 2024

![image](https://github.com/mia-mmt2-2324/earthquakes/assets/36117924/18d267b2-969c-4915-b0e8-c4f0e90ae66b)


Als je in deze repo op **4.5_day.geojson** klikt, en vervolgens rechts op de button **Raw**, krijg je de ruwe data te zien in je browser. De URL daarbij is: `https://raw.githubusercontent.com/mia-mmt2-2324/earthquakes/main/4.5_day.geojson`. Dit is tevens de URL die je dient te gebruiken in je p5js project:


```
let data;

function preload(){
    data = loadJSON("https://raw.githubusercontent.com/mia-mmt2-2324/earthquakes/main/4.5_day.geojson");
}

function setup(){
    console.log(data.metadata.title); //controleren of de data correct is ingeladen
}
``` 

De data is overgenomen van de website https://earthquake.usgs.gov/earthquakes/feed/v1.0/geojson.php en we gebruiken daarvan specifiek de dataset die aardbevingen van een Magnitude van 4.5 en hoger van de afgelopen dag. Omdat deze data uiteraard per dag wijzigt, kan het voorkomen dat er een keer in de data géén aardbeving is geweest; lastig visualiseren dan 😜. We hebben dus een kopie gemaakt van die dataset op een moment dat er veel aardbevingen waren en die opgeslagen in deze repo. Je hoeft dus enkel die externe website raad te plegen als je wat meer informatie nodig hebt, wat alle eigenschappen betekenen etc. 

