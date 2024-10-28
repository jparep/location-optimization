# Coffee Shop Location Optimization

This project uses Python to optimize the placement of coffee shops based on public library locations within Chicago. Using data from the City of Chicago, the goal is to minimize the distance between libraries and coffee shops, ensuring accessibility for book readers to the nearest coffee shop. The project leverages toos such as DOcplex for optimization, geopy for ditance calculation, and folium for mapping.


## Table of Contents
- [Project Overview](#project-overview)
- [Installation](#installation)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [How It Works](#how-it-works)
- [License](#license)


## Project Overivew

This project retrieves public libraru data from the City of Chicago, computes the geographical distance between library locations, and uses prescriptive modeling to determine optimal locations for new coffee shops. By minimizing totla distance between libraries and selected coffee shop locations, we ensure that each library has convenient access to at least one coffee shop.


## Installation

1. Clone the repository
```bash
git clone github.com:jparep/location-optimization.git
```
2. Install dependencies
```bash
pip install -r requirements.txt
```
3. Ensure you have hte necessary API access if required (City of Chicago API library data)


## Usage

1. Run the script to fetch library data and build the optimization model:
```bash
python main.py
```

2. Upon successful execution, the script:

- Fetches and processes the data.
- Sets up the optimization model.
- Solves the model to find optimal coffee shop locations.
- Displays a map using folium with the coffee shops highlighted in red and libraries in default color.

3. View the generated map (displayed directly if using Jupyter, or saved to an HTML file if running as a script).


## Dependencies

The following Python libraries are required:

- geopy for calculating geographical distances
- requests for retrieving library data
- docplex for the optimization model
- folium for displaying results on a map

Install them with:
``bash
pip install geopy requests docplex folium
```