# WhatsApp Chatbot with Twilio, OpenAI, Flask and PostgreSQL

This project is a WhatsApp chatbot built using **Twilio**, **OpenAI**, and **PostgreSQL**. The chatbot is capable of interacting with users through text, and it has a unique feature: it can **understand and process audio inputs directly** from the user, which sets it apart from typical AI chatbots like **MetaAI**.

## Features

- **WhatsApp Integration:** The bot interacts with users via WhatsApp, using Twilio's API to send and receive messages.
- **Audio Input Understanding:** Unlike other chatbots, this bot is capable of understanding audio messages directly from the user, converting speech to text for further processing.
- **OpenAI Integration:** Leverages OpenAI's GPT model to generate intelligent and context-aware responses based on user queries.
- **Database Integration (PostgreSQL):** Stores conversation history and user data, allowing for personalized interactions and improved bot performance over time.

## Technologies Used

- **Twilio API:** For WhatsApp messaging integration.
- **OpenAI GPT:** For generating responses to user inputs.
- **PostgreSQL:** To store user data and chat logs.
-**Flask**:For server
- **Speech-to-Text (Optional):** Converts user audio into text for processing.

## Setup Instructions

### Prerequisites

- Flask ()
- PostgreSQL (installed locally or using a cloud provider)
- Twilio account and WhatsApp sandbox setup
- OpenAI API key
- API credentials for Speech-to-Text (if using audio input)

### Installation Steps

1. **Clone the repository:**
   ```bash
   git clone <repository_url>
   cd <project_folder>
   ```

2. **Install dependencies:**
   pip install -r "requirement.txt"

3. **Set up PostgreSQL:**
   - Create a PostgreSQL database and configure it in your `config.js` or `.env` file.
   - Run the migration scripts to create the necessary tables.

4. **Configure Twilio:**
   - Sign up for a Twilio account and set up your WhatsApp sandbox.
   - Add your Twilio credentials (Account SID, Auth Token) to the environment variables or a config file.

5. **Configure OpenAI:**
   - Set up an API key for OpenAI and add it to your environment variables or config file.

6. **Speech-to-Text Integration (Optional):**
   - If you want the bot to process audio messages, integrate a speech-to-text service (like Google Cloud or IBM Watson) and set it up in the backend.

7. **Run the Application:**
   ```bash
   uvicorn main:app --reload --log-level debug
   ```

8. **Test the Bot:**
   - Send a message to your WhatsApp bot and interact with it via text or audio.

## Special Features

- **Audio Understanding:** Unlike standard chatbots, this bot can handle audio messages. The audio is converted to text and processed by OpenAI to generate appropriate responses.
- **Enhanced User Interaction:** The bot can remember user interactions over time, improving its responses and providing a more personalized experience.

## Contributing

Feel free to fork this project and create a pull request for improvements. If you have any bug reports or feature requests, open an issue in the GitHub repository.

## License

This project is open-source and licensed under the MIT License.

---

Feel free to update the sections based on your exact implementation and add any additional details relevant to your project!
