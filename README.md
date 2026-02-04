# React Quiz App

A dynamic quiz application built with React that tests your knowledge of React concepts. This project demonstrates the use of React Context API for state management and includes features like timed questions, score tracking, and progress monitoring.

## Features

- **Interactive Quiz**: Multiple-choice questions about React
- **Timer**: Each quiz session has a countdown timer
- **Score Tracking**: Real-time score calculation based on correct answers
- **Progress Bar**: Visual feedback on quiz completion
- **Context API**: Global state management using React Context
- **Responsive Design**: Clean and modern UI that works on all devices

## Technologies Used

- React 18
- React Context API (useContext, useReducer)
- CSS3
- JSON for quiz data

## Project Structure

```
react-quiz/
├── public/
│   ├── index.html
│   └── ...
├── src/
│   ├── components/
│   │   ├── App.js
│   │   ├── Header.js
│   │   ├── Main.js
│   │   ├── Loader.js
│   │   ├── Error.js
│   │   ├── StartScreen.js
│   │   ├── Question.js
│   │   ├── Options.js
│   │   ├── NextButton.js
│   │   ├── Progress.js
│   │   ├── FinishScreen.js
│   │   ├── Timer.js
│   │   └── Footer.js
│   ├── contexts/
│   │   └── QuizContext.js
│   ├── index.css
│   └── index.js
├── data/
│   └── questions.json
├── package.json
└── README.md
```

## Getting Started

### Prerequisites

- Node.js (version 14 or higher)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/mohammedarafaa/react-quiz.git
```

2. Navigate to the project directory:
```bash
cd react-quiz
```

3. Install dependencies:
```bash
npm install
```

### Running the Application

Start the development server:
```bash
npm start
```

The app will open in your browser at [http://localhost:3000](http://localhost:3000)

### Building for Production

Create an optimized production build:
```bash
npm run build
```

## How It Works

1. **Start Screen**: Click "Let's start" to begin the quiz
2. **Questions**: Answer multiple-choice questions about React
3. **Timer**: Complete the quiz before time runs out
4. **Progress**: Track your progress with the visual progress bar
5. **Finish Screen**: View your final score and restart if desired

## State Management

This project uses React Context API with `useReducer` for centralized state management:

- **QuizContext**: Manages quiz state including questions, current question, answers, points, and timer
- **useReducer**: Handles complex state logic with actions like:
  - `dataReceived`: Load questions
  - `start`: Begin the quiz
  - `newAnswer`: Record user answer
  - `nextQuestion`: Move to next question
  - `finish`: End the quiz
  - `restart`: Reset the quiz
  - `tick`: Update timer

## Available Scripts

- `npm start` - Runs the app in development mode
- `npm test` - Launches the test runner
- `npm run build` - Builds the app for production
- `npm run eject` - Ejects from Create React App (one-way operation)

## Learning Outcomes

This project demonstrates:
- React Hooks (useState, useEffect, useReducer, useContext)
- Component composition and reusability
- Global state management with Context API
- Conditional rendering
- Event handling
- Timer implementation
- JSON data handling

## Credits

Original project from [Jonas Schmedtmann's Ultimate React Course](https://github.com/jonasschmedtmann/ultimate-react-course)

## License

This project is open source and available for educational purposes.

## Author

[Mohammed Arafa](https://github.com/mohammedarafaa)
