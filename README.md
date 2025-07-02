# Dark Patterns Detector

A browser extension that automatically detects dark patterns on any webpage you visit. Dark patterns are deceptive design practices that manipulate users into doing things they might not otherwise do.

## Features

- **Simple Interface**: Minimalist design with a "Scan This Page" button
- **Pattern Detection**: Uses Gemini AI to analyze and identify dark patterns
- **Highlighting**: Highlight specific dark patterns or all patterns at once
- **Informative Tooltips**: View descriptions of each dark pattern and how it affects users
- **Educational Resource**: Links to more information about dark patterns

## Installation

### Development Mode

1. Download or clone this repository
2. Open Chrome and navigate to `chrome://extensions/`
3. Enable "Developer mode" in the top-right corner
4. Click "Load unpacked" and select the extension directory

### API Key Setup

1. Copy `config.template.js` to `config.js`
2. Obtain a Gemini API key from [Google AI Studio](https://makersuite.google.com/app/apikey)
3. Replace `YOUR_GEMINI_API_KEY_HERE` in `config.js` with your actual API key
4. The API key is stored locally and NOT shared when you commit code to GitHub

## Usage

1. Click on the extension icon in your browser toolbar
2. Click the "Scan This Page" button
3. Review the list of detected dark patterns
4. Use the "Highlight" buttons to visually identify dark patterns on the page
5. Click "Highlight All" to show all detected patterns at once
6. Hover over highlighted sections to see information about the dark pattern

## Icons

The extension requires three icon sizes:
- icons/icon16.png (16x16)
- icons/icon48.png (48x48)
- icons/icon128.png (128x128)

You can create these icons or replace them with your own designs.

## Technical Implementation

- **Popup Interface**: HTML/CSS/JavaScript that provides the user interface
- **Content Script**: Handles DOM manipulation and highlighting
- **AI Integration**: Sends page content to Gemini API for dark pattern detection
- **Storage**: Saves detection results between page refreshes

## Project Purpose

This extension was developed as a capstone project for BE IT Engineering, focusing on using machine learning to detect dark patterns in web design.


## Learn More

To learn more about dark patterns, visit [Deceptive Design](https://www.deceptive.design/) 
