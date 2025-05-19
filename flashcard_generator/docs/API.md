# API Documentation / API Dokümantasyonu / Documentación de API

## Overview / Genel Bakış / Descripción General

The Flashcard Generator API provides a comprehensive interface for generating educational flashcards using Google's Gemini AI. This documentation details all available endpoints, parameters, and response formats.

## Authentication / Kimlik Doğrulama / Autenticación

### API Key Setup / API Anahtarı Kurulumu / Configuración de Clave API

```python
import os
from dotenv import load_dotenv

load_dotenv()
api_key = os.getenv('GOOGLE_API_KEY')
```

### Headers / Başlıklar / Encabezados

```python
headers = {
    'Authorization': f'Bearer {api_key}',
    'Content-Type': 'application/json'
}
```

## Core Functions / Temel Fonksiyonlar / Funciones Principales

### Generate Flashcards / Flashcard Oluşturma / Generar Tarjetas

```python
def generate_flashcards(
    topic: str,
    count: int = 10,
    difficulty: str = "intermediate",
    language: str = "en"
) -> List[Dict[str, str]]:
    """
    Generate flashcards for a given topic.
    
    Args:
        topic (str): The topic to generate flashcards for
        count (int): Number of flashcards to generate (1-50)
        difficulty (str): Difficulty level (beginner/intermediate/advanced)
        language (str): Language code (en/tr/es)
    
    Returns:
        List[Dict[str, str]]: List of flashcards with front and back content
    """
```

### Example Usage / Örnek Kullanım / Ejemplo de Uso

```python
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

## Advanced Features / Gelişmiş Özellikler / Características Avanzadas

### Custom Templates / Özel Şablonlar / Plantillas Personalizadas

```python
def generate_with_template(
    topic: str,
    template: str,
    count: int = 5
) -> List[Dict[str, str]]:
    """
    Generate flashcards using a custom template.
    
    Args:
        topic (str): The topic to generate flashcards for
        template (str): Template name or path
        count (int): Number of flashcards to generate
    
    Returns:
        List[Dict[str, str]]: List of flashcards with custom format
    """
```

### Batch Processing / Toplu İşleme / Procesamiento por Lotes

```python
def batch_generate(
    requests: List[Dict[str, Any]]
) -> List[List[Dict[str, str]]]:
    """
    Generate multiple sets of flashcards in batch.
    
    Args:
        requests (List[Dict]): List of generation requests
    
    Returns:
        List[List[Dict]]: List of flashcard sets
    """
```

## Error Handling / Hata Yönetimi / Manejo de Errores

### Common Errors / Yaygın Hatalar / Errores Comunes

```python
class APIError(Exception):
    """Base class for API errors"""
    pass

class ValidationError(APIError):
    """Raised when input validation fails"""
    pass

class RateLimitError(APIError):
    """Raised when API rate limit is exceeded"""
    pass
```

### Error Handling Example / Hata Yönetimi Örneği / Ejemplo de Manejo de Errores

```python
try:
    flashcards = generator.generate(topic="History")
except APIError as e:
    print(f"API Error: {e}")
except ValidationError as e:
    print(f"Validation Error: {e}")
except RateLimitError as e:
    print(f"Rate Limit Error: {e}")
```

## Response Formats / Yanıt Formatları / Formatos de Respuesta

### Standard Response / Standart Yanıt / Respuesta Estándar

```json
{
    "flashcards": [
        {
            "front": "Question or term",
            "back": "Answer or definition",
            "metadata": {
                "difficulty": "intermediate",
                "category": "programming",
                "tags": ["python", "basics"]
            }
        }
    ],
    "metadata": {
        "count": 10,
        "language": "en",
        "generated_at": "2024-03-XX"
    }
}
```

## Rate Limits / Hız Sınırları / Límites de Tasa

- 100 requests per minute
- 1000 requests per hour
- 10000 requests per day

## Best Practices / En İyi Uygulamalar / Mejores Prácticas

1. Always handle errors appropriately
2. Implement rate limiting in your application
3. Cache responses when possible
4. Use batch processing for multiple requests
5. Validate input before sending requests

## Versioning / Sürümleme / Versionado

The API version is specified in the request header:

```python
headers = {
    'Authorization': f'Bearer {api_key}',
    'Content-Type': 'application/json',
    'X-API-Version': '1.0.0'
}
```

## Support / Destek / Soporte

For API support, please contact:
- Email: your.email@example.com
- GitHub Issues: [Create an issue](https://github.com/yourusername/flashcard_generator/issues)
- LinkedIn: [Mert Samet Çeliker](https://www.linkedin.com/in/mert-samet-çeliker-18a906294/) 