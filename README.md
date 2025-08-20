# Hotel Segmentation Strategy

An AI-powered chatbot designed to support Fidelidade's insurance agents by providing instant, accurate answers to complex product questions using Retrieval-Augmented Generation (RAG) technology.

## Project Overview

This solution was developed as part of the Business Cases with Data Science course in the MSc in Data Science and Advanced Analytics program at NOVA IMS, Lisbon. The course provides hands-on experience with real-world cases presented by established clients. This particular case was proposed by Fidelidade Insurance Company. <br>

The client’s business need was to develop customer segmentation strategy for hotel chain by targeting marketing based on geographic, demographic, and behavioral characteristics. The goal was to identify distinct customer clusters based on their booking patterns, spending habits, reliability, and proceed to outline marketing profiles for each of those clusters.

## Repository structure
- `BCWDS_hotel_segmentation_code.ipynb` - main notebook code with full pipeline and model assesment
- BCWDS_hotel_segmentation_report.pdf - full written report in pdf
- `Case1_HotelCustomerSegmentation.csv` - source data
- `data_tourism_lisbon.csv`- external data used

 
## Technical Approach

| Phase              |	          Techniques                                                                                                                             |
|--------------------|-------------------------------------------------------------------------------------------------------------------------------------------------- |
|Data Preparation    | Duplicate detection; Advanced aggregation to identify unique clients; No-show detection; Data Incoherences correction; Missing values imputation  |
|Feature Engineering | Behavioral & Value-Based Features; Customer Reliability & Spending Metrics; Binning, Derived Features and Aggregations                            |
|Model Selection     | 	K-Means                                                                                                                                          |
|Evaluation	         | 	Silhouette Score, Elbow Method                                                                                                                   |



## Key Challenges
- Lack of critical context (e.g., hotel capacity, star rating, time-series data for seasonality) which required significant assumptions
- Creating meaningful derived features that correctly capture the underlying relationships between existing data
- Algorithm selection considering tradeoffs

 
## Results
- **4+1 Clusters** - Adequately interpreted for business value

## Key Observations and Future Improvements
- Clear trade-off between booking lead time and customer value
- Start collecting crucial missing KPIs like guest satisfaction and promotion usage.
- Incorporate Time-Series Data to capture seasonality and trends
  
## Authors
- André Lourenço
- Emir Kamiloglu
- Manuel Andrade
- Rute Teixeira
- Victor Silva

### More details on https://rutemteixeira.github.io/generic/p5-hotel-strategy.html
