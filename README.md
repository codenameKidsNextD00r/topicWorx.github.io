# COVID-19 Data Visualization

This project visualizes COVID-19 data using a line chart. It allows users to filter the data by date range and view trends in Total Confirmed Cases, Active Cases, Total Deaths, and Total Recovered.
[Click here to view live demo](https://codenamekidsnextd00r.github.io/topicWorx.github.io/)

## Features
- **Interactive Line Chart**: Visualizes COVID-19 data over time.
- **Date Filtering**: Users can filter data by selecting a date range.
- **Responsive Design**: Works on both desktop and mobile devices.

## Libraries Used
- [Chart.js](https://www.chartjs.org/): A JavaScript library for rendering charts.
- [Bootstrap](https://getbootstrap.com/): A CSS framework for styling and layout.

## How to Run the Code
1. **Download the Files from Github**: Ensure you have the following files:
   - `index.html`
   - `covid.json` (sample data file)

    [Download available here](https://github.com/codenameKidsNextD00r/topicWorx.github.io)
2. **Open in a Browser**: Open the `index.html` file in a modern web browser (e.g., Chrome, Firefox, Edge).
    - you can drag and drop index.html into your browser or
    - type the location of the file in your browser's address bar e.g `http://localhost/topicWorx.github.io-main/index.html`
3. **Use the Filters**: 
   - Select a date range using the "Date From" and "Date To" fields.
   - Click "Submit" to update the chart.
   - Leaving the date fields empty or cleared will return the whole data set by default.
   - Click on one of the keys in the legend e.g `Total Confirmed Cases` to filter displayed data.

## Code Explanation
### HTML Structure
- The `index.html` file contains the structure of the web page, including:
  - A form for date filtering.
  - A canvas element for rendering the chart.
  - A footer.

### JavaScript Functionality
- **Fetching Data**: The `fetchData()` function fetches the COVID-19 data from the `covid.json` file.
- **Filtering Data**: The `filterData()` function filters the data based on the selected date range.
- **Rendering the Chart**: The `renderChart()` function uses Chart.js to render the line chart. It updates the chart dynamically when the date range is changed.
- **Date Formatting**: To enable filtering, the date date types from the form (ISO date format) had to be converted to match the date formatting provided in the JSON file

### Styling
- Bootstrap is used for styling the form, buttons, and layout.
- Custom CSS is added for additional styling, such as font and container width.

## Tips for Using the Software
- Ensure the `covid.json` file is in the same directory as the `index.html` file.
- Use a modern web browser for the best experience.
- If the chart does not update, check the browser console for errors.

## Sample Data
The `covid.json` file contains sample data in the following format:
```json
[
  {
    "Date": "2023/01/01",
    "Total Confirmed Cases": 1000,
    "Active Cases": 500,
    "Total Deaths": 50,
    "Total Recovered": 450
  },
  ...
]