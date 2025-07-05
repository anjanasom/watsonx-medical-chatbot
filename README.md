# watsonx-medical-chatbot

This project was created using IBM Watsonx assistant and Watsonx.ai. The chatbot takes the user's medical symptoms as input and recommends the appropriate medical department to consult (example: Cardiology, Nephrology, etc.).

## Objective
To classify user's symptoms using a simply conversational interface powered by a large language model.

## Tools Used
- IBM Watson Assistant
- IBM watsonx.ai (granite-3-3-8b-instruct model)
- Prompt Lab

## How It Works
1. User interacts with th medical assistant chatbot
2. When chatbot detects a need for medical help, it prompts the user for symptoms
3. User enters their symptoms
4. Assistant collects the input and calls watsonx.ai through extension
5. It instructs the model to return only the department after few shot prompting
6. Response is displayed to the user

## Screenshots
See the `/screenshots/` folder

## Prompt Example
See `prompt.txt`
