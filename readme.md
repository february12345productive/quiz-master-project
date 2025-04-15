Quiz master, interactive quiz game:

Quiz Master is a Python-based console quiz game designed to test knowledge in two areas: Current Affairs and General Knowledge. The game uses simple text files to store the quiz questions and answers, and it supports multiple rounds with dynamic scoring, interactive feedback, and a leaderboard to track high scores.

Features:-
File Structure:-
How It Works:-

Features:
Two Quiz Modes;
 Play quizzes in Current Affairs or General Knowledge.
Interactive Gameplay;
 Receive instant feedback with encouraging messages for correct and incorrect answers.
Multiple Attempts;
 Users get up to 3 attempts per question with partial credit for retries.
Leaderboard;
 Each round's score is timestamped and appended to a leaderboard file (score_leaderboard.txt), allowing you to track your best scores.
Round Summary;
 View the score summary across multiple quiz rounds.
User-Friendly Interface;
 Clear instructions and prompts guide you through the game.

File Structure:
The project contains several key files:
quiz_master.py;
  Main Python file that contains all the quiz logic and game play functionality. It handles user input, question display, scoring, and updating the leaderboard.

current.txt;
  Contains Current Affairs quiz questions and their options. Each question is followed by four answer choices (labeled A, B, C, D).

current_answers.txt;
  Contains the corresponding correct answers (one answer per question) for the Current Affairs quiz. Answers are normalized (in uppercase) for consistent comparisons.

general.txt;
  Contains General Knowledge quiz questions with multiple choice answers.

general_answers.txt;
  Contains the correct answers for the General Knowledge quiz questions.

score_leaderboard.txt (Generated at runtime);  
  Updates with the player's name, score, and timestamp after each round played.

How It Works:
1. Starting the Game:
   The game begins by prompting the user to enter their name. Once provided, the quiz instructions are displayed.

2. Quiz Mode Selection:
   The user can choose between:
   C for  Current Affairs
   G for  General Knowledge

3. Loading Questions:
   Based on the mode selected, the game loads questions and answers from the appropriate text files.

4. Scoring Mechanism:
Each question allows a maximum of three attempts.
   Correct answers on the first attempt earn full points.
   Retrying the question awards partial points.
   Encouraging messages (both positive and negative) provide real-time feedback as you progress.

5. Post-Quiz Summary:
   At the end of a round, the score is displayed, added to the leaderboard, and a round summary (including average score) is shown.

6. Multiple Rounds:
   You have the option to play additional rounds or view the leaderboard before ending the session.

