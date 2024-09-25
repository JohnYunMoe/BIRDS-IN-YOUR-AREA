# BIRDS-IN-YOUR-AREA
Short project made for the first assignment of NYU STERN class TECH-UB 24(PROJECTS IN PROGRAMMING)
# Geolocation and eBird API Integration

## Project Overview

This project retrieves the user's geographical location based on their IP address and fetches recent bird sightings in that area using the eBird API. 

## Technologies Used

- **Python 3.x**: The primary programming language used for this project.
- **Requests Library**: Used for making HTTP requests to external APIs.
- **Abstract API**: For geolocation services based on IP address.
- **eBird API**: To fetch recent bird observation data.

## How It Works

1. **API Keys**:
   - The project retrieves API keys for both the Abstract API and the eBird API using Google Colab's `userdata` feature.

2. **Get User Location**:
   - The `get_location()` function calls the Abstract API to get the user's city, region, and country code based on their IP address.

3. **Fetch Bird Sightings**:
   - The `birds_in_location(country_code)` function constructs a request to the eBird API using the retrieved country code.
   - It processes the response and returns a dictionary containing bird names, their observation locations, and observation dates.

4. **Display Results**:
   - The `main()` function orchestrates the flow by calling the location and bird sighting functions, then displays the results in a user-friendly format.

## Example Output

Upon execution, the program outputs:
- The city, region, and country code.
- A list of recent bird sightings in the format:


## Conclusion

This project demonstrates how to integrate geolocation and wildlife observation APIs to provide users with real-time data about bird sightings based on their location.


