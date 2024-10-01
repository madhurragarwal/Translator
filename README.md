# Speech-to-Text Language Detection and Translation

This project implements a simple pipeline that takes spoken input via a microphone, recognizes the speech, detects its language, and translates it to a target language. The project utilizes Python libraries such as `speech_recognition`, `langdetect`, and `deep_translator` for these tasks.

## Features
- **Speech Recognition**: Captures speech through a microphone and converts it into text using Google's Speech Recognition API.
- **Language Detection**: Automatically detects the language of the recognized text.
- **Text Translation**: Translates the recognized text into a target language using Google Translator.

## Installation

To run this project locally, follow these steps:

1. **Clone the Repository**
    ```bash
    git clone https://github.com/yourusername/speech-to-text-translate.git
    cd speech-to-text-translate
    ```

2. **Install Dependencies**
    Install the required Python libraries by running:
    ```bash
    pip install -r requirements.txt
    ```

    The project requires the following libraries:
    - `speech_recognition`
    - `langdetect`
    - `deep_translator`

3. **Configure API Access**
    Ensure you have access to the internet, as the Google Speech API and Translator require it to process audio and translate text.

## Usage

Run the `Translator.ipynb` notebook, which includes the combined speech-to-text, language detection, and translation pipeline.

### Example Workflow
1. The microphone captures your speech.
2. The speech is converted to text in the specified input language (e.g., Hindi).
3. The script detects the language of the recognized text.
4. If the detected language is different from the target language (e.g., English), the text is translated.

### Script Example

```python
speech_to_text_and_translate(target_lang='en')
