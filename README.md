# AI Code Reviewer

## Description

AI Code Reviewer is a MERN stack web application that reviews input code and provides detailed feedback on improvements, style, performance, security, and readability.

## Tech Stack

- **MongoDB**: Database (if needed for saving reviews or user data)
- **Express**: Backend web framework
- **React**: Frontend framework
- **Node.js**: JavaScript runtime
- **Additional Libraries & Tools**:
  - Google Generative AI for code reviews
  - Axios for API calls
  - PrismJS for syntax highlighting
  - Vite for fast React development
  - Cors for handling cross-origin requests
  - dotenv for environment variable management

## Installation Instructions

### Prerequisites

- Node.js (v14+)
- npm (v6+)

### Clone the Repository

```sh
git clone <repository-url>
cd ai_code_reviewer
```

### Backend Setup

1. Navigate to the Backend directory:
   ```sh
   cd Backend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Create a `.env` file with the following content:
   ```env
   GOOGLE_GEMINI_KEY=your_google_gemini_api_key_here
   ```
4. Start the backend server:
   ```sh
   npm start
   ```
   _Or if using nodemon:_
   ```sh
   npx nodemon server.js
   ```

### Frontend Setup

1. Open a new terminal window and navigate to the Frontend directory:
   ```sh
   cd Frontend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Start the development server:
   ```sh
   npm run dev
   ```

## Usage

- Open your browser and navigate to the Frontend URL (typically [http://localhost:3000](http://localhost:3000) or the port provided by Vite).
- Enter some code in the provided editor and click the "Review" button to get AI-powered feedback.

## Folder Structure

```
ai_code_reviewer/
├── .gitignore
├── Readme.md
├── Backend/
│   ├── .env
│   ├── package.json
│   ├── server.js
│   └── src/
│       ├── app.js
│       ├── controllers/
│       │   └── ai.controller.js
│       ├── routes/
│       │   └── ai.routes.js
│       └── services/
│           └── ai.service.js
└── Frontend/
    ├── .gitignore
    ├── package.json
    ├── vite.config.js
    ├── public/
    └── src/
        ├── App.jsx
        ├── main.jsx
        └── assets/
```

## Additional Information

- Customize the system instruction in `Backend/src/services/ai.service.js` as needed.
- Make sure environment variables are set correctly in the Backend to use the Google Generative AI service.
