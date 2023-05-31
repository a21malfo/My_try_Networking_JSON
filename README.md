
# Rapport

**
Detta är ett helt nytt försök att få till JSON data genom att skapa ett nytt projekt där jag gör allt
i mitt egna projekt. Något verkar vara väldigt fel i det forkade projekten till min dator. Kan ha
att göra med min dators (MAC) inställningar. Men då jag testar flera gånger om med att ändra i koden
samt gjort ett tidigare projekt och fick recylerView att fungera samt använda URL för att läsa in
data från internet så testar jag detta i ett sista försök. För skulle Ni se alla mina errors i
Logcat så verkar problemet ligga djupare än i koden.

Så jag börjar om från början helt enkelt. 

Jag börjar med att skapa en README.md fil under projektet. Det som nu också är annorlunda är att jag
själv skapar en assets fil där jag lägger in JSON datan. 

Jag börjar dock med att skapa alla klasser jag behöver, assets foldern och xml.fil för JSON datan. 








Gjort om några gånger så denna är min 5 fork, jag har nu i sista försöket utgått från mitt projekt
då jag fick det att fungerar där. Dock genom URL:n.

Först skapades en recyclerview i activity main.
Därefter skapades en layout för en recyclerview i activity_main.xml.

Skapa en ny java.class "Mountain". Använde Getter och Setter för att generera variablerna och
funktionen toString()

Därefter skapades Arraylist för klassen Mountain i MainActivity.class

Efter det skapades en ny layout resouce file, json_data.xml för json data.

Gav permission till internet i AndroidManifest.xml

Kod:
```
 <uses-permission android:name="android.permission.INTERNET" />
```

Deklarerade RecyclerViewAdapter med namnet mountainAdapter i MainActivity.java filen.

Skapade sedan javaklassen RecyclerView där jag lade in kod för både adaptern och holdern. Lade
holdern i sama java.fil som adaptern.

Fungerade inte fick en massa felmeddelande bland att permission denied i kombination med något som
heter WAKE LOCK. Googlade på detta och hittade en kod att lägga till i AndroidManifest.xml men
funkade ändå inte.

Kod:

```
<uses-permission android:name="android.permission.WAKE_LOCK" />
```
Lät dock koden vara kvar då den gav felmeddelande innan.
**

_Du kan ta bort all text som finns sedan tidigare_

## Följande grundsyn gäller dugga-svar:

- Ett kortfattat svar är att föredra. Svar som är längre än en sida text (skärmdumpar och programkod exkluderat) är onödigt långt.
- Svaret skall ha minst en snutt programkod.
- Svaret skall inkludera en kort övergripande förklarande text som redogör för vad respektive snutt programkod gör eller som svarar på annan teorifråga.
- Svaret skall ha minst en skärmdump. Skärmdumpar skall illustrera exekvering av relevant programkod. Eventuell text i skärmdumpar måste vara läsbar.
- I de fall detta efterfrågas, dela upp delar av ditt svar i för- och nackdelar. Dina för- respektive nackdelar skall vara i form av punktlistor med kortare stycken (3-4 meningar).

Programkod ska se ut som exemplet nedan. Koden måste vara korrekt indenterad då den blir lättare att läsa vilket gör det lättare att hitta syntaktiska fel.

```
function errorCallback(error) {
    switch(error.code) {
        case error.PERMISSION_DENIED:
            // Geolocation API stöds inte, gör något
            break;
        case error.POSITION_UNAVAILABLE:
            // Misslyckat positionsanrop, gör något
            break;
        case error.UNKNOWN_ERROR:
            // Okänt fel, gör något
            break;
    }
}
```

Bilder läggs i samma mapp som markdown-filen.

![](android.png)

Läs gärna:

- Boulos, M.N.K., Warren, J., Gong, J. & Yue, P. (2010) Web GIS in practice VIII: HTML5 and the canvas element for interactive online mapping. International journal of health geographics 9, 14. Shin, Y. &
- Wunsche, B.C. (2013) A smartphone-based golf simulation exercise game for supporting arthritis patients. 2013 28th International Conference of Image and Vision Computing New Zealand (IVCNZ), IEEE, pp. 459–464.
- Wohlin, C., Runeson, P., Höst, M., Ohlsson, M.C., Regnell, B., Wesslén, A. (2012) Experimentation in Software Engineering, Berlin, Heidelberg: Springer Berlin Heidelberg.
