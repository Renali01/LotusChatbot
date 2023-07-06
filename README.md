# Lotus
Hack Western 9 - November 2022
Won Cohere's Honourable Mention!

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

## Instructions - How to Run
1. Clone Repository
2. Install all the dependencies
- pip install -r requirements.txt
- pip install cohere
- pip install numpy

3. Run Web App:
- To activate virtual environment: . venv/bin/activate
- To install Flask: pip install Flask
- To run: python3 app.py

## Demo
### Welcome page
![image](https://github.com/Renali01/lotus2/assets/59395990/1f4be040-7f5f-4621-ba58-529405c8958c)

### Asking Lotus a question
![image](https://github.com/Renali01/lotus2/assets/59395990/e2de3df2-c2d8-41f6-a9db-0094c8d0fbf2)

### Having a conversation with Lotus
![image](https://github.com/Renali01/lotus2/assets/59395990/e2687d8a-2e71-44fd-9b5e-aafeac034ed6)

### Asking a follow-up question
![image](https://github.com/Renali01/lotus2/assets/59395990/5fce6287-a33c-457f-af71-19b0422bb7b2)

### Continuing conversation without prior context
![image](https://github.com/Renali01/lotus2/assets/59395990/fff315d8-e135-4a71-a415-b6b4639485d5)

