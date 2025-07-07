# Dietary Compass: Personalized Food Choice Navigator

## Project Overview

The Dietary Compass is an innovative application designed to simplify healthy food selection, automate dietary restriction checking, and educate users about processed foods. With 60% of Americans having dietary restrictions and a growing demand for transparency in food choices, this project aims to address the increasing complexity of processed foods and empower users to make informed decisions.

## Features

The application is built around three core functionalities:

### 1. Healthy Food Finder
*   **Challenge Addressed:** Users struggle to find healthier alternatives and compare similar products effectively.
*   **Solution:** An input-based recommendation system that suggests healthier options based on user input.
    *   **Example:** Inputting "soda" displays options sorted by lowest calorie content, lowest sugar content, and higher nutrition scores.
*   **Key Functions:**
    *   Fetches products by name.
    *   Extracts key nutritional information.
    *   Suggests healthier choices based on calorie count and sugar level.
    *   Provides a nutrition score to indicate overall healthiness.

### 2. Dietary Compatibility Scanner
*   **Challenge Addressed:** Time-consuming ingredient checking and risk of missing important dietary restrictions.
*   **Solution:** Automated ingredient analysis and an instant flagging system.
    *   Cross-references products with user dietary preferences.
    *   Flags allergens, diet incompatibilities, and restricted ingredients.
*   **Key Functions:**
    *   Fetches product details by barcode.
    *   Checks for allergens.
    *   Checks for dietary restrictions.
    *   Allows exploration of up to 10 matching products and specific allergen searches.

### 3. Food Processing Analyzer
*   **Challenge Addressed:** Difficulty understanding food processing levels and limited knowledge of additives.
*   **Solution:** A custom "Processing Score" system and clear ingredient explanations.
    *   Calculates processing scores based on the number of additives, types of artificial ingredients, and processing methods.
    *   Suggests less processed alternatives.
*   **Key Functions:**
    *   Searches products by name and barcode.
    *   Calculates processing scores.
    *   Generates visualizations for processing levels and nutrition (bar graphs for processing score/ingredient complexity, pie charts for nutritional composition).
    *   Utilizes NOVA score (1: Unprocessed/minimally processed, 2: Processed ingredients, 3: Processed, 4: Ultra-Processed).

## Implementation Details

### User Flow
1.  **Input Phase:** Product search, dietary preferences setting, restriction specification.
2.  **Processing Phase:** API data retrieval, score calculation, restriction checking.
3.  **Output Phase:** Results display, alternative suggestions, detailed explanations.

### API Used
*   **Open Food Facts:** Provides access to a crowdsourced database of food products, including ingredients, nutrition facts, labels, allergens, and sustainability scores. Supports JSON, XML, CSV formats and is free to use under an open data license.

### Libraries and Functions
*   **Requests:** For making HTTP requests to APIs.
*   **Time:** For managing time-related operations, potentially for rate limiting.
*   **Json:** For handling JSON data.
*   **Requests_cache:** For caching API requests to improve performance and manage rate limits.
*   **Pandas:** For data manipulation and analysis.
*   **Matplotlib.pyplot:** For creating visualizations.
*   **Typing:** For type hints.

## Extension Proposal & Outcome

### Reference Daily Intake (RDI) Integration
*   **Why:** To provide additional nutritional data and enhance educational content.
*   **What:** Scraped and integrated data from Wikipedia's nutritional tables.
*   **How:** Used web scraping techniques to extract and process data from Wikipedia pages.
*   **Outcome:** Successfully enhanced the application's nutritional database with more comprehensive information.

### Nutrition Facts Label Integration
*   **Why:** To expand data sources and improve the accuracy of nutritional information.
*   **What:** Scraped and integrated data from additional reliable nutrition websites.
*   **How:** Implemented web scraping scripts to fetch and process data from these websites.
*   **Outcome:** Improved the accuracy and reliability of nutritional information provided to users.

## Limitations & Future Work

### Current Constraints
*   API data completeness varies by region.
*   Limited to packaged foods.
*   Processing score needs refinement.

### Technical Challenges
*   Ingredient disambiguation.
*   Regional product variations.
*   Real-time data updates.
*   Data consistency across different sources.
*   Web scraping limitations (dynamic content, changes in web page structures).
*   API rate limits.

### Future Enhancements
*   **Nutrition Calculator:** Calculate calories, fats, carbohydrates, and proteins in a meal; plan balanced meals.
*   **Sustainability Analyzer:** Find products with smaller environmental impacts.
*   **User Interface:** Enhance for better navigation and readability.
*   **Expand Data Sources:** Incorporate more reliable and diverse data sources.
*   **Improve Data Processing:** Enhance data cleaning and processing techniques.
*   **Mobile Application:** Develop a mobile version for broader accessibility.
*   **Machine Learning:** Implement machine learning algorithms for personalized recommendations.

## Team

*   Via Lin
*   Mahnoor Shahid
*   Jiyeon (Jenna) Woo
*   Kaylyn Nguyen
