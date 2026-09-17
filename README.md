# YouTube Content Performance Dashboard
## M608 Business Project in Computer Science

An interactive Python Dashboard using the YouTube Data API v3, ipywidgets and Plotly to analyze YouTube Channel Metrics, Track Video Engagement and Visualize Monthly View Trends.

## **GitHub Repository Link**
https://github.com/emilyncynthiasamuel/YouTube-Content-Performance-Dashboard

## **Project Demonstration Video Link** 
https://www.youtube.com/watch?v=jkpVVBP6B3E

## Project Overview

This project is a YouTube Content Performance Dashboard, which is a Business Intelligence (BI) Application developed in Python using Live Data from the YouTube Data API v3. 
This project retrieves public statistics directly from the official visitBerlin YouTube channel and gives an overview into meaningful business insights through an interactive dashboard and the dashboard is designed for tourism business to analyze the performance of promotional videos.

## Business Problem

Tourism Businesses are often organized by Tourism Organizations, which regularly publish promotional videos on YouTube to attract Visitors and increase Destination Awareness and sometimes the manually monitored views, likes and comments and engagement rate across multiple videos is inefficient and that is the reason we have developed this dashboard, which provides a simple solution by automatically collecting live YouTube data and displaying it through the interactive visualizations for business decision making.

**Selected Tourist Organisation: visitBerlin**

**Industry: Tourism and Hospitality**

**Primary YouTube Channel: visitBerlin Official YouTube Channel : https://www.youtube.com/@visitBerlin**

**Target Audience: Travelers, culture enthusiasts, event goers and business delegates planning the visits in Berlin.**

**Key Stakeholder: Digital Marketing Manager (Tourism and Destination Branding)**

## Features
These are the Features:
(i) Live data retrieval using YouTube Data API v3
(ii) Automatic channel identification
(iii) Fetches the latest 50 Uploaded Videos (Public Videos)
(iv) Interactive dropdown menu
(v) Whole Channel Analytics
(vi) Individual Video Analytics
(vii) KPI Cards
(viii) Monthly Views Bar Chart
(ix) Video Details table
(x) Runs entirely inside Google Colab

## Technologies Used

| Technology          | Purpose                        |
| ------------------- | ------------------------------ |
| Python              | Programming language           |
| Google Colab        | Development environment        |
| YouTube Data API v3 | Live data source               |
| Pandas              | Data processing                |
| Plotly              | Interactive charts             |
| ipywidgets          | Interactive dropdown interface |

## Installing Required Libraries

Run Cell 1.

**!pip install google-api-python-client pandas plotly ipywidgets**

The notebook automatically installs all the required packages.

## Creating a YouTube API Key

This project uses the free YouTube Data API v3.

### Step 1

Open Google Cloud Console.

### Step 2

Create a new Google Cloud project.

### Step 3

Navigate to **APIs & Services**.

### Step 4

Click **Enable APIs and Services**.

### Step 5

Search for **YouTube Data API v3** and enable it.

### Step 6

Open **Credentials**.

### Step 7

Click **Create Credentials**.

### Step 8

Select **API Key**.

### Step 9

Copy the generated key.

Kindly, Replace Cell 2 with:

**API_KEY = "YOUR_API_KEY"**

Official Documentation: https://developers.google.com/youtube/v3

## How to Execute the Project

Follow these steps exactly for executing the Project.

### Step 1

Open the Notebook in Google Colab.

### Step 2

Run **Cell 1** to install all required libraries.

### Step 3

Insert your YouTube API key into **Cell 2**.

### Step 4

Run Cells **2 -> 9** sequentially.

Kindly Note: Do not skip any cells.

### Step 5

Wait for the dashboard to load.

### Step 6

Use the dropdown menu.

* **Whole Channel** displays overall analytics.
* Selecting any video displays that video's statistics.

## Dashboard Outputs

The dashboard displays:

(i) Total Views
(ii) Total Likes
(iii) Total Comments
(iv) Engagement Rate
(v) Published Date
(vi) Monthly Views Chart
(vii) Video Details Table

Kindly Note: The dashboard updates automatically whenever a different video is selected.

## YouTube API Requests

One complete execution performs only **3 API requests**.

| Endpoint        | Purpose                | Requests |
| --------------- | ---------------------- | -------: |
| channels().list | Retrieve Channel ID    |        1 |
| search().list   | Retrieve latest videos |        1 |
| videos().list   | Retrieve statistics    |        1 |
| **Total**       | Complete dashboard     |    **3** |

The implementation uses batch requests, making it efficient and suitable for repeated demonstrations.

## API Quota

The YouTube Data API v3 provides **10,000 quota units per day** for free projects.

This dashboard consumes only a very small portion of the daily quota and this is because video statistics are retrieved in one batch request.

## Future Improvements

(i) Comment sentiment analysis
(ii) Multiple channel comparison
(iii) Content Category filtering
(iv) Watch time analytics
(v) Audience retention metrics
