# Y'a quoi comme série API issues tracker

## Report an issue if your favorite show is missing or if IDs data is not correct - indexed shows in `indexed_shows_in_API.csv`

## Get tv shows info by AlloCiné, BetaSeries, IMDb or SensCritique ID
https://yqcsapi.com - For requests examples visit the [Postman documentation](https://documenter.getpostman.com/view/10720213/TzRUB74j).

### GET - Get shows by title (return 1+ results)
```https://yqcsapi.com/shows?title=game%20of%20thrones```
#### PARAMS
**title**: game%20of%20thrones

### GET - Get show by AlloCiné, BetaSeries, IMDb or SensCritique ID (return 1 result)
#### AlloCiné
```https://yqcsapi.com/shows?allocineId=7157```
#### BetaSeries
```https://yqcsapi.com/shows?betaseriesId=gameofthrones```
#### IMDb
```https://yqcsapi.com/shows?imdbId=tt0944947```
#### SensCritique
```https://yqcsapi.com/shows?senscritiqueId=Game_of_Thrones/225391```
#### PARAMS
**allocineId**: 7157

**betaseriesId**: gameofthrones

**imdbId**: tt0944947

**senscritiqueId**: Game_of_Thrones/225391
### RESULT
```
{
    "_id": "60924c07df5f9bf1dbe4ed36",
    "show": {
        "title": "Game of Thrones",
        "allocine": {
            "id": 7157,
            "url": "https://www.allocine.fr/series/ficheserie_gen_cserie=7157.html",
            "creationYear": 2011,
            "endingYear": 2019,
            "status": "Ended",
            "synopsis": "Il y a très longtemps, à une époque oubliée, une force a détruit l'équilibre des saisons. Dans un pays où l'été peut durer plusieurs années et l'hiver toute une vie, des forces sinistres et surnaturelles se pressent aux portes du Royaume des Sept Couronnes. La confrérie de la Garde de Nuit, protégeant le Royaume de toute créature pouvant provenir d'au-delà du Mur protecteur, n'a plus les ressources nécessaires pour assurer la sécurité de tous. Après un été de dix années, un hiver rigoureux s'abat sur le Royaume avec la promesse d'un avenir des plus sombres. Pendant ce temps, complots et rivalités se jouent sur le continent pour s'emparer du Trône de Fer, le symbole du pouvoir absolu.",
            "runtime": 52,
            "genres": [
                "Drame",
                "Fantastique"
            ],
            "criticsRating": 4.1,
            "criticsNumber": 7,
            "criticsRatingDetails": [{
                    "criticName": "Entertainment weekly",
                    "criticRating": 5
                },
                {
                    "criticName": "The Hollywood Reporter",
                    "criticRating": 5
                },
                {
                    "criticName": "Variety",
                    "criticRating": 5
                },
                {
                    "criticName": "Hitfix",
                    "criticRating": 4
                },
                {
                    "criticName": "Pittsburg Post-Gazette",
                    "criticRating": 4
                },
                {
                    "criticName": "TV Squad",
                    "criticRating": 4
                },
                {
                    "criticName": "Wall Street Journal",
                    "criticRating": 1.5
                }
            ],
            "usersRating": 4.7,
            "seasonsRatingDetails": [{
                    "seasonNumber": 1,
                    "seasonRating": 4.6
                },
                {
                    "seasonNumber": 2,
                    "seasonRating": 4.7
                },
                {
                    "seasonNumber": 3,
                    "seasonRating": 4.7
                },
                {
                    "seasonNumber": 4,
                    "seasonRating": 4.7
                },
                {
                    "seasonNumber": 5,
                    "seasonRating": 4.5
                },
                {
                    "seasonNumber": 6,
                    "seasonRating": 4.6
                },
                {
                    "seasonNumber": 7,
                    "seasonRating": 4.5
                },
                {
                    "seasonNumber": 8,
                    "seasonRating": 3
                }
            ]
        },
        "betaseries": {
            "id": "gameofthrones",
            "url": "https://www.betaseries.com/serie/gameofthrones",
            "usersRating": 4.68
        },
        "imdb": {
            "id": "tt0944947",
            "url": "https://www.imdb.com/title/tt0944947/",
            "usersRating": 9.39
        },
        "senscritique": {
            "id": "Game_of_Thrones/225391",
            "url": "https://www.senscritique.com/serie/Game_of_Thrones/225391",
            "usersRating": 8.2
        }
    }
}
```