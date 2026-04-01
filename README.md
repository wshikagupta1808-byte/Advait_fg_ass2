# Shakespearean Sentiment Analyzer
A lightweight rule-based sentiment analyzer designed for Shakespeare-style text.
It scores sentences using custom lexicons, negation handling, intensifiers, and punctuation-based emotion boosting.

## Working 
- **Lexicon Scoring:** Positive & negative Shakespearean words (e.g., love, noble, vile, foul) have predefined sentiment values.
- **Negation Flip:** Words like not, never, no invert the sentiment of the next scored word.
- **Intensifiers:** thrice, very, most double the strength of the upcoming word.
- **Punctuation Boost:** Words containing (! or ?) receive a 1.5× emotional boost.
- **Conjunction Reset:** but, yet reset the running score to model tone shifts.

The final sentiment is classified as Positive, Negative, or Neutral based on the cumulative score.

## Example Tested Sentences
- “I love thee thrice more than life!”
- “Thou art not fair, but vile!”
- “Hell is empty and all the devils are here.”
- “Parting is such sweet sorrow.”
- “To be, or not to be: that is the question.”

## To Run 
- save the script as : shakespeare_sentiment.py
- run it using :
      bash
python shakespeare_sentiment.py   
