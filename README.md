# MoodysGraphGPT
Fork of GraphGPT Project for Moodys

# GraphGPT (Microsoft Graph Co-Pilot v_0.75)

## What is it?
GraphGPT CoiPilot is a helpful AI Assistant made to assist Microsoft CSA's deliver better proactive support "delivery experiences" to our SfMC customers by enhancing the CSA's ability to provide real-time responses to highly technical questions and proactive deliverables.

## Demo Video
***coming soon

## How it Works
GraphGPT is a system of three major components:
1. Teams Bot with Tab component (*coming soon)
2. 1 or more Azure OpenAI deployment(s) built for GraphGPT uses cases
3. User/Use Case Specific Tools (i.e: Collection of external LLM/ AI Tools / Other automation solutions)

GraphGPT is a Teams App with the followimg Teams App Features enabled:
1. Teams Bot with Tab component to configure app settings 
   -Teams AI Libary verison currently in development (*coming soon)
2. Message Extension to expose multiple options and interactions with the bot while remaining in the same conversation window | Send any message in teams to bot
3. Tab to expose the App dashaboard view(s) and Use Case specfic tools in addition to a webchat view of the bot

GraphGPT is a Teams Bot built to provide a SfMC CSA the shortest [Time to Accurate Response: A short enough amount of time to provide a certifable response to a customer ask while on call] using generative AI tools in context of Microsoft Graph API. 

Because of known caveats concerning LLMs & generative AI technology in how they handle API related tasks, MS Graph quereies when using Generative AI tools are often in accurate or taken an unreasonable amount of time to verify the the accuracy of the response. This project aims to resolve these main blockers toward consuming geneative AI tools to assist our customers with MS Graph asks.

To do this, this project use the compoents listed above as follows:
1. Graph GPT Teams Bot: Uses the Microsoft Bot Framework and Teams Toolkit V5 to chat with the GraphGPT Azure OpenAI Deployment
  Graph GPT Teams Tab: Overall application configuration and settings, multi tool chat view (i.e ChatAll / LibreGPT)
2. Graph GPT Azure OpenAI Deployment: MS Graph Data added as part of an Azure Cognitive Search Resourch and Index
3. User/Use Case Specific Tools: (PrivateGPT to incorporate user writing style'd emails, User specific data dependent use cases, GorillaLLM, Aider, etc.)

To resolve overall common ease of use conerns with AI Tools:
-main point of access: teams bot, so users do not have to leave teams, and message history is more easily managed
-List out common uses cases of tools
-List out example questions
-Adaptaive card buttons to load system prompts and prompt templates

To resolve response speed concerns commons with large LLM based tools:
-Concurrent reponse requests to multiple AI tools
-Conccurent reponse requests to multilple search engines/research tools
-Automatic response regeneration 

To resolve response accuracy conerns with Generative AI tool consumption in Production:
-Automatic "hallucination" check via validation of the attirbution link HTTP Response code
-For Azure OpenAI: 
-Automatic response regeneration 
-Concurrent reponse requests to multiple AI tools


### Project High Level Goals:

- Cost effective to scale organization wide

- [SfMC On-Call Ready] (*add link to on call playbook)

- Modular design to addapt this projet to other MSFT Products/SfMC Teams  ("SfMC Co-Piiot" , "CSA Co-Pilot)

- Serve as a feasbility excerise in using AI tools to quickly "ramp up" on highly technical skills and ensure required skills for various Account custom solutions are maintained within SfMC timelines



### Overall Project Requirements:

- Time to Accurate Response: Short enough to provide certifable responses to customer asks while on call  (TtAR is recorded and tracker per user interaction OR human approval submission)

- Human approval process and logging of AI generated responses to customers (approvals saved in account Knowme/OneDrive/Account Team post/Teams sharepoint)

- Automatic System and User prompt configuration
  
- Automatic "memory bank" insertion

- Automating repitive Generative AI best practices for response accuracy:
  multiple reprompts conccurently with multiple agents,
  
- HTTP response code validation, Link validation, on all attribution links
  
- automated responses comparison betweeen regenerations and betweenn models and prompt verivations
  
- include (text snippet, embedding locator, screenshot, .md table) of the model's added data explicity documenting the correct answer(s) [existing problem with Azure OpenAI and TPrompt]
  
- Auto suggesting or implementing as necessary: TOC,COB prompting/AutoGPT functionality for high level problem solving & Scoping

- Mission Critical reliability of  dependent service(s) 

-Maintains MSFT Generative AI compliance requirements (*add link)

- Maintains Azure Subscription compliance requirements (*add link)

- No MSFT user data or Internal MSFT data leave MSFT Corp Managed tenant compliance boundary (*add link)



## Under the Hood (explaining the files and directory structure of this GitHub Repo/Fork)

## Under the Hood (explaining the code)

### File and Directory Structure of the Repo

### Teams Bot
-until message extension is up, use command bot commands to bot settings and basic configuraiton without the tab

### Teams Tab(s)

### Message Extension

### Adaptive Cards

### Teams App Manifest

### Azure Resources

## Completed
- power automate flow initial test complete
- Began with this github sample (https://github.com/leeford/teams-openai-bot) [Fork Link]
- Also experimented with this sample (https://github.com/formulahendry/chatgpt-teams-bot) [Fork Link]
- tested azure open ai js libary <---list out issues here>>
- Began with Bot & SSO ()
- Teams Bot using Azure OpenAPI API w/Axios Library
- attempted to use the teams AI libarbary to get responses from the GraphGPT Azure OpenAI deployment
- sucessfuly became certified as a Teams app developer

## Current Status
- Creating new Teams app beginning with a Bot using Azure AI Library told hold a conversation with the GraphGPT Azure OpenAI deployment, using a Teams app sample project


## Feature/Release Roadmap

1. MVP for testing (include name of and link of fork with feature being worked on)
  MVP requirements:
  *Deploy an Azure OpenAI deployment with all Graph and relevant docs/data added to the deployment
  *Create Teams Bot project for local debug testing by testing group using Azure AI Library
  *Display the response of  from user's OpenAI Deployment of a 16K model using and OpenAI API Key, from a users input into the bot
  *Display the response from the Graph GPT Azure OpenAI Deployment, from a users input into the bot
  *Displays both reponses in adapative cards simultaneiously


2. v_0.80 Release
-Chat completion generation
-Prompt library management
-Meomry bank management
-Message Extension
-Tab for bot settings


3. v_1.0 Release
-Persistent memory
-Automatic attribution HTTP Response code validation
-Tab app
--Claude for 100K Memory Bank filled prompts
-Bing Chat or Google Bard
-Teams App configuration tab

4. v_1.+ Release(s)
-Lorem Impsum
-List out other features from the roadmap in OneNote
-Cost management / Cost per response



## Setup Instrucctions (Minimal Path to Awesome)


### Configuration


### How to use this project (INTERNAL)

### How to use this project (EXTERNAL)

### Known Issues
- claude usuage limits
- bard usuage limits
- bard cookie disablement
-



------------------------------------------------------
### Github Links
[Title](https://github.com/leeford/teams-openai-bot)
[Title](https://github.com/formulahendry/chatgpt-teams-bot)
[Title](https://github.com/microsoft/teams-ai)
[Title](https://github.com/OfficeDev/teams-chef-sample)

### Youtube Links
[Title](https://www.youtube.com/watch?v=PtdOdYax84A)
[Title](https://www.youtube.com/watch?v=naNkZ6W1GHU)

### All other Links
[Title](https://learn.microsoft.com/en-us/microsoftteams/platform/bots/how-to/teams conversational ai/teams-conversation-ai-overview)
[Title](https://platform.openai.com/docs/libraries/node-js-library)




## AI DISCLAIMER 1
- Human approval required

## Use Cases


## Demo Video



## How it works

- Azure OpenAI + congtive & semantic search w/Azure Blob storage of MSFT internal docs	

- Codex, Aider, GPT Engineer, Gorilla, (Co-Pilot X w/power automate desktop?) for PS script generation  (potentially python/javascript refactor to PS)(possibly | use Claude 100K for refactoring
  https://github.com/ShishirPatil/gorilla

- Aider wCtags on MS Graph PS Script libary

- Gorilla fine trained moddel  of MS PS Graph Script library 
  - https://www.youtube.com/watch?v=8AqQBPI4CFI
  - Project Website: https://gorilla.cs.berkeley.edu/
  - Github Repo: https://github.com/ShishirPatil/gorilla
  - Google Colab: https://colab.research.google.com/dri...


- Bing chat and Google Bard for internet connected searches

- Bing Chat & ChatGPT 4 webchat for psuedo code generation

- Bing Chat & ChatGPT 4 webchat for for problem solving, question formulation

- Chapt GPT 4 via 3rd party API for plug in access

- Private GPT for private documents (emails, onenotes, personal docs)

- Dediccated model for content generation (emails, summaries)

- Claude for 100K Memory Bank filled prompts
https://openrouter.ai/docs#models

- Aure OpenAI for whisper AI

- ??Solution for automated meeting notes and summaries??


## Setup Instrucctions (Minimal Path to Awesome)


### Configuration


### How to use this project (INTERNAL)

### How to use this project (EXTERNAL)

## Testing procedure and Results

- questions for internatl teams chnnels
- questions via teams or emails from customers
- Learn and Dev communities forums, uses questions from here
- Githu and stackoverfflow issues boards
- Activate Graph API questions registers
- CSS Graph API cases

## FAQs

## Documentation
- point to azure devops project
- include instructions to increase Azure quota with new subscription

## Known Issues
- claude usuage limits
- bard usuage limits
- bard cookie disablement
-


## Roll Credits


## AI DISCLAIMER 2
Human approval required
