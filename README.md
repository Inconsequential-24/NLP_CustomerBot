**NLP-Powered Chatbot for Loan Renewals, Restructuring, and Cross-Selling**

This project is a prototype for an AI-powered chatbot designed to assist customers with loan renewals, restructuring options, and cross-sell recommendations. The chatbot leverages Natural Language Processing (NLP) to understand user queries, analyze sentiment, and maintain context throughout conversations. It is built using Python, Rasa, and TextBlob, and is designed to run in Visual Studio Code (VSCode).

## **Table of Contents**
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Customization](#customization)
- [Contributing](#contributing)
- [License](#license)

## **Features**
- **Language Understanding**: Uses NLP to understand and process customer queries.
- **Sentiment Analysis**: Analyzes customer sentiment to tailor responses appropriately.
- **Contextual Awareness**: Maintains conversation context to handle multi-turn interactions.
- **Custom Actions**: Includes custom actions for sentiment analysis and personalized responses.
- **Multi-channel Deployment**: Can be deployed on various platforms such as websites, mobile apps, and messaging platforms.

## **Installation**

### **Prerequisites**
- Python 3.6+
- Visual Studio Code (VSCode)
- Virtual Environment (venv)

### **Steps**
1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/nlp-powered-chatbot.git
   cd nlp-powered-chatbot
   ```
2. Create and activate a virtual environment:
  ```bash
   # On Windows
    python -m venv chatbot-env
    chatbot-env\Scripts\activate
    
    # On macOS/Linux
    python3 -m venv chatbot-env
    source chatbot-env/bin/activate
   ```
3. Install the required packages:
   ```bash
   pip install rasa textblob spacy
    python -m spacy download en_core_web_sm
   ```
4. Initialize and train the Rasa model:
   ```bash
   rasa init
    rasa train
   ```
###**Usage**

1. **Running the Chatbot**
-Start the Rasa action server:
   ```bash
    rasa run actions
    ```
2.	**Start the Rasa chatbot:**
       ```bash
       rasa shell
       ```

4.	**Interact with the chatbot:**
- Open the terminal and start a conversation to test the chatbot’s functionalities, such as handling loan renewals, restructuring, and cross-selling.

Example Interactions

-Loan Renewal: “I want to renew my car loan.”
-Sentiment Analysis: “I’m really frustrated with my current loan terms.”
-	Contextual Conversation: “Can I renew my loan? I want it for 12 months.”

