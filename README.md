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

## Assistant Export (Watsonx Assistant)
This project includes a full exported snapshot (`v1.0.json`) of the IBM Watson Assistant used in this chatbot.

- Path: `assistant_export/v1.0.json`
- It contains: Actions, steps, session variables, and watsonx.ai extension configuration
- Created via: `Create Version` (not published)

### Import Instructions
To re-import this assistant in your own Watson Assistant environment:
1. Go to Watson Assistant dashboard
2. Click “Import Assistant”
3. Upload the `v1.0.json` file
4. Reconfigure your watsonx.ai API credentials and extension setup

**Note:** The export does *not* include sensitive keys or tokens.

## Screenshots
See the `/screenshots/` folder

###Contents:
- chatbot_greet shows the overall preview of how the chatbot looks and greets the user.
- promptLab_prompt and promptLab_generated show the prompt engineering logic
- SeeWhatIDo_flow contains the assistant flow of the 'What do I do' action
- RecommendMedicalDepartment_flow contains the assistant flow of the 'Recommend department' action
- recommendDepartment_action_1, 2, and 3 shows an example interaction between the user and chatbot for collecting symptoms and recommending the appropriate department
- whatDoIDo_action_1, 2, and 3 shows an example interaction between the user and chatbot as it explains its purpose

## Prompt Example
See `prompt.txt`
