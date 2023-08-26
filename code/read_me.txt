# Project Name - Beyonf News - YouTube Comments Analysis

## Introduction
This repository contains code to perform an analysis of YouTube comments using various APIs and natural language processing techniques. The analysis includes data retrieval, data preprocessing, sentiment analysis, network analysis, and visualization of results. This README file provides instructions on how to execute the code in the correct order. Please make sure to adjust file paths as needed for your local machine for data paths.

## Getting Started

1. **Clone the Repository:** Start by cloning this repository to your local machine using the following command:
    ```
    git clone https://github.com/peersal/Beyond-News.git
    cd Beyond-News
    ```

2. **Install Dependencies:** Ensure you have the required dependencies installed. You might want to set up a virtual environment before installing dependencies.

3. **API Keys Setup:**
    - **YouTube Data API:** Obtain a YouTube Data API key by following the instructions [here](https://developers.google.com/youtube/registering_an_application).
    - **Perspective API:** You'll need an API key to use the Perspective API for toxic comment analysis. Obtain it [here](https://www.perspectiveapi.com/).
    
    Once you have the keys, replace them in the appropriate code files.

## Execution Order

Follow these steps to execute the code in the correct order:

1. **code_data_request:** Run this script to utilize the YouTube Data API for retrieving comments data.
    ```
    anaconda code_data_request.ipynb
    ```

2. **code_final_data:** Run this script to convert the retrieved data into CSV format.
    ```
    anaconda code_final_data.ipynb
    ```

3. **code_datacleaning_wordcloud:** Run this script to clean the data and generate word clouds.
    ```
    anaconda code_datacleaning_wordcloud.ipynb
    ```

4. **code_tox_score:** Run this script to utilize the Perspective API for obtaining toxicity scores of comments.
    ```
    anaconda code_tox_score.ipynb
    ```

5. **code_sentiment:** Run this script to perform sentiment analysis using the BERT model.
    ```
    anaconda code_sentiment.ipynb
    ```

6. **code_network:** Run this script to perform network analysis on the comments.
    ```
    anaconda code_network.ipynb
    ```

7. **code_dictionary:** Run this script to perform dictionary-based analyses on the comments.
    ```
    anaconda code_dictionary.ipynb
    ```

8. **code_plots:** Run this script to generate plots and visualizations based on the analysis.
    ```
    anaconda code_plots.ipynb
    ```

## Customization
Feel free to customize various parameters, such as API endpoints, file paths, and analysis methods, to suit your needs.

## Conclusion
By following these steps, you'll be able to execute the code and perform a comprehensive analysis of YouTube comments. If you encounter any issues or have questions, please don't hesitate to reach out.

Happy analyzing!
