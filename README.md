# Sentiment Analysis in Home Assistant

Integrate a model for language analysis to interpret people's mood.
To this end, ChatGPT can analyze text/video to identify feelings in terms of both polarity (positive, negative, or neutral) and detected emotion (joy, sadness, anger, fear, surprise, disgust), as well as calculate the magnitude of emotions (by assigning a numerical value to them).
In this way, the result of Sentiment Analysis can be used together with other integrations to:

    - Suggest activities based on mood
    - Suggest music playlists
    - Adjust the tone of Assist's responses
    - Suggest the most appropriate recipe (e.g., comfort food vs. processed food)
    - Choose the type of TV program to watch
    - Combine different inputs together, e.g. with wearable devices for heart rate monitoring or hours slept at night for cross-analysis
    - Create emotional profiles and identify recurring patterns

The model is composed by:
- sensors
- automation
- lovelace card

The model analyzes three different data inputs:
1) Text
2) Video, and you need:
   - LLM Vision integration
   - A camera (if you want to perform video analysis)
3) Conversation, and you need:
   - OpenAI Conversation integration
   - Assist configured
