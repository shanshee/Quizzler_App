#Quiz App with Open Trivia Database API

This repository contains a Python-based quiz application that fetches trivia questions from the Open Trivia Database API (opentdb.com). The app allows users to answer boolean-type (True/False) questions from a specified category.

![Screenshot 2024-05-05 001109](https://github.com/shanshee/Quizzler_App/assets/135793255/1eec0b29-7250-4595-a2f5-57773cf0c47d)

Code Sections
1. Fetching Quiz Questions from API
The fetch_questions.py script utilizes the requests library to send a GET request to the Open Trivia Database API. It retrieves a set of 10 boolean-type questions from a chosen category (Category ID: 18). The fetched data is processed and stored in the question_data variable for further use in the quiz.

2. Quiz Logic and Question Handling
The quiz_brain.py module defines the QuizBrain class responsible for managing the quiz's logic. It maintains the user's score, tracks the current question number, and handles user input and answer verification. The still_has_questions() method checks if there are remaining questions, while next_question() retrieves the next question and its unescaped text from the question_data. The check_answer() method verifies the user's response against the correct answer.

3. User Interface for the Quiz
The quiz_ui.py module contains the QuizInterface class that presents the quiz to the user. It displays each question using the tkinter library and gathers the user's input. The user's score is updated based on their answers, and the quiz progresses until all questions are answered.

Running the Quiz
To run the quiz, execute the main.py script. The application fetches quiz questions from the API, presents them to the user, and provides instant feedback on their answers. Have fun testing your knowledge with the quiz!
![Screenshot 2024-05-05 001003](https://github.com/shanshee/Quizzler_App/assets/135793255/83bfb49a-e073-45fe-8f90-14e99bb1e265)

