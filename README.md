# Lotus
Hack Western 9 - November 2022

## Instructions
1. Clone Repository
2. Install all the dependencies
- pip install -r requirements.txt
- pip install cohere
- pip install numpy

3. Run Web App:
- To activate virtual environment: . venv/bin/activate
- To install Flask: pip install Flask
- To run: python3 app.py

## Inspiration
We were inspired by Cohere's Conversant API (specifically creating personas) and Cohere's Grounded QA API. These APIs create conversational AI and provide factual resources, respectively, and we wanted to combine them to create a friendly and informative resource. This is how we came up with our idea, Lotus: a compassionate web app that allows teenage girls to ask uncomfortable questions about growing up.

## What it does
This web app prompts a user (target market is teenage girls) to ask uncomfortable questions about puberty, sexuality, dating, body image, feminine hygiene, periods, and more. The web-app outputs informative answers about these topics in language that will resonate with these girls and have the tone of a compassionate friend or older sister to reassure them through their worries.

## How we built it
Design and Front-End: We first designed our UI in Figma and then built the front-end with HTML, CSS, and Javascript files and used Bootstrap templates.

Web Framework: We connected the front-end and back-end with a Flask framework since the back-end was in Python. We loaded the first page in Flask, and then made a POST request with user input in a textbox to one of the functions in the answer.py file.

Back-End: Originally, we played around with the Conversant API and the Grounded QA API. Both of these APIs are written in Python. We cloned the Conversant API and created a Compassionate Friend persona in a config.json file. In the config.json file, we provided questions and answers on how to respond to different female questions like sexuality, periods, dating, feminine hygiene, and more. We ran the demo through a streamlit app that interacted with the user and had a very friendly conversation, as if the AI was your big sister.

With the cloned Grounded QA API, we tested the basic functionality of having the API search top Google results for factual answers to the user's questions. We then added two input files that modified the tone of the API to make it more friendly and conversational.

Although we demoed both, the Grounded QA API back-end is connected to the front-end. In the future, we would want to connect the Conversant API with the Grounded QA API to add a persona to the factual information.
