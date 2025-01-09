
# 🧮 Smart Math Expression Calculator (AI-Powered-Dynamic-Calculator)

An intelligent mathematical expression calculator that combines the power of React, FastAPI, and Google's Gemini AI to solve various mathematical problems through image recognition. This full-stack application can handle everything from simple arithmetic to complex equations and even interpret mathematical concepts from drawings.

## ✨ Features

- **Multi-Expression Recognition**: Process various types of mathematical expressions:
  - Basic arithmetic operations
  - Variable assignments
  - Systems of equations
  - Graphical math problems
  - Abstract mathematical concepts
- **Variable Management**: Store and reuse variables across calculations
- **Smart PEMDAS Implementation**: Follows standard order of operations
- **Modern React Frontend**: Built with Vite, TypeScript, and Tailwind CSS
- **Powerful Backend**: FastAPI-based REST API with Google Gemini AI integration
- **Real-time Processing**: Instant feedback on calculations

## 🛠️ Tech Stack

### Frontend
- React 18.x
- TypeScript
- Vite
- Tailwind CSS
- Mantine UI
- ShadcnUI Components
- React Router DOM

### Backend
- FastAPI
- Google Generative AI (Gemini-1.5-flash)
- Python 3.x
- Pillow for image processing
- Uvicorn server

## 📋 Prerequisites

- Node.js (v16 or higher)
- Python 3.8+
- Google Gemini API key
- npm or yarn package manager

## 🚀 Installation

### Backend Setup

1. Clone the repository:
```bash
git clone https://github.com/priyanshu/smart-math-calculator.git
cd smart-math-calculator
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install Python dependencies:
```bash
pip install -r requirements.txt
```

4. Create a `.env` file in the root directory:
```env
GEMINI_API_KEY=your_gemini_api_key
```

### Frontend Setup

1. Navigate to the frontend directory:
```bash
cd frontend
```

2. Install dependencies:
```bash
npm install
# or
yarn install
```

3. Create a `.env` file in the frontend directory:
```env
VITE_API_URL=http://localhost:8900
```

## 🏃‍♂️ Running the Application

### Start the Backend Server
```bash
python main.py
```
The server will start at `http://localhost:8900`

### Start the Frontend Development Server
```bash
npm run dev
# or
yarn dev
```
The frontend will be available at `http://localhost:5173`

## 🔍 How It Works

1. **Image Processing**:
   - Upload an image containing mathematical expressions
   - The image is converted to base64 and sent to the backend
   - Backend processes the image using Pillow

2. **AI Analysis**:
   - Google Gemini AI analyzes the image content
   - Identifies mathematical expressions and their context
   - Applies PEMDAS rules for calculations

3. **Response Processing**:
   - Results are formatted into structured JSON
   - Supports multiple expression types
   - Handles variable assignments and references

4. **Frontend Display**:
   - Real-time updates of calculations
   - Elegant UI with Mantine and ShadcnUI
   - Responsive design for all devices

## 📝 API Endpoints

- `POST /calculate`: Process image and return mathematical results
  - Request Body: `ImageData` (image in base64 format and variables dictionary)
  - Response: Calculated results with expressions and answers

## 🔐 Security

- CORS middleware enabled
- API key validation for Gemini AI
- Input sanitization and validation

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/AmazingFeature`
3. Commit your changes: `git commit -m 'Add some AmazingFeature'`
4. Push to the branch: `git push origin feature/AmazingFeature`
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🌟 Keywords
mathematical expression calculator, image recognition math solver, Google Gemini AI, React calculator, FastAPI math API, equation solver, mathematical OCR, PEMDAS calculator, variable expression solver, graphical math solver, TypeScript calculator, Vite React application, math expression parser

## 🔮 Future Enhancements

- Support for more complex mathematical notations
- Integration with multiple AI models
- Step-by-step solution explanations
- Mathematical expression history
- Export calculations to PDF
- Mobile application support
- Offline processing capabilities

## ⚠️ Known Issues

- Large images may take longer to process
- Certain complex mathematical notations might need manual verification
- Variable scope is limited to single sessions

## 📞 Support

For support, please open an issue in the GitHub repository or contact the maintainers.
