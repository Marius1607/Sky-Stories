# Sky-Stories
The classes  Big Dipper, Cassiopeia, Orion, Taurus, Scorpio, Polaris, UndyingStars and Sirius are only used for display purposes. Every class has an activity of its own containing TextAreas and images.
The class Constellations has the method enterConstellation which is used to acces one of the constellations. 
The class Curiosities has the method enterCuriosities which is used to acces one of the curiosities.
The functions switchToChapterPage, switchToCuriositiesPage and switchToQuizPage from the Menu Class are only used to switch to another Intent.
The class Question has no activity. It is used as a blueprint for the objects of type Question. It has 2 constructors, one empty and one with arguments and basic getters.
The class Questions has no activity also. It represents an array of object of type Question. It has 2 constructors, one empty and one with arguments and one function called checkAnswer. The function verify if the id of the button pressed by user is the correct answer.
The class Quiz has the activity called activity_quiz. It is used to display the questions, answers and to validate them. 
It has the following functions:
- populateQuestions, which takes as argument an object of type questions and populate it with Question object.
- createQuizz, which is responsible for displaying the question and the text on buttons, and also switching them.
- sendAnswer, which is responsible for checking all answers, using the checkAnswer function, and tells to createQuizz to bring up other question. If there are no more questions, it will send the user to QuizScore.
- nextQuestion switches the question for the user. It is called by the function sendAnswer.
- isANextQuestion verifies if there is a next question. If there is, the function nextQuestion is called. Otherwise, the player is send in QuizPoints.

QuizPoints is a class that has the activity quiz_points and it is used only for displaying the score after a quiz is done. 
It has a method called switchToMenuPage that is reseting the points from Quiz to 0, in case the user wants to take the Quiz again and then send the User back to the Menu.
