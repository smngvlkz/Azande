## Voice Chatbot

This is a Python script project that allows you to speak to a large language model through voice. You can ask any question or chat about any topic, and the model will generate a response that will be read aloud by the text-to-speech engine.

# Requirements

Python 3.6 or higher
openai, pyttsx3, and speech_recognition modules
OpenAI API key
Yi model from 01.AI

# Usage

Clone or download this repository to your local machine.
Open the main.py file in your preferred code editor.
Set your OpenAI API key in the openai.api_key variable.
Run the script from the terminal or command prompt using the command python main.py.
The script will wait for you to say “hello azande” to start recording your questions.
Say your question and wait for the model to generate a response.
The response will be displayed on the screen and read aloud by the text-to-speech engine.
To stop the script, press Ctrl+C.

## Technical Achievements

The script uses the speech_recognition library to convert user voice input into text. It supports various audio sources, such as microphone, audio file, or online stream.
The script uses the openai library to generate responses using the text-davinci-003 engine and a custom prompt. The prompt specifies the parameters for the completion, such as max_tokens, temperature, and stop.
The script uses the pyttsx3 library to convert the text responses into voice output. It supports various speech engines, such as SAPI5, nsss, or espeak.
The script uses the Yi model from 01.AI, a custom large language model that claims to be more accurate and fluent than GPT-3.

## Technical Challenges and Solutions

One of the challenges was to handle the errors and exceptions that might occur during the voice recognition or response generation process. For example, the user might say something that is not recognized by the speech_recognition library, or the openai library might return an invalid response. To solve this, the script uses try-except blocks to catch and handle the errors gracefully, and prints a message to inform the user of the problem.
Another challenge was to adjust the parameters of the speech_recognition and pyttsx3 libraries to optimize the performance and user experience. For example, the script had to set the pause_threshold and phrase_time_limit of the speech_recognition library to control the duration of the recording, and the rate and volume of the pyttsx3 library to control the speed and loudness of the speech output. To solve this, the script used trial and error to find the optimal values for these parameters, and allowed the user to change them if needed.
