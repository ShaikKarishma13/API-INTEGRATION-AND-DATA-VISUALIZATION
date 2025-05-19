# API-INTEGRATION-AND-DATA-VISUALIZATION

*COMPANY:* CODTECH IT SOLUTIONS  
*NAME:* SHAIK KARISHMA   
*INTERN ID:* CT06WP105
*DOMAIN:* PYTHON DEVELOPMENT  
*DURATION:* 6 WEEKS  
*MENTOR:* NEELA SANTOSH



## Overview

This project demonstrates the integration of a public API with Python to fetch real-time data and visualize it using powerful data visualization libraries. The specific task focuses on utilizing the *OpenWeatherMap API* to retrieve weather forecast data for a given city and then creating meaningful insights using *Matplotlib* and *Seaborn*. The aim is to transform raw weather data into an easily interpretable visual format, which helps users better understand temperature and humidity trends over time.

## Tools and Technologies Used

- *Python*: The core programming language used to implement the solution. Python is chosen for its simplicity, extensive libraries, and strong community support.
- *Requests*: A Python HTTP library used to make API calls to OpenWeatherMap and fetch weather data in JSON format.
- *Matplotlib*: A widely-used Python library for creating static, interactive, and animated visualizations. It was used here for plotting graphs.
- *Seaborn*: A Python visualization library based on Matplotlib that provides a high-level interface for drawing attractive statistical graphics.
- *OpenWeatherMap API*: A public weather API that provides real-time and forecasted weather data for any city in the world. It requires an API key to access its services.
- *Datetime*: A built-in Python module used to convert Unix timestamps into human-readable date and time formats.

## Problem Statement

*Objective*: Use Python to fetch data from a public API and visualize it.

*Instructions*:
- Use Python to fetch data from a public API (e.g., OpenWeatherMap).
- Process and extract meaningful data points.
- Create visualizations using Matplotlib or Seaborn.
- Deliverables: A complete Python script and a visualization dashboard.

## Project Implementation

The script begins by importing the necessary Python libraries. The Seaborn style is set for consistent and clean visuals. An API key and the desired city (Delhi) are configured to make a request to OpenWeatherMap’s 5-day forecast API endpoint.

After sending the request, the response is checked for success. If successful, the script extracts timestamped weather data points including temperature and humidity from the forecast list. These values are stored in lists which are then used for visual representation.

The data visualization section is handled using Matplotlib and Seaborn. Two line plots are created:

1. *Temperature vs Time* – This graph displays how the temperature is expected to change over the forecasted period.
2. *Humidity vs Time* – This graph shows humidity trends during the same time frame.

Both graphs are shown in a single dashboard using Matplotlib's subplot feature, with rotated x-axis labels for better readability.

## Applications of This Project

This type of task has wide-ranging real-world applications across various industries:

- *Weather Monitoring Dashboards*: Such visualizations can be integrated into apps or websites to provide users with graphical weather forecasts.
- *Smart Agriculture*: Farmers can use weather trend data to make informed decisions about irrigation, planting, and harvesting.
- *Data Journalism*: Journalists and bloggers can utilize such tools to visually represent climate trends in their reports.
- *Education*: Students learning about data analysis, APIs, or Python can use this project as a foundational example for hands-on experience.
- *Smart Home Integration*: IoT devices can use such data to automate actions (e.g., closing windows if rain is predicted).
- *Travel Planning*: Tour companies or individual travelers could use similar tools to check upcoming weather conditions visually.

## Learning Outcomes

By working on this project, I learned how to:
- Interact with RESTful APIs using Python.
- Handle and parse JSON responses.
- Convert timestamps to readable formats.
- Create dual-graph dashboards using Python visualization libraries.
- Improve the readability and aesthetics of plots using Seaborn styles.


##OUTPUT:
![Image](https://github.com/user-attachments/assets/f594ddc4-3a8a-4e33-ae90-e8f4f047cb3f)

![Image](https://github.com/user-attachments/assets/ca0c0877-174b-4e09-a668-f6578b1482c5)

