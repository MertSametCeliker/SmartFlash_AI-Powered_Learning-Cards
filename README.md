# 🧠 AI-Powered Educational Flashcard Generator / AI Destekli Eğitici Flashcard Oluşturucu / Generador de Tarjetas Educativas con IA

[![Python Version](https://img.shields.io/badge/python-3.7%2B-blue)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.32.0-FF4B4B)](https://streamlit.io/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Gemini AI](https://img.shields.io/badge/Gemini%20AI-0.3.2-orange)](https://ai.google.dev/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/yourusername/flashcard_generator/issues)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://www.linkedin.com/in/mert-samet-çeliker-18a906294/)

<div align="center">
  <img src="assets/logo.png" alt="Flashcard Generator Logo" width="200"/>
  
  *An Advanced AI-Powered Educational Tool for Dynamic Flashcard Generation*
</div>

## 📑 Table of Contents / İçindekiler / Índice
- [Features](#-features--özellikler--características)
- [English Documentation](#-english-documentation)
- [Türkçe Dokümantasyon](#-türkçe-dokümantasyon)
- [Documentación en Español](#-documentación-en-español)
- [Project Structure](#-project-structure--proje-yapısı--estructura-del-proyecto)
- [Development](#-development--geliştirme--desarrollo)
- [License](#-license--lisans--licencia)
- [Acknowledgments](#-acknowledgments--teşekkürler--agradecimientos)
- [Contact](#-contact--iletişim--contacto)

## 🌟 Features / Özellikler / Características

### 🤖 AI-Powered Generation / AI Destekli Oluşturma / Generación con IA
- **Advanced AI Integration**: Powered by Google's Gemini AI, providing state-of-the-art natural language processing capabilities for generating educational content.
  - Real-time content generation
  - Context-aware responses
  - Adaptive learning algorithms
  - Multi-language support
  - Custom content formatting

- **Smart Content Generation**: Utilizes advanced machine learning algorithms to create contextually relevant and educationally valuable flashcards.
  - Topic-specific content generation
  - Difficulty level adaptation
  - Content quality assurance
  - Educational value optimization
  - Interactive learning paths

- **Context-Aware Responses**: Implements sophisticated context understanding to generate flashcards that maintain educational coherence and progression.
  - Semantic understanding
  - Topic progression tracking
  - Learning path optimization
  - Content relevance scoring
  - Adaptive difficulty adjustment

- **Adaptive Learning**: Automatically adjusts content complexity based on user interaction and feedback.
  - User performance tracking
  - Difficulty scaling
  - Learning pace adaptation
  - Progress monitoring
  - Personalized recommendations

- **Multilingual Support**: Seamlessly generates content in multiple languages while maintaining educational quality.
  - Natural language processing
  - Cultural context awareness
  - Language-specific formatting
  - Translation quality assurance
  - Regional adaptation

### 🎨 User Interface / Kullanıcı Arayüzü / Interfaz de Usuario
- **Modern Dark Theme**: Implements a carefully designed dark theme that reduces eye strain during extended study sessions.
  - Custom color schemes
  - High contrast options
  - Accessibility features
  - Customizable themes
  - Responsive design

- **Responsive Design**: Fully responsive interface that adapts to various screen sizes and devices.
  - Mobile-first approach
  - Tablet optimization
  - Desktop enhancements
  - Touch interface support
  - Cross-platform compatibility

- **Interactive Chat Experience**: Real-time interaction with AI for dynamic flashcard generation.
  - Natural language input
  - Real-time feedback
  - Contextual suggestions
  - Interactive tutorials
  - Help system integration

- **Intuitive Navigation**: User-friendly interface with clear visual hierarchy and intuitive controls.
  - Clear menu structure
  - Quick access buttons
  - Search functionality
  - History tracking
  - Favorites system

- **Accessibility Features**: Implements WCAG 2.1 guidelines for better accessibility.
  - Screen reader support
  - Keyboard navigation
  - High contrast mode
  - Font size adjustment
  - Color blind friendly

### 📚 Customization / Özelleştirme / Personalización
- **Dynamic Flashcard Generation**: Create flashcards with customizable parameters:
  - Number of cards (1-50)
  - Difficulty level (Beginner to Advanced)
  - Content type (Definitions, Examples, Questions)
  - Language preference
  - Custom templates
  - Topic categories
  - Time limits
  - Review intervals

- **Multiple Language Support**: Comprehensive support for multiple languages with accurate translations.
  - Language detection
  - Automatic translation
  - Cultural adaptation
  - Regional variations
  - Language-specific formatting

- **Custom Topic Selection**: Generate flashcards for any subject or topic with specialized content adaptation.
  - Subject categorization
  - Topic tagging
  - Custom categories
  - Related topics
  - Topic difficulty levels

- **Export Options**: Multiple export formats including:
  - PDF (with custom templates)
  - CSV (with metadata)
  - Anki-compatible format
  - Plain text
  - HTML
  - JSON
  - XML
  - Markdown

### 🔒 Security / Güvenlik / Seguridad
- **Secure API Key Management**: Implements industry-standard security practices for API key handling.
  - Encrypted storage
  - Access control
  - Key rotation
  - Usage monitoring
  - Audit logging

- **Environment Variable Protection**: Secure storage of sensitive configuration data.
  - Variable encryption
  - Access restrictions
  - Secure defaults
  - Validation checks
  - Error handling

- **Data Privacy**: Implements strict data privacy measures:
  - No data collection
  - Local processing
  - Secure API communication
  - Data encryption
  - Privacy policy compliance

- **Regular Security Updates**: Continuous security monitoring and updates.
  - Vulnerability scanning
  - Patch management
  - Security audits
  - Compliance checks
  - Incident response

## 📸 Screenshots / Ekran Görüntüleri / Capturas de Pantalla

<div align="center">
  <img src="assets/screenshots/main-interface.png" alt="Main Interface" width="800"/>
  <p><em>Ana Arayüz / Main Interface / Interfaz Principal</em></p>
  
  <img src="assets/screenshots/flashcard-generation.png" alt="Flashcard Generation" width="800"/>
  <p><em>Flashcard Oluşturma / Flashcard Generation / Generación de Tarjetas</em></p>
  
  <img src="assets/screenshots/export-options.png" alt="Export Options" width="800"/>
  <p><em>Dışa Aktarma Seçenekleri / Export Options / Opciones de Exportación</em></p>
</div>

## 📖 English Documentation

### Detailed Setup Guide

#### System Requirements
- **Hardware Requirements**:
  - CPU: 2.0 GHz or higher
  - RAM: 4GB minimum (8GB recommended)
  - Storage: 500MB free space
  - Display: 1280x720 minimum resolution

- **Software Requirements**:
  - Operating System: Windows 10/11, macOS 10.15+, or Linux
  - Python 3.7 or higher
  - Modern web browser (Chrome, Firefox, Safari, Edge)
  - Git for version control

#### Advanced Installation

1. **Clone with Specific Branch**:
   ```bash
   git clone -b stable https://github.com/yourusername/flashcard_generator.git
   ```

2. **Create Virtual Environment with Specific Python Version**:
   ```bash
   python3.9 -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate     # Windows
   ```

3. **Install Dependencies with Version Control**:
   ```bash
   pip install -r requirements.txt --no-cache-dir
   ```

4. **Configure Environment Variables**:
   ```bash
   # Create .env file with all required variables
   cat > .env << EOL
   GOOGLE_API_KEY=your_api_key_here
   DEBUG_MODE=False
   MAX_CARDS=50
   DEFAULT_LANGUAGE=en
   EOL
   ```

5. **Verify Installation**:
   ```bash
   python -c "import streamlit; import google.generativeai; print('Installation successful!')"
   ```

### API Documentation

#### Authentication
```python
import os
from dotenv import load_dotenv

load_dotenv()
api_key = os.getenv('GOOGLE_API_KEY')
```

#### Basic Usage
```python
import streamlit as st
from flashcard_generator import FlashcardGenerator

# Initialize generator
generator = FlashcardGenerator(api_key=api_key)

# Generate flashcards
flashcards = generator.generate(
    topic="Python Programming",
    count=10,
    difficulty="intermediate",
    language="en"
)
```

#### Advanced Features
```python
# Custom template generation
flashcards = generator.generate_with_template(
    topic="Chemistry",
    template="definition_example",
    count=5
)

# Batch processing
results = generator.batch_generate([
    {"topic": "Math", "count": 5},
    {"topic": "Physics", "count": 5}
])
```

#### Error Handling
```python
try:
    flashcards = generator.generate(topic="History")
except APIError as e:
    st.error(f"API Error: {e}")
except ValidationError as e:
    st.error(f"Validation Error: {e}")
```

## 📖 Türkçe Dokümantasyon

### Ön Koşullar
- **Python Ortamı**:
  - Python 3.7 veya daha yüksek
  - pip (Python paket yöneticisi)
  - Sanal ortam desteği
- **API Gereksinimleri**:
  - Google Gemini API anahtarı
  - Aktif internet bağlantısı
- **Sistem Gereksinimleri**:
  - Minimum 4GB RAM
  - 500MB boş disk alanı
  - Modern web tarayıcı

### Kurulum Kılavuzu

1. **Depoyu Klonlayın**:
   ```bash
   git clone https://github.com/yourusername/flashcard_generator.git
   cd flashcard_generator
   ```

2. **Sanal Ortam Oluşturun**:
   ```bash
   # Windows
   python -m venv venv
   venv\Scripts\activate

   # Linux/Mac
   python -m venv venv
   source venv/bin/activate
   ```

3. **Bağımlılıkları Yükleyin**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Ortamı Yapılandırın**:
   ```bash
   # .env dosyası oluşturun
   echo "GOOGLE_API_KEY=your_api_key_here" > .env
   ```

### Kullanım Kılavuzu

1. **Uygulamayı Başlatın**:
   ```bash
   streamlit run app.py
   ```

2. **Uygulamaya Erişin**:
   ```
   http://localhost:8501
   ```

3. **Flashcard Oluşturun**:
   - Konunuzu girin
   - Kart sayısını seçin
   - Zorluk seviyesini belirleyin
   - "Oluştur" düğmesine tıklayın

4. **Dışa Aktarma Seçenekleri**:
   - "Dışa Aktar" düğmesine tıklayın
   - Format seçin
   - Dosyayı indirin

## 📖 Documentación en Español

[Previous Spanish documentation remains unchanged...]

[Rest of the content remains unchanged...]

## Contact / İletişim / Contacto

For questions and support, please contact:
- Email: celiker_samet@hotmail.com
- GitHub Issues: [Create an issue](https://github.com/yourusername/flashcard_generator/issues)
- LinkedIn: [Mert Samet Çeliker](https://www.linkedin.com/in/mert-samet-çeliker-18a906294/) 