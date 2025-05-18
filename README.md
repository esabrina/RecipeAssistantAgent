# Personal Recipe Assistant Agent
> A multi-agent system for generating and adapting meal recipes
## Project Overview
This project develops a conversational Artificial Intelligence agent designed to assist users, understanding natural language requests, in discovering and adapting culinary recipes. Leveraging the Google Gemini SDK, the agent interacts with users via a text-based chat interface, taking into account available ingredients and dietary restrictions. As a bonus functionality, it also explores adapting recipes for Airfryer cooking, promoting healthier preparation methods. For more information, [see](Recipe_Assistant_MVP_Project.pdf) the complete project file.

The project is implemented in Python within the Google Colab environment, demonstrating the use of large language models for practical, interactive applications.
### Multi-Agent Structure:
While the user interacts with a single assistant, the internal logic is structured conceptually as a multi-agent system orchestrated by the main code. Different parts of the process, such as understanding the user, generating the base recipe, and adapting for restrictions or Airfryer, can be seen as distinct "agents" or modules working together. This approach demonstrates how complex tasks can be broken down and handled by specialized components, even when powered by a single underlying model like Gemini.

### Features Highlights (MVP)
The Minimum Viable Product (MVP) of this project focuses on the core conversational and recipe generation/adaptation capabilities using the Google Gemini SDK. Key aspects include:
- Natural Language Processing (NLP): Understanding user inputs regarding ingredients, restrictions, meal types, and adaptation requests.
- Recipe Search and Creation (Simulated): Utilizing the generative capabilities of the Gemini model to create recipes based on the provided ingredients and criteria, as the MVP does not include an external recipe database or web scraping.
- Simple Recipe Adaptation: Offering basic ingredient substitutions based on dietary restrictions.
- Airfryer Adaptation (Bonus): Providing specific instructions to adapt a generated recipe for cooking in an Airfryer.
- Text-Based Interface: Interaction occurs through a simple chat interface within the Google Colab notebook.

## Technologies Used
- Programming Language: Python
- Development Environment: Google Colab
- AI SDK: Google Gemini SDK

## How to Run the Notebook in Google Colab
1. Open the Notebook: Navigate to the project repository on GitHub (https://github.com/esabrina/RecipeAssistantAgent) and click on the Recipe_Assistant_MVP.ipynb file.
2. Open in Colab: Click the "Open in Colab" button at the top of the notebook preview on GitHub. This will open the notebook directly in your Google Colab environment.
3. Configure Your Google API Key:
   - You need a Google API Key to use the Gemini SDK. If you don't have one, you can obtain it from the Google AI Studio.
   - Securely add your API key in Colab: Click the 🔑 icon in the left sidebar of your Colab notebook. Add a new secret with the name GOOGLE_API_KEY and paste your API key in the "Value" field. Ensure the "Notebook access" is enabled for this secret.
   - The code in the notebook is configured to read the API key from Colab Secrets.
4. Run the Code Cells:
   - Execute each code cell in the notebook sequentially.
   - The first cells will install necessary libraries and configure the API key.
   - The subsequent cells initialize the Gemini model(s) and the chat interface.
   - The final cell contains the main interaction loop.
5. Interact with the Assistant: Once the assistant is initialized, you will see a prompt asking for your input. Type your recipe requests (e.g., *"I have chicken, broccoli, and rice. I want a gluten-free lunch for 2 people and I want to adapt it for the Airfryer."*) and press Enter.Exit: Type exit in the chat to end the conversation.
## Contributing
If you'd like to contribute to this project, please feel free to fork the repository and submit a pull request.
