# Vora

> Open-source, privacy-first voice dictation for everyone

Vora is a cross-platform voice dictation system that keeps your data private. Dictate naturally across any application with complete control over your data - no subscriptions, no limits, no compromises.

## ✨ Features

- 🎤 **System-wide dictation** - Works in any application
- 🔒 **Privacy-first** - Local processing by default, your data never leaves your device
- 🚀 **Fast & accurate** - Powered by open-source Whisper models
- 💻 **CLI support** - Voice input for your terminal workflows
- 🏠 **Self-hostable** - Deploy your own backend if you choose
- 🆓 **Truly free** - No subscription, no usage limits, no accounts required

## 🛠️ Tech Stack

- **Desktop App**: Wails (Go + React + TypeScript + shadcn/ui)
- **Backend API**: Go (Fiber framework)
- **ML Service**: Python (FastAPI + faster-whisper)
- **CLI Tool**: Go (Cobra)

**Prerequisites:**

- Go 1.25+
- Node.js 24+
- Python 3.11+
- Docker & Docker Compose
- Make

## 📁 Repository Structure

```
vora/
├── desktop/          # Wails desktop app (Go + React)
├── ml-service/       # Python ML service (FastAPI + Whisper)
├── cli/              # Go CLI tool
├── docs/             # Documentation
├── scripts/          # Build and utility scripts
├── server/           # Go API server
├── Makefile          # Central build system
└── docker-compose.yml
```

## 🚧 Project Status

**Currently in initial setup phase** - Repository structure is being established.

**Current Progress:**

- [ ] Desktop app audio capture
- [ ] Whisper model integration
- [ ] Backend API implementation
- [ ] CLI tool functionality
- [ ] Component integration

## 📋 Development Roadmap

### Phase 1: MVP (Current)

- [ ] Basic desktop application with audio recording
- [ ] Local Whisper transcription
- [ ] Simple CLI tool
- [ ] Backend API skeleton

### Phase 2: Enhanced Features

- [ ] Improved UI/UX
- [ ] Clipboard integration
- [ ] Auto-paste functionality
- [ ] Model selection

### Phase 3: Advanced

- [ ] Custom voice commands
- [ ] Multi-language support
- [ ] Self-hosting documentation
- [ ] Performance optimization

## 🏗️ Architecture

Vora uses a hybrid Go + Python architecture:

```
Desktop App (Wails) ──> Go Backend API ──> Python ML Service
                                              (Whisper)
                                                 ▲
CLI Tool (Go) ───────────────────────────────────┘
```

- **Go** handles system integration, routing, and performance-critical operations
- **Python** handles ML model inference (Whisper)
- Communication via HTTP/gRPC between components

## 📝 License

MIT License - see [LICENSE](LICENSE) for details

## 🔗 Links

- Documentation: Coming soon
- Issues: [GitHub Issues](https://github.com/heyvora/vora/issues)
- Discord: Coming soon

---

**Note**: This project is in active early-stage development. Star ⭐ the repo to follow our progress!
