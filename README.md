# Belly Button Biodiversity Dashboard

Welcome to the Belly Button Biodiversity Dashboard! This project visualizes data from the Belly Button Biodiversity dataset, which catalogs the microbial species found in human navels. The dataset reveals that a small number of microbial species (also known as operational taxonomic units, or OTUs) are present in more than 70% of people, while others are relatively rare.

The goal of this project is to build an interactive dashboard using D3.js and Plotly.js to explore the Belly Button Biodiversity dataset. Users can select individual samples from a dropdown menu to view detailed information about the microbial species found in those samples. The dashboard includes:

- A horizontal bar chart displaying the top 10 OTUs found in the selected individual.
- A bubble chart showing the distribution and abundance of all OTUs in the sample.
- A demographic information panel displaying the selected individual's metadata.

## Deployment

The project is deployed on GitHub Pages. 
You can access the dashboard via URL:
https://steve-yuan-8276.github.io/belly-button-challenge/

## Features

### Demographic Information

- **Metadata Display**: The panel displays the selected individual's demographic information, including ID, ethnicity, gender, age, location, and other relevant data.

### Interactive Dropdown Menu

- **Sample Selection**: Users can select different samples from the dropdown menu to update the charts and metadata panel.

### Bar Chart

- **Top 10 OTUs**: The bar chart displays the top 10 OTUs found in the selected sample.
- **Sample Values**: The chart uses `sample_values` as the values for the bars.
- **OTU IDs**: The chart uses `otu_ids` as the labels for the bars.
- **Hovertext**: The chart uses `otu_labels` to display additional information when hovering over each bar.

### Bubble Chart

- **OTU Distribution**: The bubble chart shows the distribution of all OTUs in the selected sample.
- **X Values**: The chart uses `otu_ids` for the x-axis values.
- **Y Values**: The chart uses `sample_values` for the y-axis values.
- **Marker Size**: The marker sizes are determined by `sample_values`.
- **Marker Colors**: The marker colors are determined by `otu_ids`.
- **Hovertext**: The chart uses `otu_labels` to display additional information when hovering over each bubble.

## Technologies Used

- **D3.js**: Used for data manipulation and fetching the JSON data.
- **Plotly.js**: Used for creating the interactive bar and bubble charts.
- **JavaScript**: Handles the logic for updating charts and displaying metadata.

## Project Structure

- `index.html`: The main HTML file that contains the structure of the dashboard.
- `static/js/app.js`: The JavaScript file that handles data fetching, processing, and visualization.
- `samples.json`: The dataset used for this project.
