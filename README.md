# Transport Catalogue

Transport Catalogue is a C++ project designed to efficiently store, query, and visualize transportation data, such as bus routes and stops. It provides powerful tools for managing transportation networks and optimizing route planning.

## Features

- **Data Storage**: Efficient storage for bus stops, routes, and distances.
- **Query System**: Retrieve detailed information about specific routes and stops.
- **Route Optimization**: Calculate optimal routes based on stored data.
- **Map Rendering**: Generate SVG maps for visualizing transportation networks.
- **JSON Input/Output**: Interact with the catalogue through JSON files.

## Requirements

- **C++ Compiler**: Compatible with C++17 or newer.
- **Libraries**:
  - Standard Template Library (STL)
  - JSON parsing library (e.g., `nlohmann/json`)
  - SVG rendering library (if external libraries are used)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/StasWagner/TransportCatalogue.git
   cd TransportCatalogue
   ```

2. Build the project:
   ```bash
   mkdir build
   cd build
   cmake ..
   make
   ```

3. Run the application:
   ```bash
   ./transport_catalogue
   ```

## Usage

1. **Provide Input**: Prepare a JSON file with bus stops, routes, and distances.

2. **Run Queries**: Use the application to query routes and visualize the data.

3. **View Results**: Analyze the output JSON or generated SVG map.

## Example Input

```json
{
  "base_requests": [
    {
      "type": "Stop",
      "name": "Stop A",
      "latitude": 55.751244,
      "longitude": 37.618423
    },
    {
      "type": "Bus",
      "name": "Bus 1",
      "stops": ["Stop A", "Stop B", "Stop C"],
      "is_roundtrip": true
    }
  ]
}
```

## Example Output

- JSON query results
- SVG map file
