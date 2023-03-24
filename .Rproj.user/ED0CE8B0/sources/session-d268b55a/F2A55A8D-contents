library(plumber)
library(tidygeocoder)

#* @apiTitle Geocoding API

#* Geocode an address
#* @param address The address to geocode
#* @get /geocode
function(address) {
  if (missing(address) || address == "") {
    return(list(error = "Please provide an address."))
  }
  
  result <- geocode(address, method = 'osm')
  
  if (nrow(result) == 0) {
    return(list(error = "No results found for the given address."))
  }
  
  return(result)
}
