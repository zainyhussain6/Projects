# Sentiment Analysis Project

## Overview
I wanted to understand a little more about how sentiment analysis worked as I was totally oblivious to the inner workings of text analysis. I was aware of two libraries that were commonly used: **TextBlob** and **NLTK**. I did some research on how they worked and figured that a good way to test them out would be to get **IMDB reviews of the new Star Trek show**. Web scraping is also something I had never done in practice, so I figured it was a good opportunity to also get an idea of how that was done.

## Challenges
The main challenge was getting the web scraping tool to precisely capture the data I wanted and in the quantity I needed. I used **Selenium** for this purpose, and after a lot of tweaking, I was able to get the data in the desired format. Then it was just a matter of applying the two main **NLP tools** I was experimenting with and plotting the results.

## Outcome
I gained some insight into how the Star Trek show had been received by audiences and critics. Throughout the life of the show, reviews oscillated between strongly positive and strongly negative. However, as the show progressed, not only did interest wane, but reviews also began to become more **neutral**. It is said that any kind of publicity is good publicity, so when viewership begins to drop off and reviews start hovering around neutrality, that's often the death knell for a show.

The **TextBlob** library represented this reality fairly well. During the beginning of the show, sentiment oscillated wildly between positive and negative, indicating strong feelings and high engagement with the show. But as the story progressed, sentiment began hovering closer and closer to neutral, with a slight positive edge.

**NLTK's VADER** is said to be better suited for online text as it captures context and tone more accurately. The positive sentiment trend started off with higher average values and over time became smaller and smaller. The negative sentiment trend interestingly followed a similar pattern. The picture became clearer when looking at the **neutrality score**, as by the end of the show it seemed like most of the comments were neutral, reflecting a lack of passionate engagement that a show needs for repeated viewership.

## Conclusion
Both tools provided interesting insights that seemed to roughly coincide with what my knowledge of the show's perception was. **NLTK** was able to give a more granular picture of the reviews, providing individual metrics for positive, negative, and neutral sentiment. Reading up on the math behind elements like **tokenization** for text analysis was certainly interesting, as was learning the fundamentals of **web scraping**.
