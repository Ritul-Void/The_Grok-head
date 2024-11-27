# The_Grok-head(v1.5.1)
it is a Grok AI gui application based on the grok ai api , an chatbot app. currrently token is fiexed at 200 you can chage it in the code


# Grok AI Chat Bot 

## Overview
The Grok AI Chat Bot is a web-based application that facilitates interaction with a conversational AI model. It features a clean and responsive UI with options for settings, message history, and chat customization.

---

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [File Structure](#file-structure)
- [Setup](#setup)
- [UI Components](#ui-components)
- [Customization](#customization)
- [Event Listeners](#event-listeners)
- [Storage](#storage)
- [Future Enhancements](#future-enhancements)

---

## Features
1. **Responsive Chat Interface**: 
   - Dark-themed UI with smooth message scrolling.
   - User and bot messages displayed distinctly.
2. **Settings Modal**:
   - Customize API key and system role message.
3. **Chat History**:
   - View previous chat sessions in a modal.
4. **Keyboard Input**:
   - Type messages in the input box and send with a button or Enter key.
5. **Reset Chat**:
   - Clear current messages to start fresh.
6. **Mobile-Friendly**:
   - Adjusted styles for smaller screens.

---

## Technologies Used
1. **HTML**: Structuring the web app.
2. **CSS**: Styling and responsive design.
3. **JavaScript**: Handling interactions and functionality.
4. **Third-party Libraries**:
   - [Marked](https://marked.js.org/): Parse Markdown text.
   - [DOMPurify](https://github.com/cure53/DOMPurify): Sanitize HTML content for security.

---

## File Structure
```plaintext
- index.html       # Main HTML file
- styles.css       # Contains styling (inline in your case)
- scripts.js       # JavaScript functionality
- assets/          # Any additional assets (images, etc.)
```

---

## Setup
1. Save the code as `index.html`.
2. Include the required scripts from the CDN:
   - `marked.min.js`
   - `dompurify.min.js`
3. Open the file in a web browser to run the chat interface.

---

## UI Components

### Chat Container
- **HTML**: `<div class="chat-container">`
- **CSS**: Styled to occupy the full viewport height and contain messages.

### Chat Header
- **HTML**: `<div class="chat-header">`
- **Features**:
  - History button (`🕓`).
  - Title (`The Grock Head`).
  - Settings button (`⚙️`).

### Chat Messages
- **HTML**: `<div class="chat-messages">`
- **CSS**: `overflow-y: auto` for scrollable content.

### Input Container
- **HTML**:
  ```html
  <div class="input-container">
    <input type="text" class="input-box" id="userInput" placeholder="Type your Message..." />
    <button class="send-button" id="sendMessage">↵</button>
    <button class="reset-button" id="resetChat">✎</button>
  </div>
  ```
- **JavaScript**: Handles sending and resetting of messages.

### Modals
1. **Settings Modal**:
   - Customize API key and system role message.
   - Save data in `localStorage`.
2. **History Modal**:
   - Display chat history in a tabular format.

---

## Customization

### Fonts
- **Google Fonts**:
  - `Doto` for headings.
  - `Space Grotesk` for body text.

### Colors
- Background: `#202020` (dark theme).
- Bot Messages: `#525252` (gray).
- User Messages: `#ffffff` (white).

### Variables
- **CSS Variables**:
  - `--dot-bg`: Background for the dotted pattern.
  - `--dot-color`: Color for dots.

---

## Event Listeners

### Core Events
1. **Send Message**:
   - Triggered by `#sendMessage` button or pressing Enter.
   - Appends user message and a placeholder for bot response.
2. **Reset Chat**:
   - Clears all messages when `#resetChat` button is clicked.
3. **Open Settings**:
   - Displays the settings modal when `#openSettings` is clicked.
4. **Close Settings**:
   - Hides the settings modal when `#closeSettings` is clicked.
5. **Save API Key**:
   - Saves API key and system role message to `localStorage`.
6. **View History**:
   - Opens the history modal.
7. **Close History**:
   - Closes the history modal.

---

## Storage
1. **LocalStorage**:
   - **API Key**: `localStorage.getItem("apiKey")`.
   - **System Role**: `localStorage.getItem("systemRoleMessage")`.
2. **Chat History**:
   - Saved in a structured format for retrieval.

---

## Future Enhancements
1. **Backend Integration**:
   - Connect with an API endpoint for bot responses.
2. **Real-Time Chat**:
   - Add WebSocket support for live updates.
3. **Message Formatting**:
   - Allow Markdown and emoji support.
4. **Export Chat**:
   - Add an option to export chat history as a file.
5. **Themes**:
   - Allow switching between light and dark modes.

---
##Future Updates 
-electron app
-mobile app
-document upload
-additional model support 
-voice ai
-token customisation
---
## Additional Notes
- Ensure browser compatibility for all features.
- Optimize performance for larger chat histories.
- Use secure methods to store and handle API keys.

---

## Contact
For issues or suggestions, please contact [Your Email/Support Link].
