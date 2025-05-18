# Gemini Twitter Bot

A Twitter bot that uses Google's Gemini AI to automatically reply to tweets about specific topics.

## Features

- Monitors Twitter for specific topics/keywords
- Uses Google Gemini to generate contextual responses
- Configurable rate limiting
- MongoDB integration for data persistence
- Comprehensive logging

## Prerequisites

- Node.js (v16 or higher)
- MongoDB
- Twitter Developer Account
- Google Cloud Account with Gemini API access

## Setup

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```
3. Copy `.env.example` to `.env` and fill in your credentials:
   ```bash
   cp .env.example .env
   ```
4. Configure your environment variables in `.env`

## Required Environment Variables

- `TWITTER_API_KEY`: Your Twitter API key
- `TWITTER_API_SECRET`: Your Twitter API secret
- `TWITTER_ACCESS_TOKEN`: Your Twitter access token
- `TWITTER_ACCESS_SECRET`: Your Twitter access secret
- `GEMINI_API_KEY`: Your Google Gemini API key
- `MONGODB_URI`: MongoDB connection string
- `TOPICS`: Comma-separated list of topics to monitor
- `MAX_REPLIES_PER_HOUR`: Maximum number of replies per hour

## Usage

Start the bot:
```bash
npm start
```

For development with auto-reload:
```bash
npm run dev
```

## Project Structure

```
src/
├── config/         # Configuration files
├── services/       # Core services (Twitter, Gemini)
├── models/         # Database models
├── utils/          # Utility functions
└── index.js        # Main application entry
```

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License

MIT