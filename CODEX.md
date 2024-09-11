<!--BEGIN_BANNER_IMAGE--> <picture> <source media="(prefers-color-scheme: dark)" srcset="/.github/banner_dark.png"> <source media="(prefers-color-scheme: light)" srcset="/.github/banner_light.png"> <img style="width:100%;" alt="D3M0N AI banner" src="https://raw.githubusercontent.com/livekit/agents/main/.github/banner_light.png"> </picture> <!--END_BANNER_IMAGE-->
D3M0N-AI-Realms
<!--BEGIN_DESCRIPTION-->
D3M0N-AI-Realms is a real-time, interactive, multi-modal AI framework built for creating chaotic, demon-themed experiences. It’s designed for entertainment platforms, allowing users to interact with digital personas, summon entities, and engage in real-time conversations. The framework handles speech-to-text, voice activity detection, and real-time personality generation while scaling to support thousands of concurrent sessions.

<!--END_DESCRIPTION-->
Using D3M0N-AI-Realms, you can create custom agents that serve as hosts, bouncers, or assistants in digital worlds, perfect for immersive shows, live call-in events, and interactive, chaotic experiences. It integrates seamlessly with LiveKit for real-time interaction, voice recognition, and audio streaming.

Note: This is in Beta, meaning APIs may change, and we welcome feedback. Feel free to contribute or chat with us on our Community Slack.

Features & Examples
Digital Summoning: Summon random entities based on user input with live STT and VAD.
Real-time Personality Switching: Switch AI personalities in real-time based on user actions or moods.
Live Show Integration: Perfect for hosting live interactive shows where users can call in and engage with digital demons or other entities.
Chaos Control: Built-in voice activity detection to adjust the AI's response based on noise levels and user engagement.
Check out these sample projects:

Voice assistant demo
Text-to-Speech agent example
Speech-to-Text demo
Installation
bash
Copy code
pip install d3m0n-ai-realms
Plugins
Leverage existing plugins to add more features:

Plugin	Features
livekit-plugins-deepgram	STT
livekit-plugins-elevenlabs	TTS
livekit-plugins-openai	LLM, STT, TTS
Example Code
Here's how to get your D3M0N agent up and running:

python
Copy code
from livekit.plugins.openai.llm import LLM
from livekit.agents import Agent

# Define agent behavior
class D3M0NAgent(Agent):
    def on_message(self, message):
        self.send_message(f"Welcome to the underworld, how can I help?")
Launching the System
Once installed, use the following commands to start your agent:

bash
Copy code
python d3m0n_agent.py start
To work in development mode with hot reloading:

bash
Copy code
python d3m0n_agent.py dev
Playground
The project also includes a web UI called Playground for testing agent functionality. Modify the UI or integrate it into your system for real-time testing.

Hosted playground
Source code
This CODEX serves as your guide for D3M0N-AI-Realms, a unique framework for real-time interactive AI experiences, blending advanced AI interaction with chaotic and entertaining digital personas. Whether for live shows or interactive chat, this framework ensures scalable, dynamic experiences tailored to your vision.







