# PRTCJP-846 Explore Conversational AI Interfaces

## Summary

User Interfaces is the design or the system through which the user and the computer interact. Conversational user interfaces are the user interfaces that help humans to interact with computers using Voice or text. As technology is growing, it is becoming easy through NLU to interpret human voice or text to an understandable computer format. <br />
• Voice assistants allow a person to interact verbally. <br />
• Chatbots where the user interacts with the bots by typing commands or queries. <br />

How to integrate them? <br />
• Used through custom interfaces set up for the web and is ignorant of the model running in the background <br />
• Used through chat applications such as Facebook Messenger, Whatsapp or Twitter <br />
• Used through conversational AI platforms <br />
• Used through custom interfaces with conversational AI platforms <br />

| Library | Pros | Cons |
|---------|------|------|
| Vanilla React Interfaces | the most flexibility in designing the interface and backend | less ready-to-use than the other options and needs more setup |
| Use Existing Chat Applications | ready to use once we have backend running, and users are already familiar with the interfaces/need minimum training | more difficult to bypass fidelity permission |
| ConvAI platforms | ready to use if we already build the model using the platform | have to use a platform |
|Custom UI with platforms | easy to plug in chatbot and flexibility in the custom interface | need to use a platform and need to work on the interface development |

## Vanilla React Interface
### Installation
Tutorial on the implementation is [here](https://www.freecodecamp.org/news/how-to-build-a-chatbot-with-react/) <br />
• Install [Node.JS](https://nodejs.org/en/download/package-manager/) <br />
• From the vanilla_chatbot folder, run `npm install` <br />
• From the same folder, run `npm start`, a browser window will automatically open with the running webpage <br />

See also implementation with [react-simple-chatbot](https://www.npmjs.com/package/react-simple-chatbot) and [demo](https://lucasbassetti.com.br/react-simple-chatbot/#/docs/previous-value) 

## Use Existing Chat Applications
Commonly used applications include: <br />
• Facebook Messenger <br />
• Slack <br />
• Telegram <br />
• Twilio <br />
• Google Hangout Chat <br />
• Microsoft Teams <br />
• Custom Websites <br />

[Example](https://api.slack.com/bot-users) of slack bot configuration.

## Conversational AI Platforms
Conversational AI Platforms provide testing interfaces to manage bots and conversing with existing bots. Some options are: <br />
• Test option on [dialogflow](https://cloud.google.com/dialogflow/es/docs/integrations/aog) <br />
• AWS Lex  <br />
• RASA X  <br /> 

RASA X setup <br />
• pip install [rasa](https://rasa.com/docs/rasa/installation/) <br />
• start a new folder, run `rasa init` to start test model <br />
• (optional) train/configure model  <br />
• install rasactl following [instruction](https://rasa.com/docs/rasa-x/installation-and-setup/installation-guide/) <br />
• inside test model folder, run `rasactl connect rasa (test model name)`, a browser window will automatically open with rasa x interface, more instructions can be found [here](https://rasa.com/docs/rasa-x/installation-and-setup/connect-rasa-to-rasa-x/)

## Use Custom React Interface with ConvAI platforms 
Add chatbot component to custom websites using. Some options are: <br />
• build chatbot component with [aws-lex-web-ui](https://github.com/aws-samples/aws-lex-web-ui) <br />
• build chatbot component with [rasa webchat](https://github.com/botfront/rasa-webchat) <br />

rasa-webchat example <br />
• have rasa model running <br />
• change the port number of socketUrl in /rasa-webchat-bot/src/App.js to the port where the rasa model is running <br />
• run `npm install` and `npm start` in the /rasa-webchat-bot folder to start interface with rasa bot component <br />











