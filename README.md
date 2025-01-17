# DineLex-Restaurant-Jargon-Lexicon
DineLex is a categorized lexicon of restaurant-related terms (Food, Service, Ambiance, Drinks, Other) created using R and OpenAI's API. Designed to enhance sentiment analysis of reviews, it streamlines text classification for data-driven insights in the hospitality industry.

# DineLex: A Restaurant Jargon Lexicon  

DineLex is a comprehensive and categorized lexicon of restaurant-related terminology, created to enhance sentiment analysis and customer feedback classification for the restaurant industry. Using R and OpenAI's GPT-3.5-turbo API, this project provides a structured dataset with terms categorized into five predefined groups: **Food, Service, Ambiance, Drinks, and Other**.  

## Overview  

Customer reviews are rich with insights, but analyzing large volumes of text manually is time-consuming and often inconsistent. By automating the categorization of restaurant-specific jargon, DineLex serves as a foundational tool for accurate sentiment analysis, enabling businesses to better understand and respond to customer feedback.  

The resulting dataset can be integrated into broader data analysis workflows, including sentiment analysis of restaurant reviews and trend detection over time.  

## Key Features  
- Categorization of 25,000+ restaurant-related terms into **Food, Service, Ambiance, Drinks, and Other**.  
- Workflow automation for handling and categorizing large text datasets.  
- Integration with OpenAI’s GPT-3.5-turbo API for efficient classification.  
- Robust error handling and debugging processes for API integration.  
- Exportable dataset for use in sentiment analysis and other NLP tasks.  

## Project Workflow  

1. **Loading Packages and Data**
   - Loading necessary packages, loading pre-processed data (Yelp review text data tokenized with stop words and duplicates removed and NRC lexicon anti-join preformed). 

2. **API Integration**  
   - Terms were categorized using OpenAI's API, with custom prompts ensuring consistent classification.  

3. **Debugging and Iteration**  
   - Addressed challenges such as handling unexpected categories and refining classifications through iterative code runs.  

4. **Visualization and Insights**  
   - Visualized the distribution of terms across the five categories to validate and interpret results.  

5. **Final Export**  
   - Cleaned and categorized dataset saved as `restaurant_jargon_clean.csv` for future use.  

## Repository Structure  
├── data/
│ ├── excluded_words_with_categories.csv # Raw input data
│ ├── restaurant_jargon_clean.csv # Final categorized lexicon
├── scripts/
│ ├── data_cleaning.R # Data preparation scripts
│ ├── api_classification.R # API integration and classification
│ ├── visualization.R # Visualization scripts
├── visuals/
│ ├── category_distribution.png # Distribution of terms across categories
├── README.md # Project documentation

## Installation and Usage  

### Prerequisites  
- **R (v4.0 or later)**  
- Libraries: `tidyverse`, `httr`, , `gptstudio`, `jsonlite`  

### Steps to Run the Project  

1. Clone this repository:  
   ```bash  
   git clone https://github.com/ptomovic/DineLex-Restaurant-Review-Lexicon.git  
