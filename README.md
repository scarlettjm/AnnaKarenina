# Anna Karenina: Tolstoy by the Numbers

This project uses computational text analysis to explore *Anna Karenina* by Leo Tolstoy. Using R, the analysis extracts patterns in themes, characters, emotions, and environmental imagery by applying natural language processing (NLP) techniques.

## Overview

The goals of this project include:

- Identifying frequent mentions of characters, colors, foods, settings, and animals
- Performing sentiment and emotion analysis
- Visualizing findings using bar plots, histograms, and word clouds
- Exporting processed results to Excel for further exploration

## Tools & Libraries

The analysis was conducted using the following R libraries:

- [`tidyverse`](https://www.tidyverse.org/)
- [`tidytext`](https://cran.r-project.org/web/packages/tidytext/index.html)
- [`ggplot2`](https://ggplot2.tidyverse.org/)
- [`wordcloud`](https://cran.r-project.org/web/packages/wordcloud/index.html)
- [`openxlsx`](https://cran.r-project.org/web/packages/openxlsx/index.html)
- `RColorBrewer`
- `afinn` and `nrc` sentiment lexicons (via `get_sentiments()`)

## Data

- The dataset consists of the full text of *Anna Karenina* in `.txt` format.
- Additional manually created lists for analysis:
  - Character names (e.g., "Anna", "Levin", "Vronsky")
  - Food and drink items (e.g., "bread", "wine", "soup")
  - Animals (e.g., "horse", "dog", "cow")
  - Colors (e.g., "red", "white", "black")
  - Events (e.g., "ball", "marriage", "death")
  - Sounds (e.g., "laugh", "whisper", "thunder")
  - Settings (e.g., "Moscow", "country estate", "theater")

## Process

1. **Text Loading and Cleaning**  
   - Load the `.txt` file  
   - Convert text to a tidy tibble  
   - Tokenize into words using `unnest_tokens()`  
   - Remove stopwords and incomplete lines  

2. **Keyword Frequency Analysis**  
   - Count word occurrences in each predefined category  
   - Generate bar plots for each thematic group  

3. **Sentiment & Emotion Analysis**  
   - Use the AFINN and NRC lexicons  
   - Score and visualize sentiment values  
   - Create emotion word clouds and export structured results

4. **Data Export**  
   - Create summary tables for each category  
   - Export all data and charts to `.xlsx` files using `openxlsx`

## Outputs

- Bar charts for mentions of food, animals, colors, events, sounds, and settings
- Histograms of sentiment scores
- Word cloud visualizations of emotion words
- Excel workbooks with structured category data and embedded plots



## How to Use

1. Clone or download this repository
2. Open the `.Rmd` or `.R` script in RStudio
3. Ensure `anna.karenina.txt` is in the working directory
4. Install required libraries if necessary
5. Run the scripts to reproduce analysis, generate charts, and export results

## Credits

- Text source: [Project Gutenberg – *Anna Karenina*](https://www.gutenberg.org/ebooks/1399)
- Analysis and Visualization by: Scarlett Moldovan



