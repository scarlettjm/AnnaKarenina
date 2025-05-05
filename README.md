Anna Karenina: Tolstoy by the Numbers

This project explores Anna Karenina by Leo Tolstoy using computational text analysis in R. Through natural language processing (NLP) techniques, it investigates recurring themes, character mentions, emotional tones, settings, and other literary elements.

Tools & Libraries Used

tidyverse & tidytext – data wrangling and text mining
ggplot2 – data visualization
wordcloud, RColorBrewer – word cloud generation
openxlsx – exporting analysis to Excel
afinn, nrc – sentiment and emotion lexicons

Dataset

The analysis uses the full text of Anna Karenina, available as a .txt file.

Analysis Features

Tokenization: Breaks the novel into individual words.
Entity Extraction: Tracks mentions of:
Characters (Anna, Vronsky, Kitty, Levin, etc.)
Settings (Moscow, train station, etc.)
Events (marriage, affair, death, etc.)
Colors, sounds, food, and animals
Sentiment Analysis:
AFINN lexicon for numeric sentiment scoring
NRC lexicon for emotion classification (e.g., joy, anger)
Visualizations:
Frequency bar charts for themes
Sentiment histograms
Word clouds for emotional tone
Excel Export: Key datasets and plots exported to .xlsx for further exploration

Example Visuals

You’ll find:

Bar Charts of food, color, and sound mentions
Histograms of sentiment score distribution
Word Clouds based on NRC emotion words

Project Structure

 anna-karenina-analysis/
├── anna.karenina.txt              # Text of the novel
├── anna_karenina_analysis.xlsx   # Compiled data outputs
├── scripts/                      # All R scripts used
├── visualizations/               # Exported PNGs of plots
└── README.md                     # This file
Takeaways

This project uses data to enhance close reading, revealing how literary tropes and emotional tones shift throughout Anna Karenina. It bridges literature and computation to show how stories can be interpreted through a data-driven lens.

To Run Locally

Clone this repo
Open in RStudio
Ensure required libraries are installed
Run each .R or .Rmd script in order

Credits

Text: Project Gutenberg
Author: Scarlett Moldovan
