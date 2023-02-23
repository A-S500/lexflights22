# lexflights22

A data package built with [`{anyflights}`](https://anyflights.netlify.app/).

```r
anyflights::anyflights("LEX", 2022, 1:11) |>
  anyflights::as_flights_package("lexflights22")
```



The main data is:

- `flights`

  - Data on (most?) flights departing Lexington Bluegrass between January and November 2022
  
- `weather`

  - Hourly weather data from the LEX weather station

The remaining are data data dictionaries.

- `airlines`

  - Gives the full name associated with the two letter carrier column in flights.

- `airports`

  - Gives several points of metadata, including the full `$name` associated with the three letter faa symbol found in `flights$origin` and `fights$dest`.

- `planes`

  - Gives a lot of metadata for each plane associated with its `$tailnum`
