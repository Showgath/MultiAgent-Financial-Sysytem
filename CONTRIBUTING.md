# Contributing to MultiAgent Financial System

Thank you for your interest in contributing! This document provides guidelines and instructions for contributing to this project.

## 🤝 How to Contribute

### 1. Fork and Clone
```bash
git clone https://github.com/YourUsername/MultiAgent-Financial-Sysytem.git
cd MultiAgent-Financial-Sysytem
```

### 2. Create a Feature Branch
```bash
git checkout -b feature/your-feature-name
```

Use descriptive branch names:
- `feature/add-portfolio-optimization`
- `bugfix/fix-api-connection`
- `docs/update-installation-guide`

### 3. Make Your Changes
- Write clean, readable code
- Add comments for complex logic
- Follow PEP 8 style guide
- Test your changes thoroughly

### 4. Commit Your Changes
```bash
git commit -m "Brief description of changes"
```

Use clear commit messages:
- ✅ Good: `feat: add portfolio optimization algorithm`
- ✅ Good: `fix: resolve API timeout issues`
- ❌ Bad: `update stuff`

### 5. Push and Open a Pull Request
```bash
git push origin feature/your-feature-name
```

Then open a Pull Request on GitHub with:
- Clear title describing the change
- Description of what was changed and why
- Reference to any related issues

---

## 📋 Before You Submit

- [ ] Code follows PEP 8 style guide
- [ ] Changes are tested and working
- [ ] Documentation is updated if needed
- [ ] No hardcoded API keys or secrets
- [ ] `.env` files are not committed

---

## 🎯 Areas for Contribution

### High Priority
- [ ] Unit tests (test coverage)
- [ ] Error handling improvements
- [ ] Documentation updates
- [ ] Bug fixes

### Medium Priority
- [ ] Performance optimizations
- [ ] Additional financial indicators
- [ ] Enhanced visualization
- [ ] Code refactoring

### Future Ideas
- [ ] Database integration
- [ ] Docker containerization
- [ ] Deployment to cloud
- [ ] Mobile app version
- [ ] Real-time notifications

---

## 💻 Development Setup

```bash
# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Copy environment template
cp main/.env.example main/.env

# Add your API keys to main/.env

# Run the application
cd main
# Terminal 1:
uvicorn server:app --reload
# Terminal 2:
streamlit run app.py
```

---

## 🧪 Testing

Please test your changes before submitting:

```bash
# Manual testing
python -m pytest tests/

# Check code style
flake8 main/

# Type checking
mypy main/
```

---

## 📝 Code Style Guidelines

### Python
- Follow PEP 8
- Use meaningful variable names
- Add docstrings to functions
- Use type hints where possible

### Example Function:
```python
def fetch_stock_data(symbol: str, period: str = "1y") -> dict:
    """
    Fetch stock data from yfinance.
    
    Args:
        symbol (str): Stock ticker symbol (e.g., 'AAPL')
        period (str): Data period (default: '1y')
    
    Returns:
        dict: Stock data with OHLCV values
    """
    # Implementation here
    pass
```

---

## 🐛 Reporting Issues

If you find a bug:

1. Check if it's already reported in Issues
2. Create a new issue with:
   - Clear title
   - Steps to reproduce
   - Expected vs. actual behavior
   - Python version and OS
   - Error messages/logs

---

## 📚 Documentation

When adding features:
- Update README.md if needed
- Add docstrings to code
- Include usage examples
- Update this CONTRIBUTING.md if process changes

---

## 🚀 Getting Help

- Review the [Technical Report](Finance%20%26%20Technical%20analysis.pdf)
- Check existing issues and PRs
- Read the main [README.md](README.md)
- Ask questions in Issues

---

## 📜 License

By contributing, you agree that your contributions will be licensed under the MIT License.

---

Thank you for contributing! 🎉
