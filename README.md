# R Geocoding API

This project provides a simple REST API to geocode addresses using R, the plumber package, and the tidygeocoder package.

## Requirements

- R (>= 4.0.0)
- plumber package
- tidygeocoder package

## Installation

1. Install the required R packages:

```R
install.packages("plumber")
install.packages("tidygeocoder")
```

2. Clone this repository or download the geocode_api.R file.

## Usage

1. Run the API locally:

```R
library(plumber)
api <- plumb("geocode_api.R")
api$run(port = 8000)
```

2. Send a request to the API:
curl "http://localhost:8000/geocode?address=1600+Amphitheatre+Parkway,+Mountain+View,+CA"

## License

This project is licensed under the MIT License.
