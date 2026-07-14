# How Diverse Were the Lyrics Across Chris Cornell's Musical Career?

## What I hoped to accomplish

I wanted to try analyzing text with natural language processing. I also wanted to practice asking more direct questions about the data than I did with my first project.

## Overview of Data Analysis Process

- I used the Genius API to retrieve lyrics from Chris Cornell's solo and band albums. 

- I then made all words lowercase and then used the spacy library to create a cleaner set of lyrics that removed stop words and vocalizations. I also had to remove certain words from spacy's default stop word list. For instance, I kept all pronouns because I wanted to answer questions regarding pronoun usage. I also kept in negative words like "not" and "never."

- I also played around with keeping lyric tags like "chorus", "intro", and "outro," and I uploaded that jupyter notebook to this repository. I had thought they would be helpful when looking at n-grams, but because I didn't include n-grams in my final project, I decided to remove these labels. 

- I initially used Counter to try to answer my questions about pronoun usage but I revisited to count and categorize (first-, second-, and third-person) programmatically and with the help of ChatGPT. 

- I then focused my question on lexical diversity/unique word counts, which I answered using the nltk library.

## Skills Used and Key Learning Moments

- I learned about new libraries and APIs for this project and had some practice using them. 

- Tokenization can make it tricky to deal with contractions. 

- Just when I thought I was done cleaning, I would catch new errors as I scrolled through the lyrics. One thing that was hard to catch were all the different vocalizations. 

- I initially wanted to do top n-grams by album, but the ones that surfaced were kind of boring.

- I learned how to reshape some data to create range charts. 

- I had to reframe my initial narrative from "Chris Cornell's lyrics" to "lyrics associated with Chris Cornell" because, at least to my untrained eye, the Genius API doesn't provide a structured songwriting credit for each song. Looking back, I should've taken more time to understand the metadata before making assumptions and moving forward.

- I realized I was doing a lot of things manually, like when I first counted the different pronouns used in each album. I revisited those questions and tried to answer them programmatically. 

## What I Wanted to Do

- I wanted to count instances of grammatical moods, mainly imperative and interrogative, just as a fun exercise but also because Cornell seems to sing a lot of imperatives and ask questions. While it was straightforward enough to keep in the question marks, identifying and counting the imperative felt like it would require more manual work than I had the time for. 
- I was able to count how many questions were asked per song and per album, but I didn't think that question alone was intersting. I wanted to answer "What questions does he ask?" I made initial attempts to extract those but moved on in the interest of time. 
- I was also interested in how language transitions from verse to chorus, but I didn't have time to research an approach. 
