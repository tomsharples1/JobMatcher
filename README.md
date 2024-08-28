# JobMacther
This is a personal project aimed towards helping graduates like myself land their first job. The premise is simple, you take your CV and a job description and create a percentage match and the job with the highest percentage match is the best suited to you. During my initial approach, I web scraped job data from Google using SerpApi then used Sci-kit learns cosine similarity function to compare my CV against each job descritpion, then it would output a table ot jobs best suited to me. 

\nI realised that words such as 'the' and 'a' would be counted on both documents but they dont provide any meaning, this lead me to explore NLP to improve the percentage match. This was great, I learnt about tokenisation, lemmitisation and stop words allowing me to clean the text and in theory have a higher percentage match. When I ran the preprocessed text through the cosine similarity algorithm the pecentage match decreased by pretty much 75%. I realised now that although cosine simalarity is good it doens't capture what the words mean, it doesn't understand NER.

\nI then found lots of different text similarity algorithms and settled on using BERT, which is based off the BERT chatbot, and it yielded the best results.

\nThe main take aways from this project is that NLP is really difficult and takes a lot of understanding. The real world positive of this project was that it got me a final interview at Tickermaster ! 

