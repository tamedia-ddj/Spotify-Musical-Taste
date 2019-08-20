# Spotify-Musical-Taste

### Examples to demonstrate how to analyse musical taste with the Spotify API

<!---
optional folgendermassen Bild einfügen:
![Trump Hate](dt.png)
Source: [Gage Skidmore](https://www.flickr.com/photos/gageskidmore/32758233090)>)
--->
 
**Data Source**: Spotify

**Article**: [The online Tool will be published here](https://www.tagesanzeiger.ch/)  


## Table of Content
  * [Introduction](#introduction)
  * [Spotify API / Spotipy](#spotify-api---spotipy)
  * [Analysis](#analysis)
  * [Input Files](#input-files)
  * [Output Files](#output-files)
  * [License](#license)


## Introduction
What is the musical taste of the different generations living in Switzerland? To answer this question, the Tamedia Datajournalism Team looked at data from Spotify and built the [Musical-Taste Analysis Tool available here](https://www.tagesanzeiger.ch/).  

As a reminder we define the generations as follows:  
- Generation Z: born 1994 or later  
- Generation Y: born 1981-1994  
- Generation X: born 1965-1980  
- Generation Babyboomer: born 1946-1964  

We asked Spotify to give us the 100 most often played songs from these generations. These lists are shared here in the "Data_Input" folder. The musical features of these songs were then analysed visualized.  

Additionaly, the user can then compare his own musical taste with the average of the Top100 of the different generations.

This Github repository will not show or explain all the calculations done in the online Tool. Rather it should show some examples, how to use the Spotify API to analyze Audio Features.

## Spotify API / Spotipy

**Spotify API:**  
We use the spotify API for two things:
- Getting musical features of songs
- Getting the Top100 tracks of users

The authorization process is bit tricky. First you need a Spotify account. Then you need to upgrade this account to a developer account and you need to create a "Spotify App" in this account. From this App you need the Client-ID and the Client-Secret-ID. For help with the authorization pross check the corrsponding documentation on [spotify.com](https://developer.spotify.com/documentation/general/guides/authorization-guide/) and [Spotipy](https://spotipy.readthedocs.io/en/latest/#authorized-requests)  

For General Documentation refer to the [Spotify API-Documentation](https://developer.spotify.com/documentation/web-api/)

**Spotipy**  
To facilitate working with the Spotify API, the package "Spotipy" was used. Documentation can be found here: https://spotipy.readthedocs.io/

## Analysis
The Jupiter Notebook shows some examples how to get and analyse Songs with the Spotify API using the Spotipy package. There are further explanations and comments in the Notebook.

## Input Files

### gen_.csv

Top100 Tracks received from Spotify. One file per generation.

Variable | Description
--- | --- 
`uri ` | Spotify-URI
`artist ` | Artist Name
`track ` | Track Name


## Output Files
- all_gen_artists_count.csv: Which artists show up how many times in each generations Topp 100 Songs
- all_gen_average_values.csv: Average values for different audio features for each generation

## License

*Spotify-Musical-Taste* is free and open source software released under the permissive MIT License.
