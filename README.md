#React chatbot 
This app for chatbot build with React using the `react-chatbot-kit`.

## Table of contents.
1. [Installation](#installation)
2. [Usage](#usage)
3. [Customization](#customization)


**#Installation**

To get started with this project,follow these steps:
1.Create app:
npx create-react-app my-app

2.Open file
cd my-app

3.Start the development server:
npm start

4.Open you browser and navigate to http://localhost:3000


**Usage**
Here's how to use the chatbot in my React application:

1.Import the Chatbot component:
import Chatbot from 'react-chatbot-kit'
import 'react-chatbot-kit/build/main.css'
import config from './config';

2.Set up the chatbot in my component:
function App() { 
  return (
    <div className="App">
      <header className="App-header">
        <Chatbot
          config={config}
          actionProvider={ActionProvider}
          messageParser={MessageParser}
          headerText='LSEG chatbot'
          placeholderText='Please pick an option'
        />
      </header>
    </div>
  );
}

export default App;

**Customization**
To customize the chatbot, I modified the configuration and added my own message parser and action provider.

**1.Configuration Example:**
const botName = 'LSEG chatbot';
const message = "Hello! Welcome to LSEG. I'm here to help you."
const config = {
  botName: botName,
  initialMessages: [
    createChatBotMessage(`${message}`, {
      withAvatar: true,
      delay: 500,
      widget: 'menuSelected',
    }),
    
  ],
}
**2.Action Provider**

Create a file named ActionProvider.js

**3.Message Parser**

Create a file named MessageParser.js

**4.CusttomMessage**
  Create a file named CusttomMessage.js where the data from the first table is stored.

**5.Stock**
 Create a file named Stock.js where the data from the second table is stored.

** 6.FinalView**
  Create a file named FinalView.js , data from the third table .
 
