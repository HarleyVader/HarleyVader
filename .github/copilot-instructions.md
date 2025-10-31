# GitHub Copilot Instructions for BambiSleep Ecosystem

## 🌀 Codebase Overview

This is a **multi-project ecosystem** focused on **hypnotic AI applications**, **Discord bots**, **web applications**, and **server management tools**. The codebase represents a specialized collection of interconnected projects for content delivery, AI integration, and community management.

### 🎯 Primary Tech Stack

- **Languages**: JavaScript (Node.js), TypeScript, PHP, Shell/Bash, Python
- **Frameworks**: Express.js, Discord.js, p5.js, Socket.io
- **Databases**: MongoDB, MySQL/MariaDB, PostgreSQL
- **AI/ML**: Model Context Protocol (MCP), LMStudio integration
- **Media**: FFmpeg for audio/video processing
- **Infrastructure**: Docker, systemd services, Apache/Nginx

### 📁 Project Structure & Purposes

#### 🤖 AI-Enhanced Discord Bot (`js-bambisleep-bimbot/`)
- **Purpose**: Advanced Discord bot with AI integration for hypnotic content
- **Features**: Audio/video streaming, LMStudio AI integration, script generation
- **Stack**: Node.js, Discord.js, FFmpeg, MCP protocol
- **Key Files**: `bimbot.js`, `commands/`, `utils/`, `mcp/server.js`

#### 💬 Real-time Chat Platform (`js-bambisleep-chat/`)
- **Purpose**: WebSocket-based chat with psychedelic effects and TTS
- **Features**: Real-time messaging, spiral animations, trigger detection
- **Stack**: Node.js, Express.js, Socket.io, p5.js
- **Key Files**: `server.js`, `public/js/`, `views/`

#### 🔗 Patreon Integration Library (`js-bambisleep-chat-patreon/`)
- **Purpose**: TypeScript library for Patreon API v2 integration
- **Features**: OAuth2, webhook handling, rate limiting, auto token refresh
- **Stack**: TypeScript, Node.js, comprehensive testing
- **Key Files**: `src/`, `examples/`, strict TypeScript definitions

#### 🏛️ Community Hub (`js-bambisleep-church/`)
- **Purpose**: Community-voted link aggregation with AI integration
- **Features**: Real-time voting, MCP server, content curation
- **Stack**: Node.js, Express.js, EJS templating, MCP protocol
- **Key Files**: `src/server.js`, `src/mcp/McpServer.js`, `views/`

#### 🎥 Video Streaming Service (`js-brandynette-xxx-filehost/`)
- **Purpose**: Kawaii-themed video streaming platform
- **Features**: Video file hosting, streaming API, pink UI theme
- **Stack**: Node.js, Express.js, custom video player
- **Key Files**: `src/server.js`, `public/`, `BRANDIFICATION/`

#### 🌀 Interactive Trigger Game (`js-psychodelic-trigger-mania/`)
- **Purpose**: Browser-based psychedelic trigger interaction
- **Features**: Eye cursor tracking, trigger lists, visual effects
- **Stack**: HTML5, CSS3, Bootstrap, vanilla JavaScript
- **Key Files**: `index.html`, `listOfTriggers.json`, `js/`

#### 🖥️ Server Control Panel (`js-bambilseep-hestiacp/`)
- **Purpose**: Fork of HestiaCP for web hosting management
- **Features**: User management, DNS, databases, SSL certificates
- **Stack**: PHP, Bash, Apache/Nginx, MariaDB
- **Key Files**: `bin/`, `web/`, `install/`, extensive CLI tools

### 🎨 Design Philosophy & Conventions

#### Code Style
- **ES6+ modules** preferred over CommonJS
- **Async/await** over promises for readability
- **Environment variables** for all configuration
- **Comprehensive error handling** with proper logging
- **TypeScript** for type safety where applicable

#### Naming Conventions
- **Files**: kebab-case for directories, camelCase for JS files
- **Variables**: camelCase for variables and functions
- **Constants**: UPPER_SNAKE_CASE for environment variables
- **Classes**: PascalCase

#### Project Patterns
- **MCP Integration**: Use Model Context Protocol for AI features
- **Service Architecture**: Separate concerns (bots, web servers, APIs)
- **Configuration**: `.env` files with `.env.example` templates
- **Testing**: Jest for testing, pre-deployment validation scripts
- **Documentation**: Comprehensive README files with emojis and clear structure

### 🔧 Development Guidelines

#### When Working on Discord Bots
- Use Discord.js v14+ patterns
- Implement slash commands with proper validation
- Handle voice channel connections gracefully
- Include comprehensive error handling for media playback

#### When Working on Web Applications
- Use Express.js with proper middleware
- Implement Socket.io for real-time features
- Include CORS configuration for API endpoints
- Use EJS or static HTML depending on project needs

#### When Working on AI Integration
- Follow MCP protocol standards
- Include fallback logic for AI service unavailability
- Implement proper token management and rate limiting
- Use environment variables for API keys and endpoints

#### When Working on Server Management
- Follow Bash scripting best practices
- Include proper argument validation
- Use exit codes consistently
- Maintain compatibility with Debian/Ubuntu systems

### 🚀 Deployment & Infrastructure

#### Service Management
- **systemd** services for production deployment
- **Docker** containers where applicable
- **Process managers** like PM2 for Node.js applications
- **Nginx/Apache** reverse proxy configurations

#### Security Considerations
- **Environment variables** for sensitive data
- **Input validation** and sanitization
- **Rate limiting** on public APIs
- **HTTPS/SSL** for all web services

### 📦 Package Management

#### Node.js Projects
- Use **npm** for dependency management
- Include both `dependencies` and `devDependencies`
- Pin major versions for stability
- Include `npm audit` in CI/CD pipelines

#### PHP Projects
- Follow **PSR standards** where applicable
- Use **Composer** for dependency management
- Include proper autoloading

### 🔍 Special Considerations

#### AI Integration
- Always include fallback behavior when AI services are unavailable
- Implement proper error handling for API rate limits
- Use environment variables for model selection and API endpoints

#### Media Handling
- Use **FFmpeg** for audio/video processing
- Implement proper file validation and security checks
- Include support for multiple audio/video formats

#### Real-time Features
- Use **Socket.io** for WebSocket management
- Implement proper connection handling and error recovery
- Include heartbeat/ping mechanisms for connection stability

### 🎯 Project Relationships

- **bimbot** serves as the central Discord hub
- **chat** provides web-based community interaction
- **church** handles content curation and voting
- **patreon** manages subscription and payment integration
- **filehost** provides media streaming capabilities
- **hestiacp** manages server infrastructure
- **trigger-mania** offers interactive experiences

All projects share common themes of **AI integration**, **real-time interaction**, and **community-focused features** while maintaining distinct purposes and technical approaches.

---

*Note: The `A-OS/` directory contains rescue/utility ISOs and should be ignored for development purposes.*