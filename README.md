
# VocalGPT: Engage in Realistic AI-Powered Phone Call Simulations 

This project combines the power of OpenAI's GPT language model and ElevenLabs' realistic voice synthesis to create engaging and dynamic voice-based chatbot experiences. Simulate phone calls with a customizable AI assistant, complete with natural conversations and lifelike voice interactions.

## Features

- **Voice-Based Interaction:** Talk to the AI using your microphone, and hear its responses in a synthesized voice.
- **GPT-Powered Conversations:** Leverage the advanced language capabilities of OpenAI's GPT models (gpt-4o) for natural and context-aware responses. 
- **Customizable Prompts:** Define specific scenarios and information for the AI using prompt files, enabling tailored interactions (like simulating customer service calls, role-playing, etc.).
- **ElevenLabs Integration:** Utilize ElevenLabs' API to generate high-quality, human-like speech from the AI's responses.
- **OpenAI Text-to-Speech (Optional):** Choose between ElevenLabs or OpenAI's text-to-speech engine for generating the AI's voice.

## Use Cases

- **Customer Service Training:** Simulate realistic customer support interactions to train agents in handling various scenarios.
- **Language Learning:** Practice conversational skills in a foreign language with a patient and engaging AI tutor.
- **Role-Playing and Storytelling:** Create immersive role-playing games or interactive stories with dynamic dialogue. 
- **Accessibility:** Provide a voice-based interface for interacting with AI models, enhancing accessibility for users with visual impairments. 

## Talking with Your Own Voice (ElevenLabs)

ElevenLabs allows you to create custom voice clones. By integrating your own cloned voice, you can make the AI speak with your voice, leading to highly personalized and engaging experiences.

**Here's how to do it:**

1. **Create a Voice Clone:** Follow the instructions on the [ElevenLabs platform](https://beta.elevenlabs.io/) to create a clone of your own voice. You'll typically need to record a few phrases.
2. **Get Your Voice ID:**  Once your voice clone is ready, ElevenLabs will provide you with a unique Voice ID.
3. **Update the Code:** In the `VOICE_ID` variable, replace the placeholder value with your ElevenLabs Voice ID:
   ```python
   VOICE_ID = "YOUR_ELEVENLABS_VOICE_ID" 
   ```

Now, when you run the application, the AI's responses will be spoken in your own voice, creating a truly unique and personalized experience.

## Getting Started

1. **Prerequisites:**
   - Python 3.7 or higher
   - OpenAI API Key: [https://platform.openai.com/account/api-keys](https://platform.openai.com/account/api-keys)
   - ElevenLabs API Key: [https://beta.elevenlabs.io/](https://beta.elevenlabs.io/)
2. **Installation:**
   ```bash
   git clone https://github.com/yourusername/your-repo-name 
   cd your-repo-name
   pip install -r requirements.txt 
   ```
3. **Configuration:**
   - Update the `api_key` values in the code with your OpenAI and ElevenLabs API keys. 
   - Customize the prompt file (`prompts/vet_prompt.md` by default) to define your desired scenario.
4. **Run the Application:**
   ```bash
   python main.py 
   ```

## Command Line Arguments

- `-pf, --prompt_file`: Specify a different prompt file.
- `-tts, --tts_type`: Choose the TTS engine (default: `openai`): 
    - `openai`: Use OpenAI's text-to-speech.
    - `elevenlabs`: Use ElevenLabs' text-to-speech.

## Contributing

Contributions are welcome! Feel free to open issues or pull requests. 

## License

This project is licensed under the MIT License.

