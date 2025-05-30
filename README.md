﻿# Joke Teller with Voice RSS API

![jokeImage](https://github.com/user-attachments/assets/d3d818f1-78ec-4a0b-9a84-b68868e3774c)

This project is a simple joke-telling web application that fetches jokes from the JokeAPI and uses the Voice RSS API to convert them to speech. It includes a button to fetch and play jokes, with the button automatically disabling while the joke is playing.

## Architecture
![Architecture](architecture%20of%20api%20requests.png)

## Features

- Fetches programming-related jokes from the JokeAPI.
- Converts text jokes to speech using the Voice RSS Text-to-Speech API.
- Disables the button while a joke is playing to prevent interruptions.

## Prerequisites

1. A free Voice RSS API key. You can obtain one by signing up at [Voice RSS API](https://www.voicerss.org/).
2. Basic understanding of HTML, CSS, and JavaScript.

## How It Works

1. When the user clicks the button, the app fetches a joke from the JokeAPI.
2. The fetched joke is passed to the Voice RSS API, which converts it into speech.
3. The joke is played using an audio element in the browser.
4. The button is disabled while the joke is playing and re-enabled when playback ends.

## Code Structure

### HTML

The HTML includes:

- A button element with the ID `button` to trigger the joke fetch.
- An audio element with the ID `audio` to play the joke audio.

### JavaScript

The JavaScript includes:

- Integration with the JokeAPI to fetch jokes.
- Integration with the Voice RSS API for text-to-speech functionality.
- Functions to manage the button's state and handle audio playback.

### Example JavaScript Functions

- **`getJokes()`**: Fetches a joke from the JokeAPI and passes it to the `tellMe()` function.
- **`tellMe(joke)`**: Uses the Voice RSS API to convert the joke into speech.
- **`toggleButton()`**: Toggles the button's disabled state.
- **Event Listeners**: Listens for the button click to fetch jokes and for the audio element's `ended` event to re-enable the button.

## Setup Instructions

1. Clone this repository or copy the code into your project.
2. Replace `<YOUR_API_KEY>` in the `tellMe()` function with your Voice RSS API key.
3. Open the project in a browser.

## Usage

1. Click the button to hear a programming joke.
2. Wait for the joke to finish playing before clicking the button again.

## Dependencies

- [JokeAPI](https://jokeapi.dev) for fetching jokes.
- [Voice RSS API](https://www.voicerss.org/) for text-to-speech functionality.

### Image taken from [ ROBOT.GIF from Giphy](https://giphy.com/gifs/robot-cinema-4d-eyedesyn-3o7abtn7DuREEpsyWY)
