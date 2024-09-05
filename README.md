# Narration of your webcam feed using 11labs voices

## Setup

Clone this repo, and setup and activate a virtualenv:

```bash
python3 -m pip install virtualenv
python3 -m virtualenv venv
source venv/bin/activate
```

Then, install the dependencies:
`pip install -r requirements.txt`

Make a [Replicate](https://replicate.com), [OpenAI](https://openai.com/), and [ElevenLabs](https://elevenlabs.io) account and set your tokens in the .env file:

```
OPENAI_API_KEY=<your-openai-token>
REPLICATE_API_KEY=<your-replicate-token>
ELEVENLABS_API_KEY=<your-elevenlabs-token>
```

Make a new voice in Eleven and get the voice id of that voice.
Custom voices requires a paid subscription (Standard+ minimum).

Enter the VOICE_ID in the .env file:
```
ELEVENLABS_VOICE_ID=<voice-id>
```

## Run it!

In on terminal, run the webcam capture:
```bash
python capture.py
```
In another terminal, run the narrator:

```bash
python narrator.py
```

