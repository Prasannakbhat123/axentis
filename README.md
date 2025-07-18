# WhatsApp Bot Platform

A full-stack WhatsApp bot platform with a web interface for controlling the bot, executing commands, and capturing screenshots.

## Features

- Connect to WhatsApp via QR code
- Send and receive messages through a web interface
- Voice message support with speech-to-text and text-to-speech
- System command execution
- Screenshot capture
- AI-powered command generation

## Setup

### Requirements

- Node.js (v14+)
- npm or yarn
- For voice message support: ffmpeg and whisper AI

### Installation

1. Clone the repository:

```bash
git clone <repository-url>
cd axentis
```

2. Install dependencies:

```bash
npm run install-all
```

3. For Windows users who want to use the screenshot functionality:

```bash
npm run setup-windows
```

This will download and install nircmd, which is used for taking screenshots on Windows.

4. Start the application:

```bash
npm start
```

The application will start both the backend server (port 3000) and the frontend development server (port 5173).

## Usage

1. Open your browser and navigate to `http://localhost:5173`
2. Connect to WhatsApp by scanning the QR code in the WhatsApp tab
3. Start interacting with the bot from both the web interface and WhatsApp

## Troubleshooting

### Screenshot Issues

If you encounter issues with the screenshot functionality:

- On Windows: Run `npm run setup-windows` to install nircmd
- On Linux: Ensure you have gnome-screenshot, scrot, or ImageMagick installed
- On macOS: No additional setup required

## Project Structure

- `backend/` - Backend server with API endpoints
- `frontend/` - React frontend
- `package.json` - Root package.json for managing the project

## Environment Variables

Create a `.env` file in the backend directory with the following variables:

```
PORT=3000
GOOGLE_API_KEY=your_google_api_key
ELEVEN_LABS_API_KEY=your_eleven_labs_api_key
YOUTUBE_API_KEY=your_youtube_api_key
```

## License

MIT License
 
 
