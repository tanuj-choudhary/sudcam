# Augmented Reality Sudoku Solver

This project will let you use your phone (or your computers webcam) as an Augmented Reality camera for solving Sudoku puzzles.

It's an interesting proof of concept to see how powerful browsers on phone are now.

To perform the OCR we use tensorflowjs. The image processing is all carried out in customer code.


# This project consists of 3 folders:

- app - the JavaScript application that runs in the browser using a phone's camera or webcam
- digit_recognition_gui - the gui app for digit recognition model
- sudoku-gui - the gui app for testing sudoku algorithm.

# Building the App

To build the application you will need to have node and yarn installed.

## Setup

```
cd app
yarn
yarn start
```

If you want to run the app locally then you will need to use something like `ngrok` to proxy `https` connections from your phone to your local server (most phones will not allow access to the camera unless the page is served over https).

Running in your desktop browser should work so long as you use the `localhost` connection as this bypasses the `https` requirement.

## Building

```
yarn build
```

# Training the neural network

The application invluces a pretrained network so you only need to do this if you want to train the network on new images.
