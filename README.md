# LargeScaleDataCollection

As part of a political event coding pipeline, students are going to design a spark based preprocessing tool that does the following steps:
  1. Collects data by crawling a set of spanish news websites on a daily basis.
  2. Extracts the main content of the article and related metadata (i.e headline, author, date
published)
  3. Process the extracted content with and generate universal dependency parse for each sentences within the content (use Apache Spark here)
  4. Store the collected data and processed data in a way compatible with event coder’s input format in MongoDB
  5. Running some deduplication algorithm at content level. (Comparing two articles from different urls and find out whether they cover the same story)

There are several software packages that can be used at different steps. Details will be provided upon request. Key challenges will be design a crawler such a way that can avoid duplicates, implementation of UD-parse generation in streamlined manner, Setting up apache kafka for inter-module communication and content level deduplication.

Input: Set of seed URLs to spanish news sources

Output: Stored data in MongoDB including raw text and processed ones. Structure outline will
be provided later.
