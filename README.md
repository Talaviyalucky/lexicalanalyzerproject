# Lexical Analyzer

A comprehensive Lexical Analyzer tool that identifies tokens in various programming languages including C, Java, Python, and JavaScript.

## 🚀 Features

- **Multi-language Support**: Analyze code written in C, Java, Python, and JavaScript.
- **Auto-detection**: Automatically detects the programming language based on code snippets.
- **Validation**: Ensures the selected language matches the input code.
- **Token Classification**: Identifies and classifies tokens into:
  - Keywords
  - Identifiers
  - Operators (Relational, Assignment, etc.)
  - Literals (Strings, Constants)
  - Preprocessor Directives (C)
  - Separators & Brackets
- **Backend Storage**: Save analysis results for future reference.

## 🛠️ Tech Stack

- **Frontend**: React.js
- **Backend**: Node.js, Express.js
- **Database**: MongoDB (via Mongoose)
- **Styling**: CSS3

## 📂 Project Structure

```text
lexical-analyzer/
├── backend/            # Express.js backend
│   ├── models/        # Mongoose schemas
│   ├── routes/        # API endpoints
│   └── server.js      # Entry point for backend
├── public/             # Static assets
└── src/                # React frontend
    ├── compiler/       # Core Lexer logic
    ├── components/     # UI Components
    └── App.js          # Main React component
```

## ⚙️ Installation & Setup

### Prerequisites

- Node.js (v14 or higher)
- MongoDB

### Steps

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd lexical-analyzer
   ```

2. **Setup Backend**

   ```bash
   cd lexical-analyzer/backend
   npm install
   ```

   Create a `.env` file in the `backend` folder and add your MongoDB URI:

   ```env
   MONGO_URI=your_mongodb_connection_string
   PORT=5001
   ```

   Start the backend server:

   ```bash
   npm start
   ```

3. **Setup Frontend**
   ```bash
   cd ../lexical-analyzer
   npm install
   npm start
   ```
   The application will be available at `http://localhost:3000`.

## 📖 Usage

1. Open the application in your browser.
2. Select the programming language from the dropdown (or let auto-detection work).
3. Paste your code into the input box.
4. View the generated token table showing the lexeme, token type, and matching pattern.
5. (Optional) Save the analysis to the database.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
