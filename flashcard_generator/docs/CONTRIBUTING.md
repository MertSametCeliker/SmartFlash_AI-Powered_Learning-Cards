# Contributing Guide / Katkıda Bulunma Kılavuzu / Guía de Contribución

## Code of Conduct / Davranış Kuralları / Código de Conducta

Please read our [Code of Conduct](CODE_OF_CONDUCT.md) before contributing.

## How to Contribute / Nasıl Katkıda Bulunulur / Cómo Contribuir

### 1. Fork the Repository / Depoyu Çatallayın / Bifurcar el Repositorio

1. Go to [flashcard_generator](https://github.com/yourusername/flashcard_generator)
2. Click the "Fork" button
3. Clone your fork:
   ```bash
   git clone https://github.com/yourusername/flashcard_generator.git
   ```

### 2. Set Up Development Environment / Geliştirme Ortamını Kurun / Configurar Entorno de Desarrollo

```bash
# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # or .\venv\Scripts\activate on Windows

# Install dependencies
pip install -r requirements.txt
pip install -r requirements-dev.txt

# Install pre-commit hooks
pre-commit install
```

### 3. Create a Branch / Dal Oluşturun / Crear una Rama

```bash
git checkout -b feature/your-feature-name
```

### 4. Make Changes / Değişiklikler Yapın / Realizar Cambios

1. Write your code
2. Add tests
3. Update documentation
4. Run tests:
   ```bash
   pytest tests/
   ```
5. Run linting:
   ```bash
   flake8
   black .
   isort .
   ```

### 5. Commit Changes / Değişiklikleri Kaydedin / Confirmar Cambios

```bash
git add .
git commit -m "feat: add new feature"
```

### 6. Push Changes / Değişiklikleri Gönderin / Enviar Cambios

```bash
git push origin feature/your-feature-name
```

### 7. Create Pull Request / Pull Request Oluşturun / Crear Pull Request

1. Go to your fork on GitHub
2. Click "New Pull Request"
3. Select the main repository as the base
4. Add description of changes
5. Submit pull request

## Development Guidelines / Geliştirme Kuralları / Pautas de Desarrollo

### Code Style / Kod Stili / Estilo de Código

- Follow PEP 8 guidelines
- Use type hints
- Write docstrings for all functions
- Keep functions small and focused
- Use meaningful variable names

### Testing / Test Etme / Pruebas

- Write unit tests for new features
- Maintain test coverage above 80%
- Include integration tests for API endpoints
- Test edge cases and error conditions

### Documentation / Dokümantasyon / Documentación

- Update README.md for major changes
- Document new features in API.md
- Add docstrings to new functions
- Update type hints
- Include usage examples

### Git Workflow / Git İş Akışı / Flujo de Trabajo Git

1. Use feature branches
2. Write clear commit messages
3. Keep commits atomic
4. Rebase before submitting PR
5. Squash commits when appropriate

## Pull Request Process / Pull Request Süreci / Proceso de Pull Request

1. Update documentation
2. Add tests
3. Ensure CI passes
4. Get code review
5. Address feedback
6. Merge when approved

## Review Process / İnceleme Süreci / Proceso de Revisión

1. Code review by maintainers
2. Automated checks:
   - Tests
   - Linting
   - Type checking
   - Documentation
3. Manual review:
   - Code quality
   - Architecture
   - Security
   - Performance

## Release Process / Sürüm Süreci / Proceso de Lanzamiento

1. Update version number
2. Update changelog
3. Create release notes
4. Tag release
5. Deploy to PyPI

## Communication / İletişim / Comunicación

- Use GitHub Issues for bugs
- Use GitHub Discussions for ideas
- Join our [Discord server](https://discord.gg/your-server)
- Follow our [blog](https://your-blog.com)

## Recognition / Tanınma / Reconocimiento

- Contributors will be listed in README.md
- Significant contributions will be highlighted
- Regular contributors may become maintainers

## Questions? / Sorularınız mı var? / ¿Preguntas?

Contact us:
- Email: your.email@example.com
- GitHub Issues: [Create an issue](https://github.com/yourusername/flashcard_generator/issues)
- LinkedIn: [Mert Samet Çeliker](https://www.linkedin.com/in/mert-samet-çeliker-18a906294/) 