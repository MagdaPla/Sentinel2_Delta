# Sentinel2_Delta
Codi en JAva-script per executar des de Google Earth Engine. 
El Codi següent es pot copiar al https://code.earthengine.google.com/?authuser=1 
Com que en el projecte quantificació de danys als arrossars en calen imatges totalment lliures de núvols per a la zona d'interès ens cal revisar prèviament cadascuna de le simatges, així que hi ha un codi per anar visualitzant les imatges. El filtrats per núvols no em funcionaven bé doncs es donava llindars a nivell de tota la imatge enlloc de tot el fragment. 

Una vegada veiem que són correctes copiel el nom de la imatge en un txt i finalment anirem descarregant cadascuna d'aquestes imatges sel·leccionades, baixant les tres bandes necessàries per a calcular el NDVI.

Hauríem pogut calcular el NDVI i baixar cada imatge però en aquest cas he preferit tenir les imatges originals per a editar la memòria, per a fer comprobacions de parcel·les d'estudi, etc. 

A més, els processos de mosaicat trobats no em servien per a mosaicar imatges concretes, doncs mosaiquen imatges d'una sèrie temporal per data, etc. i tenint en compte que no les faria servir totes he trobat que no era necessari.

Una vegada descarregades les imatges es mosaicaren les dues passades de cada data (TBF i TCF) i es calcularà NDVI o altres índexs que siguin necessaris.
