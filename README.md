# Geolocation Toolkit

This Geolocation Toolkit package provides basic functionalities for working with geolocation data in JavaScript applications. It includes functions for geocoding addresses, reverse geocoding coordinates, and calculating distances between coordinates.

## Installation

You can install the Geolocation Toolkit package via npm:

```bash
npm install geolocation-toolkit
```

## Usage

Import the Geolocation Toolkit functions into your JavaScript code:

```javascript
const { geocode, reverseGeocode, calculateDistance } = require('geolocation-toolkit');
```

### Geocoding

To geocode an address (convert address to coordinates), use the `geocode` function:

```javascript
const coordinates = geocode('123 Main St, City, Country');
console.log(coordinates);
// Output: { latitude: 123.456, longitude: 789.012 }
```

### Reverse Geocoding

To reverse geocode coordinates (convert coordinates to an address), use the `reverseGeocode` function:

```javascript
const address = reverseGeocode(123.456, 789.012);
console.log(address);
// Output: '123 Main St, City, Country'
```

### Calculating Distance

To calculate the distance between two sets of coordinates, use the `calculateDistance` function:

```javascript
const distance = calculateDistance(40.7128, -74.0060, 34.0522, -118.2437);
console.log(distance);
// Output: 3934.28 // Distance in kilometers
```

## License

This Geolocation Toolkit package is licensed under the [MIT License](LICENSE).
