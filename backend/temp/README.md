# S.H.A.D.O.W Backend

**Video Evidence Recognition & Intelligent Truth Assessment System**

AI-powered deepfake detection API using multi-layered hybrid analysis.

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template)

---

## 🚀 Quick Deploy

### Railway (Recommended)
```bash
railway login
railway init
railway up
railway variables set CORS_ORIGINS="https://your-frontend.vercel.app"
```

### Render / Heroku
See [DEPLOYMENT.md](DEPLOYMENT.md) for detailed instructions.

---

## ⚡ Features

- **Image Analysis**: Neural ensemble, frequency analysis, facial analysis, metadata forensics
- **Video Analysis**: Multi-layered hybrid detection with temporal consistency, audio analysis, physiological signals
- **Real-time Progress**: Server-Sent Events for live analysis updates
- **Configurable**: Environment-based configuration for all settings

---

## 📋 Requirements

- Python 3.12+
- 2GB+ RAM (4GB recommended)
- Optional: CUDA-compatible GPU

---

## 🛠️ Local Development

```bash
# Install dependencies
pip install -r requirements.txt

# Create environment file
cp .env.example .env

# Run server
python main.py
```

Server runs at: `http://localhost:8000`

API docs at: `http://localhost:8000/docs`

---

## 🔧 Configuration

See `.env.example` for all configuration options.

Key environment variables:
- `CORS_ORIGINS` - Allowed frontend URLs
- `MODEL_DEVICE` - `cuda` or `cpu`
- `MAX_FILE_SIZE_MB` - Upload limit

---

## 📚 API Endpoints

- `GET /health` - Health check
- `POST /analyze/image` - Quick image analysis
- `POST /analyze/image/comprehensive` - Comprehensive image analysis
- `POST /analyze/video` - Simple video analysis
- `POST /analyze/video/comprehensive` - Full hybrid video detection
- `GET /analyze/progress` - SSE progress updates

Full API documentation: `/docs`

---

## 🏗️ Project Structure

```
backend/
├── main.py                 # FastAPI application
├── config.py              # Configuration
├── requirements.txt       # Dependencies
├── models/                # Detection models
├── services/              # Business logic
└── utils/                 # Utilities
```

---

## 🐛 Troubleshooting

**Out of Memory**: Upgrade to 2GB+ RAM plan

**CUDA not available**: Set `MODEL_DEVICE=cpu`

**CORS errors**: Add frontend URL to `CORS_ORIGINS`

See [DEPLOYMENT.md](DEPLOYMENT.md) for more help.

---

## 📝 License

MIT License

---

## 👥 Team

- Faizan - Lead Engineer
- Vallabha - AI Architecture
- Gurunanda - Product Design

---

Built with ❤️ for digital truth and transparency
