---
date_start: '04-02-25'
date_end : '05-02-25'
title: 'Vooronderzoek haroldk.nl'
slug: 'vooronderzoek-haroldk'
---

# intro

in [week 1](../blog/week-1.md) heb ik meer gekeken naar de opdracht van [haroldk.nl](https://www.haroldk.nl/), waarbij ik help met het maken van de website.

Tijdens het maken van deze briefing, had ik nog een aantal vragen over hoe ik bepaalde dingen opbouw. 

## Wat wil ik allemaal onderzoeken?
* ik wil kijken naar [sanity.io](https://www.sanity.io), waarbij ik wil kijken naar de werking hiervan en hoe ik een webite bouw met deze tool
* ook wil ik kijken naar [bandsintown](https://www.artist.bandsintown.com/integrations/spotify)
  * deze applicatie helpt data van spotify up-to-date te houden
    * dit gaat onder andere over dingen als optredens en data.

### [Sanity.io](https://www.sanity.io)
* CMS (content management system)
* het is een studio, waarin je een website kan bouwen. 
* Hierbij kan je werken via een zo gehete studio, waarin je dan een website kan creeeren. 

#### Welke vragen heb je?
Na wat snuffelen door de pagina's, kwamen een aantal vragen bij mij naar boven.

* Waar staan de assets van deze website?
  * Waar kan ik de repository vinden?
* Hoe word het live gezet?
* Er staat dus één dataset in, maar welke data staat er in hoe kan ik dit inzien?

#### Wat is je opgevallen aan het project?
* Het is gemaakt met next.js lijkt het 
  * Grote kans dat de deployment plaatsvind via vercel

#### Hoe vind ik de repo locatie?
Ik ben dus nu aan het kijken waar de repo daadwerkelijk staat. 

### [bandsintown](https://www.artist.bandsintown.com/integrations/spotify)
* ze hebben ook een sign up form voor een mailinglijst

#### Hoe kom je bij de data
> * [hier kan je een link vinden over hoe zij dit hebben beschreven](https://help.artists.bandsintown.com/en/articles/9186477-api-documentation)

* Als artiest moet je de data 

#### API
Om bij de api te komen, moet de api key worden opgehaald van de artiest. [hier](https://help.artists.bandsintown.com/en/articles/7053475-what-is-the-bandsintown-api) kan je de documentatie erover vinden

* hiervoor moet de artiest een account hebben
* om bij de api te kunnen komen, moet deze key worden opgehaald.

##### API links
Er zijn een aantal links die je kan gebruiken om zo bij de data (API) te komen

###### artist name
```
https://rest.bandsintown.com/artists/{{artist_name}}/?app_id=yOUrSuP3r3ven7aPp-id
```

###### artist ID
```
https://rest.bandsintown.com/artists/id_{{artist_id}}/?app_id=yOUrSuP3r3ven7aPp-id
```

###### facebook page
```
https://rest.bandsintown.com/artists/fbid_{{Facebook page id}}/?app_id=yOUrSuP3r3ven7aPp-id
 ```

 ##### event information
 met deze link zou je de informatie over de optredens en dergelijke kunnen krijgen

 ```
 https://rest.bandsintown.com/artists/{{artist_name}}/events/?app_id=yOUrSuP3r3ven7aPp-id
 
 ```

## Wat zijn je vragen aan de opdrachtgever?
* Ik heb even onderzocht hoe ik nou bij de code kom van de site. Dit is mij overgins niet echt duidelijk geworden. Sanity.io lijkt vanuit hier een rol te spelen waaruit de data word opgehaald. 
  * Het lijkt dus zo dat de code op een andere locatie staat in een repository. Dit is mij echter niet duidelijk. Daarom was ik benieuwd hoe de vorige frontender heeft gedaan. Is het handig voor mij om anders met hem in contact te komen en te kijken hoe hij dit heeft gedaan?
* óók heb ik naar [bandsintown](https://www.artist.bandsintown.com/integrations/spotify) gekeken. Om gebruik te maken van deze tool, is er een account nodig die laat zien dat hij/zij de manager is van het artiesten account. Door hiervoor een account aan te maken, kan er een zogehete sleutel worden opgehaald waarin alle data staat die van Spotify afkomt. 
  * Is er al een account aangemaakt hiervoor? Zo niet, lijkt het me handig als de opdrachtgever dit zelf doen. Zodat hij alle touwtjes in handen blijft hebben. Mocht er ooit in de toekomst iemand anders aan werken, kan hij er gemakkelijk bij. 
  * Er moet dus een account worden aangemaakt op [bandsintown](https://www.artist.bandsintown.com/integrations/spotify), waaruit uiteindelijk die sleutel moet worden opgevraagd. Door aan te melden kan jij je profiel claimen van Spotify. 
  > * [Hier kan een account gemaakt worden.](https://artists.bandsintown.com/signup?)
