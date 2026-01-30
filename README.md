dashboard.py

This is the main application file that runs the Streamlit dashboard
Responsibilities:
Loads the water quality dataset
Creates a multi-tab Streamlit interface
Displays:
Raw data and descriptive statistics
2D plots (line and scatter plots)
3D geographic visualization
NASA Astronomy Picture of the Day (APOD)
Calls functions from api.py to retrieve external API data
How to run:
streamlit run dashboard.py

api.py

This file contains helper functions for external API communication.
Responsibilities:
Handles HTTP requests to NASA’s APOD API
Separates API logic from UI logic
Returns structured JSON data for use in the dashboard
This modular design improves readability, maintainability, and reusability.

biscayneBay_waterquality.csv

This CSV file contains the water quality dataset used by the dashboard.
Example fields include:
Time
Temperature (°C)
pH
Dissolved Oxygen (ODO mg/L)
Latitude and Longitude

.env
This file stores environment variables for sensitive API keys.

The following Python libraries are required:
streamlit
pandas
plotly
requests
python-dotenv

Total Water Column (m)

The dataset is loaded and analyzed using the Pandas library.
