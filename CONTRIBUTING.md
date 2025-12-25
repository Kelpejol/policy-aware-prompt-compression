# Contributing to Prompt Compression Gateway

Thanks for your interest in contributing! This document provides guidelines for contributions.

## How to Contribute

### Reporting Bugs

- Check if the bug already exists in [Issues](../../issues)
- Use the bug report template
- Include reproduction steps, expected vs actual behavior
- Add relevant logs and environment info

### Suggesting Features

- Check existing [Issues](../../issues) and [Discussions](../../discussions)
- Describe the problem you're solving
- Explain your proposed solution
- Consider backward compatibility

### Pull Requests

1. **Fork the repository**

2. **Create a branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make your changes**
   - Write clear, documented code
   - Add tests for new features
   - Update documentation if needed

4. **Test your changes**
   ```bash
   pytest
   black gateway/ tests/
   ruff check gateway/ tests/
   ```

5. **Commit with clear messages**
   ```bash
   git commit -m "feat: add new compression algorithm"
   ```

6. **Push and create PR**
   ```bash
   git push origin feature/your-feature-name
   ```

## Development Setup

```bash
# Clone your fork
git clone https://github.com/your-username/prompt-compression-gateway.git
cd prompt-compression-gateway

# Create virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements-dev.txt

# Run tests
pytest
```

## Code Style

- Follow PEP 8
- Use type hints
- Write docstrings for functions
- Format with Black: `black gateway/ tests/`
- Lint with Ruff: `ruff check gateway/ tests/`

## Commit Messages

Use conventional commit format:

- `feat:` New feature
- `fix:` Bug fix
- `docs:` Documentation changes
- `test:` Test additions/changes
- `refactor:` Code refactoring
- `chore:` Maintenance tasks

Example: `feat: add batch compression endpoint`

## Questions?

- Open a [Discussion](../../discussions)
- Check existing [Issues](../../issues)

Thank you for contributing! 🎉
