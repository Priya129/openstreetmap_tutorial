# Flutter Map with Directions

A Flutter project that integrates mapping, real-time location tracking, and routing functionalities using OpenStreetMap (OSM) and OSRM APIs.

## Features

- **Real-time User Location Tracking**  
  - Uses the `location` package to access the device’s GPS location.
  - Displays the user's current position on the map.

- **Search for Destination**  
  - Users can enter a location name in the search bar.  
  - Uses the Nominatim API to fetch latitude and longitude for the searched location.

- **Display Map Using OpenStreetMap**  
  - Integrates the `flutter_map` package to render OpenStreetMap tiles.  
  - Provides zooming and panning functionalities.

- **Navigation Route from Current Location to Destination**  
  - Uses the OSRM (Open Source Routing Machine) API to fetch the shortest route.  
  - The route is displayed as a red polyline on the map.

- **Custom Markers for User and Destination**  
  - A blue navigation icon represents the user’s location.  
  - A red pin represents the searched destination.

- **Real-time Location Updates**  
  - Listens to location changes and updates the user’s position on the map dynamically.

- **Error Handling and User Feedback**  
  - Displays error messages when location search fails or route fetching is unsuccessful.

## Packages Used

| Package Name | Purpose |
|-------------|---------|
| **flutter_map** | Displays OpenStreetMap (OSM) tiles and map features. |
| **flutter_map_location_marker** | Shows the user’s live GPS location on the map. |
| **latlong2** | Provides latitude-longitude handling for map-related calculations. |
| **location** | Fetches real-time user location using device GPS. |
| **http** | Makes API requests to fetch location data and routes. |

## APIs Used

1. **Nominatim API** (https://nominatim.org/)  
   - Converts a location name (e.g., "New York") into latitude and longitude.  
   - Used for geocoding to find destination coordinates.

2. **OSRM API** (http://project-osrm.org/)  
   - Computes the shortest route from the user's current location to the destination.  
   - Returns a polyline that represents the route.



