# Basic Chatbot in Python

## Project Overview

This project involves the development of a basic chatbot using Python to interact with users and provide appropriate responses based on predefined intents. The chatbot uses a JSON file containing a set of intents, each with examples of user queries and corresponding responses. The project implements a simple matching algorithm to identify the most relevant response based on user input.

## Features
- Load and process intents stored in a JSON file.
- Preprocess user input by converting text to lowercase, removing punctuation, and tokenizing words.
- Simple intent-matching algorithm based on user input.
- Provide real-time responses through a Command-Line Interface (CLI).
- Consistent user input cleaning for accurate matching with intents.

## Requirements
- Python 3.x
- Modules:
  - `json`
  - `re` (for text preprocessing)

## Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-repo/basic-chatbot.git
   cd basic-chatbot
   ```

2. **Install required modules** (if necessary):
   ```bash
   pip install re
   ```

3. **Add your intents**:
   - Open the `intents.json` file.
   - Modify or add new intents with corresponding user queries and responses.

   Example `intents.json` structure:
   ```json
   {
     "intents": [
       {
         "tag": "greeting",
         "patterns": ["Hi", "Hello", "How are you?"],
         "responses": ["Hello!", "Hi, how can I assist you today?"]
       },
       {
         "tag": "goodbye",
         "patterns": ["Bye", "See you later", "Goodbye"],
         "responses": ["Goodbye! Have a great day!", "See you later!"]
       }
     ]
   }
   ```

4. **Run the chatbot**:
   ```bash
   python chatbot.py
   ```

## How It Works
1. The chatbot loads the intents data from a `JSON` file.
2. User input is preprocessed to ensure consistency (lowercasing, punctuation removal, tokenization).
3. The chatbot matches the cleaned input with the examples provided in the intents.
4. It returns the most relevant response associated with the matched intent.
5. Users interact with the chatbot via a Command-Line Interface (CLI).

## Example Interaction

```bash
User: Hi
Bot: Hello! How can I assist you today?

User: Bye
Bot: Goodbye! Have a great day!
```

## Key Concepts and Techniques
- **JSON**: Used to store and structure intents.
- **Text Preprocessing**: Input is cleaned (lowercased, tokenized) for accurate intent matching.
- **Simple Matching Algorithm**: The chatbot uses a basic algorithm to match user input with predefined patterns.
- **Command-Line Interface (CLI)**: Enables real-time user interaction.

## Future Enhancements
- Implement more advanced NLP techniques for better intent matching.
- Add support for multiple languages.
- Develop a graphical user interface (GUI) for improved user experience.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to customize the repository link, future enhancements, or any other details based on your specific project.
