# Sonos TTS Using audioClip

This project was built with [React Express Starter](https://github.com/philnash/react-express-starter). Then Sonos-specific interfaces were built, and back-end server endpoints to invoke them.

Read more about this project on the [Sonos Developer Blog]( https://developer.sonos.com/code/making-sonos-talk-with-the-audioclip-api/).

In a nutshell, we're using the [audioClips](https://developer.sonos.com/reference/control-api/audioclip/) namespace commands in the [Sonos Control API](https://developer.sonos.com/build/direct-control/) to play speech. This speech was created using Google Translate's text to speech API.

To use this app, you'll need to get an API key from the [Sonos Developer Portal](https://developer.sonos.com). Create an account there, then create a new [Control Integration](https://developer.sonos.com/news/create-client-credentials/). You can read more about getting started with Control Integrations [here](https://developer.sonos.com/build/connected-home-get-started/).

## Using this project

Clone the project, change into the directory and install the dependencies.

```bash
git clone https://github.com/sonos/sonos-audioclip-tts.git
cd sonos-audioclip-tts
npm install
```

Copy the `.env.example` file to an `.env` file. Enter your API key and secret, obtained above, in that new `.env` file.

Run both the server and front-end applications together with the command:

```bash
npm run dev
```

The React application will run on port 3000 and the server port 3001.
