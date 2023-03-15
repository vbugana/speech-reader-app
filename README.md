# Speech Reader App

A text to speech app for non-verbal people. Pre-made buttons and custom text speech. This project uses the Web Speech API

## Description

This is a simple web app for a speech synthesizer. It includes the following functionalities:

- Display a set of boxes, each containing an image and a message. When a box is clicked, its message is spoken aloud using the speech synthesis API.
- Allow the user to toggle a text box for entering their own message, which can be read aloud using the "Read Text" button.
- Allow the user to choose from a list of available voices for the speech synthesizer.

Here's a breakdown of the code:

1. First, it selects various elements from the HTML document using the `querySelector` and `getElementById` methods.
2. It defines an array of objects called data, each representing a speech box with an image and text message.
3. It iterates over the data array and calls the `createBox` function to create a box for each object.
4. The `createBox` function creates a `div` element, sets its class to box, and populates it with an image and text message. It also adds a click event listener to the box that speaks its text message when clicked.
5. It defines a `SpeechSynthesisUtterance` object called message, which will be used to store the text to be spoken.
6. It defines an empty array called voices, which will be used to store the available voices for the speech synthesizer.
7. It defines a `getVoices` function that gets the available voices using the `getVoices` method of the `speechSynthesis` object.
8. It then populates the `voicesSelect` element with options for each available voice.
9. It defines a `setTextMessage` function that sets the text property of the message object to the specified text.
10. It defines a `speakText` function that speaks the text stored in the message object using the speak method of the `speechSynthesis` object.
11. It defines a `setVoice` function that sets the voice property of the message object to the selected voice from the `voicesSelect` element.
12. It adds an event listener to the `voiceschanged` event of the `speechSynthesis` object, which calls the `getVoices` function when the list of available voices changes.
13. It adds event listeners to the `toggleBtn`, `closeBtn`, `voicesSelect`, and `readBtn` elements that toggle the text box, close the text box, change the selected voice, and read the entered text, respectively.
14. Finally, it calls the `getVoices` function to populate the voicesSelect element with the available voices.

Overall, this a simple example of how to use the speech synthesis API to create a basic speech synthesizer web app.

## Project Specifications

- Create responsive UI (CSS Grid) with picture buttons
- Speaks the text when button clicked
- Drop down custom text to speech
- Speaks the text typed in
- Change voices and accents

## License

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## Technologies Used

![HTML 5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)

![CSS 3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

![Javascript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

## 😂 Here is a random joke that'll make you laugh!

![Jokes Card](https://readme-jokes.vercel.app/api)

https://mdb.pushkaryadav.in/generate
