# PulseNet API

Network monitoring and analysis API built with TypeScript and Express.

## Features

- Real-time network monitoring
- SSE (Server-Sent Events) for live updates
- LLM integration for intelligent analysis
- Rate limiting and authentication middleware
- Comprehensive NOC (Network Operations Center) services

## Quick Start

### Prerequisites
- Node.js 18+
- npm or yarn

### Installation

```bash
# Install dependencies
npm install

# Build TypeScript
npm run build

# Start development server
npm run dev

# Start production server
npm start
```

### Environment Variables

Copy `.env.example` to `.env` and configure:

```bash
cp .env.example .env
```

## Deployment

### Railway

1. Connect your GitHub repository to Railway
2. Set environment variables in Railway dashboard
3. Deploy automatically on push to main branch

### Docker

```bash
docker build -t pulsenet-api .
docker run -p 3000:3000 pulsenet-api
```

## API Structure

```
src/
├── middlewares/      # Express middleware (auth, rate-limit, etc)
├── services/         # Business logic (NOC services, LLM, SSE)
├── workspace/        # API schema definitions (Zod)
└── index.ts         # Application entry point
```

## Services

- **NOC SSE**: Server-Sent Events for real-time network status
- **NOC LLM**: AI-powered analysis and insights
- **NOC Collector**: Data collection from network sources
- **NOC Analysis**: Network performance analysis
- **NOC Actions**: Automated response actions
- **NOC Settings**: Configuration management
- **Subscription Lifecycle**: Manage service subscriptions

## License

MIT
