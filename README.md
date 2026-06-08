# MultiAgent Financial System
**AI Agent in Asset Management**

## 🎯 Project Overview

**MultiAgent Financial System** is an AI-powered asset management platform that demonstrates:
- **Multi-agent architecture** with specialized financial analysis agents
- **LLM integration** (Google Gemini) for intelligent decision-making
- **Full-stack development** (FastAPI backend + Streamlit frontend)
- **Real-world data integration** (yfinance, Alpha Vantage APIs)
- **Production-ready architecture** with scalable design

**Tech Stack**: Python, FastAPI, Streamlit, Google Gemini AI, pandas, scikit-learn, numpy

---

## ✨ Key Features

- **Multi-Agent Analysis**: Specialized agents for different financial metrics and analysis
- **Real-Time Data**: Live stock data via yfinance and Alpha Vantage APIs
- **AI-Powered Insights**: Leverages Google Gemini for intelligent financial analysis
- **Interactive Dashboard**: Streamlit-based frontend for easy visualization and interaction
- **REST API Backend**: FastAPI backend for programmatic access and scalability
- **Scalable Architecture**: Designed for team integration and system expansion
- **Data Pipeline**: ETL workflow for financial data processing and preparation

---

## 🛠️ Technical Highlights

- **Architecture**: Microservices-ready with separate backend and frontend layers
- **AI Integration**: Demonstrates prompt engineering and LLM orchestration
- **Data Pipeline**: ETL workflow for financial data processing
- **API Design**: RESTful API with proper separation of concerns
- **Modern Stack**: FastAPI, Streamlit, and contemporary Python libraries
- **Financial Analysis**: Integration with industry-standard financial APIs

---

## 📚 Resources & Documentation

### Financial Data APIs
- **yfinance**: https://ranaroussi.github.io/yfinance/reference/index.html
- **Alpha Vantage**: https://www.alphavantage.co/documentation/

### AI Model
- **Google Gemini**: https://aistudio.google.com/
- ⚠️ **Security Note**: Keep your API keys private and never commit them to version control

### Technical Report
- **Full Analysis**: [Finance & Technical Analysis Report](Finance%20%26%20Technical%20analysis.pdf)

---

## 🏗️ System Architecture

![System Architecture](Basic%20Structure.jpg)

---

## 📋 Project Workflow

### Phase 1: Individual Agent Development
1. **Fetch Financial Data**: Download stock data using yfinance and Alpha Vantage APIs
2. **Data Preparation**: Clean and process the data for AI analysis
3. **Build AI Agent**: Create your agent with custom instructions and prompts
4. **Test & Iterate**: Validate outputs and refine the agent as needed

### Phase 2: Integration & Reporting
5. **Consolidate Requirements**: Team discussion on which agents/features to include
6. **Integrate Agents**: Combine individual agents into a unified system
7. **Generate Reports**: Produce research analysis from the integrated system
8. **Final Deliverables**: Complete coursework report and presentation

---

## 🚀 Installation & Setup

### Prerequisites
- **Python 3.10** or higher
- **Two terminal windows** (for backend and frontend)
- **Internet connection** (for API access)

### Step-by-Step Instructions

#### 1. Clone the Repository
```bash
git clone https://github.com/Showgath/MultiAgent-Financial-Sysytem.git
cd MultiAgent-Financial-Sysytem
```

#### 2. Create a Virtual Environment (Recommended)
```bash
python -m venv venv
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
```

#### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

#### 4. Configure API Keys
1. Open `main/APIKey.py`
2. Add your **Google Gemini API key** (get it from https://aistudio.google.com/)
3. Add your **Alpha Vantage API key** (get it from https://www.alphavantage.co/)

**Alternative (Recommended for security)**: Use `.env` file
- Copy `main/.env.example` to `main/.env`
- Add your API keys to the `.env` file
- Update `APIKey.py` to load from environment variables

#### 5. Launch the Application
**Open Two Terminal Windows**:

**Terminal 1 - Backend Server**:
```bash
cd main
uvicorn server:app --reload
```
Backend will run at: `http://localhost:8000`

**Terminal 2 - Frontend Dashboard**:
```bash
cd main
streamlit run app.py
```
Frontend will open at: `http://localhost:8501`

#### 6. Access the Application
- **Frontend Dashboard**: http://localhost:8501
- **Backend API**: http://localhost:8000
- **API Documentation**: http://localhost:8000/docs

---

## 💡 Usage Tips

- **Keep terminals running**: Ensure both backend and frontend terminals are active simultaneously
- **API Rate Limits**: Be aware of rate limits on yfinance and Alpha Vantage free tiers
- **Security**: Never hardcode API keys; use environment variables or `.env` files
- **Debugging**: Check terminal outputs for error messages and API responses

---

## 📁 Project Structure

```
MultiAgent-Financial-Sysytem/
├── README.md                              # This file
├── LICENSE                                # MIT License
├── CONTRIBUTING.md                        # Contribution guidelines
├── requirements.txt                       # Root dependencies
├── .gitignore                            # Git ignore rules
├── Basic Structure.jpg                   # Architecture diagram
├── Finance & Technical analysis.pdf      # Technical documentation
│
├── main/                                 # Main application folder
│   ├── requirements.txt                  # Additional dependencies
│   ├── APIKey.py                         # API key configuration
│   ├── .env.example                      # Environment variables template
│   ├── server.py                         # FastAPI backend
│   └── app.py                            # Streamlit frontend
│
├── prototype/                            # Prototype experiments
└── investment memo/                      # Investment analysis documents
```

---

## 🚀 Future Enhancements

- [ ] Portfolio optimization algorithm
- [ ] Machine learning model for price prediction
- [ ] Database integration for historical analysis
- [ ] Enhanced error handling and logging
- [ ] Unit tests and CI/CD pipeline
- [ ] Docker containerization for deployment
- [ ] Authentication and user management
- [ ] Real-time notifications for market alerts

---

## 📊 Skills Demonstrated

This project showcases proficiency in:

✅ **Full-Stack Python Development** - Backend and frontend integration  
✅ **AI/LLM Integration** - Google Gemini API orchestration  
✅ **API Design** - RESTful APIs with FastAPI  
✅ **Frontend Development** - Interactive dashboards with Streamlit  
✅ **Financial Data Analysis** - pandas, numpy, technical analysis  
✅ **Multi-Agent Architecture** - Scalable, modular design  
✅ **Professional Documentation** - Clear, comprehensive guides  
✅ **Software Engineering Best Practices** - Version control, dependencies, security  

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/YourFeatureName`)
3. Commit your changes (`git commit -m 'Add YourFeatureName'`)
4. Push to the branch (`git push origin feature/YourFeatureName`)
5. Open a Pull Request

For detailed guidelines, see [CONTRIBUTING.md](CONTRIBUTING.md).

---

## 📜 License

This project is open source and available under the [MIT License](LICENSE).

---

## 📧 Support & Questions

For questions or issues:
- Check the [Technical Report](Finance%20%26%20Technical%20analysis.pdf)
- Review the [Architecture Diagram](Basic%20Structure.jpg)
- Open an issue on GitHub

---

**Last Updated**: June 2026  
**Project Status**: Active Development
