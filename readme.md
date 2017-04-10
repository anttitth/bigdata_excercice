## Bigdata harjoitystyö

Harjoitustyö tehtiin Jyväskylän ammattikorkeakoulun Bigdata kurssilla. Tehtävänantona oli yhdistää kaksi eri tietolähdettä vapaavalintaisessa ympäristössä ja analysoida sitä vapaavalintaisen hypoteesin perusteella. Tietolähteillä oletetaan olevan jokin yhteys, joka pyritään tuomaan esille. Harjoitustyön tarkoituksena on tutustua valittuun ympäristöön, mikä tässä tapauksessa oli Ibm Bluemix sekä harjoitella datan keräämistä ja sen analysointia.

# Toteutus

Harjoitustyössä kerättiin dataa noderediin muodostetun flown avulla, joka on tallennettuna koodina .json -muodossa. Ylimääräisnä nodeina tuotiin worldmap, mikä piirtää koordinaattipisteet kartalle, sentiment-node, mikä arvioi twitterviestin positiivisuuden sekä openweathermap, mikä hakee annettujen koordinaattipisteiden avulla säätiedot.

Harjoitustyössä halutut tiedot (sää, sentiment arvo, sijainti) tallennettiin cloudantin tietokantaan, mistä se exportattiin dashdb-työkaluun analysointia varten. Tiedoista analysoitiin sitä, onko viestit positiivisempia hyvällä säällä.

Lopputulos: Kerättyä dataa ehdittiin tallentaa vain lyhyen aikaa, jolloin ei voitu tehdä luotettavaa vertailua siitä, onko viestit positiivisempia hyvällä säällä. Kerätystä datasta voitiin kuitenkin päätellä, että hyvällä säällä tehdään päivityksiä twitteriin huomattavasti enemmän kuin huonolla säällä.
