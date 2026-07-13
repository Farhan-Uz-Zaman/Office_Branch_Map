# Office Branch Map

An interactive web application that visualizes office locations on a Google Map with a searchable, country-based sidebar summary.

## Features

* 🌍 Displays office locations using Google Maps.
* 📍 Color-coded markers grouped by country.
* 📂 Expandable sidebar listing offices by country.
* 🔢 Total office count.
* 🖱️ Click an office in the sidebar to:

  * Pan the map to the selected office.
  * Zoom into the location.
  * Display office details in an information window.
* 🗺️ Click a map marker to view office information.
* 📐 Automatically fits the map to display all office locations.

## Technologies Used

* HTML5
* CSS3
* JavaScript (Vanilla)
* Google Maps JavaScript API
* GeoJSON

## Data Source

Office information is retrieved from an API endpoint:

```text
YOUR_API_GATEWAY_URL
```

The endpoint is expected to return JSON in the following format:

```json
[
  {
    "branch_office_name": "Office Name",
    "country_name": "Country",
    "project_name": "Project Name",
    
  }
]
```

## Google Maps API

Replace the placeholder values before running the application.

### API Endpoint

```javascript
YOUR_API_GATEWAY_URL
```

### Google Maps API Key

Replace:

```text
GOOGLE_MAPS_API_KEY
```

with your own Google Maps JavaScript API key.

## Project Structure

```text
.
├── index.html
└── README.md
```

## Running the Project

1. Clone the repository.

```bash
git clone https://github.com/Farhan-Uz-Zaman/Office_Branch_Map.git
```

2. Open the project folder.

3. Replace:

   * `YOUR_API_GATEWAY_URL`
   * `GOOGLE_MAPS_API_KEY`

4. Serve the project using a local web server.

Examples:

Using Python:

```bash
python -m http.server
```

or

```bash
python3 -m http.server
```

Then open:

```text
http://localhost:8000
```

## Application Workflow

1. Initialize Google Maps.
2. Fetch office data from the API.
3. Group offices by country.
4. Generate an expandable country summary.
5. Convert office data into GeoJSON.
6. Display offices as color-coded markers.
7. Automatically fit the map to all locations.
8. Display office information when a marker or sidebar item is selected.

## Future Improvements

* Search by office name.
* Filter by country or project.
* Marker clustering for dense regions.
* Custom marker icons.
* Legend for country colors.
* Dark mode.
* Export office list to CSV.
* Responsive mobile layout.

## License

This project is intended for internal visualization and reporting purposes.
