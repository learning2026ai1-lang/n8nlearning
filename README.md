# N8N Learning - Node.js Project

A Node.js learning project built with Express.js for the n8n workflow automation platform.

## Features

- Express.js HTTP server
- RESTful API endpoints
- Health check endpoint
- Environment variable configuration
- Development and production modes

## Installation

```bash
# Install dependencies
npm install
```

## Running the Project

### Development Mode (with auto-reload)
```bash
npm run dev
```

### Production Mode
```bash
npm start
```

The server will be available at `http://localhost:3000`

## API Endpoints

### GET /
Welcome endpoint that returns server status and timestamp.

**Response:**
```json
{
  "message": "Welcome to N8N Learning Node.js Project",
  "status": "running",
  "timestamp": "2026-05-26T12:00:00.000Z"
}
```

### GET /api/health
Health check endpoint for monitoring server status.

**Response:**
```json
{
  "status": "healthy",
  "uptime": 123.456,
  "timestamp": "2026-05-26T12:00:00.000Z"
}
```

## Environment Variables

Create a `.env` file in the root directory:

```env
PORT=3000
NODE_ENV=development
```

## Project Structure

```
.
├── src/
│   └── index.js          # Main server file
├── package.json          # Project dependencies
├── .env.example          # Environment variables template
├── .gitignore            # Git ignore rules
└── README.md             # This file
```

## Development

- **nodemon** - Automatically restarts the server on file changes
- **jest** - Testing framework for unit tests

## License

MIT
