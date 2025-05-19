# Setup Guide / Kurulum Kılavuzu / Guía de Configuración

## Prerequisites / Ön Gereksinimler / Prerrequisitos

- Python 3.8 or higher
- pip (Python package installer)
- Git
- A Google Cloud account with Gemini API access
- Virtual environment tool (recommended)

## Installation Steps / Kurulum Adımları / Pasos de Instalación

### 1. Clone the Repository / Depoyu Klonlayın / Clonar el Repositorio

```bash
git clone https://github.com/yourusername/flashcard_generator.git
cd flashcard_generator
```

### 2. Create and Activate Virtual Environment / Sanal Ortam Oluşturun ve Aktifleştirin / Crear y Activar Entorno Virtual

#### Windows
```bash
python -m venv venv
.\venv\Scripts\activate
```

#### Linux/MacOS
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies / Bağımlılıkları Yükleyin / Instalar Dependencias

```bash
# Install production dependencies
pip install -r requirements.txt

# Install development dependencies (optional)
pip install -r requirements-dev.txt
```

### 4. Configure Environment Variables / Ortam Değişkenlerini Yapılandırın / Configurar Variables de Entorno

Create a `.env` file in the project root:

```bash
# .env
GOOGLE_API_KEY=your_api_key_here
DEBUG=False
LOG_LEVEL=INFO
```

### 5. Verify Installation / Kurulumu Doğrulayın / Verificar la Instalación

Run the test suite:

```bash
pytest tests/
```

## Project Structure / Proje Yapısı / Estructura del Proyecto

```
flashcard_generator/
├── docs/                    # Documentation
├── flashcard_generator/     # Main package
│   ├── __init__.py
│   ├── generator.py        # Core generation logic
│   ├── templates.py        # Flashcard templates
│   └── utils.py           # Utility functions
├── tests/                  # Test suite
├── examples/              # Example scripts
├── requirements.txt       # Production dependencies
├── requirements-dev.txt   # Development dependencies
└── README.md             # Project documentation
```

## Configuration Options / Yapılandırma Seçenekleri / Opciones de Configuración

### API Configuration / API Yapılandırması / Configuración de API

```python
# config.py
API_CONFIG = {
    'base_url': 'https://api.gemini.google.com/v1',
    'timeout': 30,
    'max_retries': 3,
    'cache_enabled': True,
    'cache_ttl': 3600  # 1 hour
}
```

### Logging Configuration / Günlük Yapılandırması / Configuración de Registro

```python
# logging_config.py
LOGGING_CONFIG = {
    'version': 1,
    'disable_existing_loggers': False,
    'formatters': {
        'standard': {
            'format': '%(asctime)s [%(levelname)s] %(name)s: %(message)s'
        },
    },
    'handlers': {
        'default': {
            'level': 'INFO',
            'formatter': 'standard',
            'class': 'logging.StreamHandler',
        },
    },
    'loggers': {
        '': {
            'handlers': ['default'],
            'level': 'INFO',
            'propagate': True
        }
    }
}
```

## Development Setup / Geliştirme Kurulumu / Configuración de Desarrollo

### 1. Install Development Tools / Geliştirme Araçlarını Yükleyin / Instalar Herramientas de Desarrollo

```bash
pip install -r requirements-dev.txt
```

### 2. Configure Pre-commit Hooks / Pre-commit Kancalarını Yapılandırın / Configurar Hooks de Pre-commit

```bash
pre-commit install
```

### 3. Setup Testing Environment / Test Ortamını Kurun / Configurar Entorno de Pruebas

```bash
# Create test database
python -m pytest tests/ --setup-show
```

## Troubleshooting / Sorun Giderme / Solución de Problemas

### Common Issues / Yaygın Sorunlar / Problemas Comunes

1. **API Key Issues / API Anahtarı Sorunları / Problemas con la Clave API**
   - Verify API key in `.env` file
   - Check API key permissions
   - Ensure API key is active

2. **Dependency Conflicts / Bağımlılık Çakışmaları / Conflictos de Dependencias**
   ```bash
   pip check
   ```

3. **Virtual Environment Issues / Sanal Ortam Sorunları / Problemas con el Entorno Virtual**
   ```bash
   # Recreate virtual environment
   rm -rf venv
   python -m venv venv
   source venv/bin/activate  # or .\venv\Scripts\activate on Windows
   pip install -r requirements.txt
   ```

## Security Considerations / Güvenlik Hususları / Consideraciones de Seguridad

1. Never commit `.env` file
2. Use environment variables for sensitive data
3. Implement rate limiting
4. Validate all input data
5. Use HTTPS for API calls

## Performance Optimization / Performans Optimizasyonu / Optimización de Rendimiento

1. Enable response caching
2. Use batch processing for multiple requests
3. Implement connection pooling
4. Monitor memory usage
5. Profile code regularly

## Support / Destek / Soporte

For additional help:
- Check the [documentation](docs/)
- Open an [issue](https://github.com/yourusername/flashcard_generator/issues)
- Contact: your.email@example.com 