# 🎙️ Perplexity Voice Module Integration

> Advanced voice AI system with continuous context, memory, and dynamic learning capabilities

## 🎯 Overview

This project implements a sophisticated voice AI system that integrates the Perplexity Voice Module with advanced operator code to provide:

- **Continuous Context**: Maintains conversation history and understanding
- **Dynamic Memory**: Long-term and short-term memory management
- **Context Enrichment**: Multi-source context integration
- **Real-time Learning**: Adaptive responses based on interaction patterns

## 🏗️ Architecture

### Three-Layer System Design

1. **Voice I/O Layer**: Handles audio input/output and speech processing
2. **Context & Memory Layer**: Manages conversation state and memory storage
3. **Operator Layer**: Orchestrates business logic and context enrichment

### Technology Stack

- **Voice Processing**: Perplexity Voice SDK
- **Memory Management**: SuperMemory + Vector Databases
- **Security**: MCP Guardian with authentication and rate limiting
- **Integration**: Notion MCP, GitHub MCP, Calendar connectors
- **Deployment**: Docker containers with load balancing

## 🚀 Quick Start

### Prerequisites

- Node.js 18+
- Docker and Docker Compose
- API keys for Perplexity, Notion, and other services

### Installation

```bash
# Clone the repository
git clone https://github.com/GlacierEQ/perplexity-voice-integration.git
cd perplexity-voice-integration

# Install dependencies
npm install

# Configure environment variables
cp .env.example .env
# Edit .env with your API keys

# Start the development server
npm run dev
```

### Docker Deployment

```bash
# Build and run with Docker Compose
docker-compose up --build -d

# Scale the service
docker-compose up --scale voice-ai-system=3
```

## 📋 Configuration

### Required Environment Variables

```bash
# Core API Keys
PERPLEXITY_API_KEY=your_perplexity_api_key
NOTION_TOKEN=your_notion_integration_token
SUPERMEMORY_API_KEY=your_supermemory_api_key
GITHUB_TOKEN=your_github_personal_access_token

# Database Configuration
PINECONE_API_KEY=your_pinecone_api_key
NEO4J_URI=your_neo4j_database_uri
NEO4J_USER=your_neo4j_username
NEO4J_PASSWORD=your_neo4j_password

# Security Settings
JWT_SECRET=your_jwt_secret_key
ENCRYPTION_KEY=your_encryption_key
RATE_LIMIT_MAX=100
RATE_LIMIT_WINDOW=60000
```

## 🔧 Components

### Voice I/O Layer (`src/voice/`)
- Audio capture and processing
- Speech-to-text integration
- Text-to-speech output
- Context-aware voice synthesis

### Memory System (`src/memory/`)
- Multi-layer memory architecture
- Vector storage and retrieval
- Knowledge graph integration
- Real-time memory updates

### Operator Layer (`src/operator/`)
- Business logic orchestration
- Context enrichment pipeline
- Security and validation
- Performance optimization

### Integration Connectors (`src/connectors/`)
- Notion MCP connector
- GitHub MCP connector
- SuperMemory connector
- Calendar integration

## 📊 Performance Metrics

### Target Performance
- Voice Processing Latency: < 200ms
- Memory Retrieval Speed: < 100ms
- Context Enrichment Time: < 300ms
- API Response Time: < 500ms
- Error Rate: < 0.1%

### Monitoring
- Real-time metrics dashboard
- Performance alerting
- Error tracking and logging
- Resource usage monitoring

## 🔐 Security Features

- **Authentication**: OAuth2 and JWT token validation
- **Rate Limiting**: Configurable request throttling
- **Data Encryption**: AES-256-GCM for sensitive data
- **Input Validation**: Comprehensive input sanitization
- **Audit Logging**: Complete interaction tracking

## 🛠️ Development

### Project Structure

```
perplexity-voice-integration/
├── src/
│   ├── voice/           # Voice I/O components
│   ├── memory/          # Memory management
│   ├── operator/        # Business logic
│   ├── connectors/      # External integrations
│   ├── security/        # Security modules
│   └── utils/           # Utility functions
├── config/              # Configuration files
├── docs/                # Documentation
├── tests/               # Test suites
├── docker/              # Docker configurations
└── scripts/             # Deployment scripts
```

### Testing

```bash
# Run unit tests
npm test

# Run integration tests
npm run test:integration

# Run performance tests
npm run test:performance

# Generate coverage report
npm run test:coverage
```

### Building

```bash
# Build for production
npm run build

# Build Docker image
docker build -t perplexity-voice-integration .

# Create deployment package
npm run package
```

## 📚 Documentation

- [Architecture Guide](docs/architecture.md)
- [API Reference](docs/api.md)
- [Deployment Guide](docs/deployment.md)
- [Security Guide](docs/security.md)
- [Troubleshooting](docs/troubleshooting.md)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines

- Follow ESLint configuration
- Write comprehensive tests
- Document new features
- Update CHANGELOG.md
- Ensure security compliance

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

- **Issues**: [GitHub Issues](https://github.com/GlacierEQ/perplexity-voice-integration/issues)
- **Discussions**: [GitHub Discussions](https://github.com/GlacierEQ/perplexity-voice-integration/discussions)
- **Documentation**: [Project Wiki](https://github.com/GlacierEQ/perplexity-voice-integration/wiki)

## 🎯 Roadmap

- [ ] Multi-modal integration (image/document processing)
- [ ] Advanced analytics and insights
- [ ] Mobile application support
- [ ] Real-time collaboration features
- [ ] Advanced AI model fine-tuning
- [ ] Enterprise security enhancements

---

**Made with ❤️ by the GlacierEQ Team**

*Empowering intelligent voice interactions through advanced AI integration*