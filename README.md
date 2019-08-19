# Spotify-Musical-Taste

### Untertitel

<!---
optional folgendermassen Bild einfügen:
![Trump Hate](dt.png)
Source: [Gage Skidmore](https://www.flickr.com/photos/gageskidmore/32758233090)>)
--->

Short Description: Examples to demonstrate how to analyze musical taste with the Spotify API



#### 
**Datenquelle(n)**: Quelle des Datensatzes: BLW

**Artikel**: [The online Tool will be published here](https://www.tagesanzeiger.ch/)

## bei grösseren Projekten: Inhaltsverzeichnis

1. Introduction / Available Data
2. Spotify API / Spotipy
3. Getting the User top 100 Songs
4. Analysis


## Introduction
What is the musical taste of the different generations living in Switzerland? This is the basic question we want to answer with this analysis and the corresponding online-Tool.

As a reminder we define the generations as follows:
Generation Z: born 1994 or later
Generation Y: born 1981-1994
Generation X: born 1965-1980
Generation Babyboomer: born 1946-1964

We asked Spotify to give us the 100 most often played songs from these generations. These lists are shared here in the "Data_Input" folder. The musical features of these songs were then analysed visualized.

The user can then compare his own musical taste with the averge of the Top100 of the different generations.


## Spotify API / Spotipy

Einige Beispielelemente:

**Spotify API:**
We use the spotify API for two things:
- Getting musical features of songs
- Getting the Top100 tracks of users

https://developer.spotify.com/documentation/web-api/

**Spotipy**
To facilitate working with the Spotify API, the package "Spotipy" was used. Documentation can be found here: https://spotipy.readthedocs.io/


* item 1
* item 2
* item 3
* ...







## Input Files

### gen_.csv

Top100 Tracks received from Spotify by generation

Variable | Description
--- | --- 
`uri ` | Spotify-URI
`artist ` | Artist Name
`track ` | Track Name




## License

*Projekttitel* is free and open source software released under the permissive MIT License.
