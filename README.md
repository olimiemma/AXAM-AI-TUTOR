# 🎓 AI Tutor for Grades 6-12(OFFLINE AS WELL)

An intelligent tutoring system that uses both OpenAI GPT and Ollama's Llama models to provide comprehensive, age-appropriate explanations for science and algebra concepts. Designed specifically for middle and high school students (ages 11-18).

## ✨ Features

### 🤖 Dual AI Architecture
- **Ollama Llama 3.2**: For local, privacy-focused tutoring
- **OpenAI GPT-4o-mini**: For high-quality, reliable explanations
- **Streaming Responses**: Real-time answer generation for better engagement

### 🎯 Pedagogical Excellence
- **Grade-Level Adaptation**: Tailored explanations for 6th-12th grade students
- **Multiple Learning Modalities**: Visual, auditory, and kinesthetic approaches
- **Real-World Applications**: Connects concepts to everyday life
- **Step-by-Step Breakdowns**: Clear, logical progression through complex topics
- **Cultural Inclusivity**: Diverse examples and culturally responsive teaching

### 📚 Subject Coverage
- **Mathematics**: Algebra, linear equations, quadratic functions, systems of equations
- **Science**: Chemistry, physics, biology (photosynthesis, chemical bonding)
- **Computer Science**: Code explanation and programming concepts

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- OpenAI API key
- Ollama installed locally

### Installation

1. **Clone the repository**
```bash
git clone <repository-url>
cd ollama-tutor
```

2. **Install dependencies**
```bash
pip install -r requirements.txt
```

3. **Set up environment variables**
```bash
cp .env.example .env
# Add your OpenAI API key to .env
OPENAI_API_KEY=your-api-key-here
```

4. **Set up Ollama**
```bash
# Install Ollama (if not already installed)
curl -fsSL https://ollama.ai/install.sh | sh

# Pull the Llama 3.2 model
ollama pull llama3.2
```

5. **Launch the notebook**
```bash
jupyter notebook "Ollama 6 to12 grade tutorchat.ipynb"
```

## 📖 Usage

### Interactive Chat Mode
```python
# Run the chat interface
chat_with_ollama()
```

Example session:
```
You: What is photosynthesis?
Ollama: Great question! Think of plants like solar-powered food factories...
```

### Single Question Mode
```python
# Ask a specific question
question = "Explain quadratic equations in simple terms"
# The system will provide a comprehensive, grade-appropriate explanation
```

### Customizable Teaching
- Modify `system_prompt` to adjust teaching style
- Change `MODEL_GPT` or `MODEL_LLAMA` to use different AI models
- Adjust grade level and complexity in the system prompt

## 🏗️ System Architecture

### Core Components
- **AI Integration**: Seamless switching between OpenAI and Ollama
- **Streaming Display**: Real-time Markdown rendering with IPython
- **Pedagogical Framework**: Evidence-based teaching strategies
- **Error Handling**: Robust API error management

### Teaching Methodology
The system implements proven educational strategies:
- **Scaffolding**: Gradual complexity progression
- **Multiple Modalities**: Visual, verbal, and practical explanations
- **Active Learning**: Interactive questioning and problem-solving
- **Differentiated Instruction**: Adapts to various learning levels

## 🎨 Example Explanations

### Mathematics
**Linear Equations**: Balance scale analogy with step-by-step solving
**Quadratic Functions**: Real-world applications (basketball shots, bridge design)
**Systems of Equations**: Practical scenarios (fundraiser planning, chemistry mixtures)

### Science
**Photosynthesis**: Solar-powered factory metaphor
**Chemical Bonding**: "Party analogy" for atomic interactions
**Physics Concepts**: Everyday examples and visual descriptions

## ⚙️ Configuration

### Environment Variables
```env
OPENAI_API_KEY=your_openai_api_key
OLLAMA_API=http://localhost:11434/api/chat
```

### Model Settings
```python
MODEL_GPT = 'gpt-4o-mini'
MODEL_LLAMA = 'llama3.2'
```

## 🔧 Customization

### Adapting for Different Grade Levels
Modify the `system_prompt` to adjust:
- Language complexity
- Example sophistication
- Mathematical notation level
- Real-world application depth

### Adding New Subjects
Extend the system prompt to include:
- New subject domains
- Grade-appropriate examples
- Common misconceptions
- Relevant teaching strategies

## 📊 Performance

### Response Quality
- **OpenAI GPT**: High accuracy, comprehensive explanations
- **Ollama Llama**: Good performance for local processing
- **Streaming**: Enhanced user engagement through real-time display

### Educational Value
- **Age-Appropriate**: Tailored for 6th-12th grade comprehension
- **Engaging**: Uses metaphors, analogies, and real-world connections
- **Comprehensive**: Multiple approaches to each concept
- **Supportive**: Encouraging tone with error analysis

## 🛠️ Development

### File Structure
```
ollama-tutor/
├── Ollama 6 to12 grade tutorchat.ipynb
├── requirements.txt
├── .env.example
└── README.md
```

### Dependencies
- `openai`: OpenAI API integration
- `ollama`: Local LLM interaction
- `python-dotenv`: Environment management
- `IPython`: Interactive display features
- `requests`: HTTP API calls

## 🤝 Contributing

We welcome contributions to enhance:
- Teaching methodologies
- Subject coverage
- User interface
- Performance optimization

### Areas for Improvement
- Additional subject domains
- Multilingual support expansion
- Assessment integration
- Parent/teacher dashboard

## 📄 License

This project is designed for educational purposes. Please ensure compliance with:
- OpenAI usage policies
- Ollama terms of service
- Local educational regulations

## 🙏 Acknowledgements

- **OpenAI** for GPT model access
- **Ollama** for local LLM capabilities
- **Educational researchers** whose pedagogical strategies informed the teaching methodology

## 🆘 Support

### Common Issues
1. **API Key Problems**: Verify format and environment variable setup
2. **Ollama Connection**: Ensure Ollama service is running on port 11434
3. **Model Download**: Use `ollama pull llama3.2` if model not found

### Troubleshooting
- Check the troubleshooting notebook in the repository
- Verify all dependencies are installed
- Ensure proper internet connectivity for API calls

---

**Start empowering students with AI-powered tutoring today!** 🚀

*Note: Always supervise AI interactions in educational settings and verify content accuracy for critical learning objectives.*
