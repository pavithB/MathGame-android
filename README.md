<h1 align="center">  SolveMath </h1>
<br/>
<br/>

<h3 align="center">
The application will be a basic brain training game, which will be asking the user to calculate the answer to various simple arithmetic expressions. [mobile game (#android) is about solving math problemst, Players able to choose difficulty level. </h3>

<p align="center">
1. When the application starts, it presents the user 4 buttons labelled New Game, Continue, About and Exit.
</p>

<p align="center">
  <img src="https://cloud.githubusercontent.com/assets/23357240/26764064/2c6a5afa-497d-11e7-8748-2703bd73df82.png" width="350"/>
</p>
<p align="center">
2. Clicking on the About button, it should present the user with a popup window which describes the rules of the game 
  (it is left up to you to determine the appropriate text of the rules displayed, by looking at the subquestions below). 
  </p>
  
  <p align="center">
  <img src="https://cloud.githubusercontent.com/assets/23357240/26764073/4bae0768-497d-11e7-8996-76b95172e65d.png" width="350"/>
</p>
  <p align="center">
3. Clicking on the Exit button should terminate the application. 
</p>
<p align="center">
4. Clicking on the Continue button, a previously started game is resumed. The game resumes from exactly the same point that it was 
  left before, i.e. the implementation needs to restore the exact previous state of the game. For this, in order to work, the user should
  be asked whether he would like to save the current game when he clicks on the Exit button. Next time the application starts and the user 
  clicks on the Continue button, the state of the last game saved should be restored. 
  </p>
  <p align="center">
5. Clicking on the New Game button, starts a new game for the user. The user is presented with 
  four levels of game diﬃculty, Novice, Easy, Medium, Guru. Clicking on each one of them sets the maximum number of terms 
  involved in the arithmetic expression that the user needs to calculate (see the next subquestion). The Novice level corresponds
  to an arithmetic expression involving exactly 2 integers. The Easy level corresponds to an arithmetic expression with maximum 
  3 terms, i.e. it can contain 2 or 3 integers. The Medium level corresponds to an arithmetic expression with 
  maximum 4 terms, i.e. it can contain 2, 3, or 4 integers. The Guru level corresponds to an arithmetic expression with maximum 
  6 terms and minimum 4 terms, i.e. it can contain 4, 5 or 6 integers. 
  </p>
  
  <p align="center">
  <img src="https://cloud.githubusercontent.com/assets/23357240/26764078/603ffc04-497d-11e7-9d75-4353f758d7ef.png" width="350"/>
</p>
<p align="center">
6. After the user sets the diﬃculty level, by clicking on one of the 4 levels, the user is presented with the main game screen
  which contains a random (not ﬁxed or hardcoded but randomly generated by the program itself) arithmetic expression among 
  integers, based on the diﬃculty level he/she has chosen. The arithmetic expression includes random mixed operations utilising 
  addition, subtraction, multiplication and division. Following the above description, if the user has chosen previously a Medium 
  level of diﬃculty, he/she will be presented with a single random arithmetic expression which includes 2, 3, or 4 integers. Examples 
  of such expressions are 55∗2−4−101, 102/3/3, 589−281, 123 + 5∗6 + 2. Besides the arithmetic expression, the game screen also contains 
  13 buttons corresponding to numbers 0 to 9, the DEL key, the # key and the minus − key. The screen should be looking exactly like 
  Figure 1, although spacing, fonts, colours and sizes of boxes and buttons can be diﬀerent. Once the user starts typing the correct 
  answer by using the game screen buttons, the question mark ? will disappear and replaced with the numbers that the user types.
  E.g. if the user enters number 1 followed by 3, etc. then the numbers 1, 3, etc. should replace the question mark in the Figure. 
  A digit appears on the screen as soon as the user types each single digit, by using the on screen buttons, i.e. the answer appears 
  digit by digit and NOT just when the user types the whole answer. If the user presses DEL and deletes all digits typed, the ?
  does not appear again. The user indicates that the full answer is completed by hitting the # button. If the user makes a mistake 
  he/she can delete the last digit typed by pressing the DEL button. The arithmetic expression should be evaluated from left to right
  and all operations assume the same precedence. No parentheses or other brackets should be presented to the user to determine the 
  precedence. Every arithmetic expression (including subexpressions within the whole expression) should be evaluated in such a way, 
  that if the result is a non-integer, the result should be rounded to the closest integer number. For example, the expression 10/3*2 
  should evaluate to 6, because 10/3 is 3.333 which is rounded to 3, then multiplied by 2, giving the overall result of 6. In total, 
  for a single game, the user will be presented and asked to guess 10 diﬀerent arithmetic expressions. Note that this subquestion, 
  requires the user to use the game screen buttons to give the answer and NOT the Android device soft or hard keyboard! 
  </p>
  
  <p align="center">
  <img src="https://cloud.githubusercontent.com/assets/23357240/26764089/af975bee-497d-11e7-847a-c226b5bf5aab.png" width="350"/>
</p>
 <p align="center">
7. As soon as the user enters the # sign following the answer, the message CORRECT! (in green colour) or the message WRONG! 
  (in red colour) appears on the screen, depending on whether the answer given is correct or incorrect respectively, as shown 
  in Figure 2. Pressing the # button again, presents the user with the next arithmetic expression, until the user completes the 
  full cycle of guessing 10 arithmetic expressions. 
  </p>
    <br/>
  <p >
  <img align="left" src="https://cloud.githubusercontent.com/assets/23357240/26764094/c295607e-497d-11e7-8c13-1e736244c18c.png" width="350"/> <img align="right" src="https://cloud.githubusercontent.com/assets/23357240/26764096/c9b0a2c4-497d-11e7-9db6-1a230d6ec4a2.png" width="350"/>
</p>
  <br/>
 <p align="center">
8. Extend the implementation so that the user can switch on hints from a preference menu. If the hints option is “on” then 
  he/she will be given 4 attempts per question (arithmetic expression), in case his ﬁrst, second and third attempts to answer 
  are incorrect. Every time that the user gives an incorrect answer when this option is “on” the application will
  be displaying “greater” (if the user’s answer is less than the correct answer) and “less” (if the user’s answer is greater than
  the correct answer). 
  </p>
  <br/>
  <p >
  <img align="left" src="https://cloud.githubusercontent.com/assets/23357240/26764100/ebdc9f56-497d-11e7-9419-320adbfa51c7.png" width="350"/> <img align="right" src="https://cloud.githubusercontent.com/assets/23357240/26764101/eeece55c-497d-11e7-851f-d995e7b4f414.png" width="350"/>
</p>
  <br/>
  <p align="center">
9. Extend the application by providing a countdown timer, counting from 10 down to 1, every tick occurring after 1 second exactly.
  The countdown timer is displayed in the main screen of the game, as shown in Figure 3. As soon as the counter reaches the value of 0,
  the next arithmetic expression is presented to the user (in this case the user does not need to press the # to move to the next question). 
  However, if the user presses the # button before the counter reaches 0, the counter stops, the game displays whether the answer is
  correct or incorrect and a subsequent press of # moves to the next question. In the case that hints are “on”, a press of the # button
  before the counter reaches 0 does not stop the counter if the answer is incorrect. The counter keeps running until it
  reaches 0, or until the maximum attempts per question is reached (4) or until the user gives the correct answer to the question. 
  </p>
 <p align="center">
10. In the end of each game (after 10 arithmetic expressions), the user will be displayed with a score which the sum of the points scored in each question. The score will take into account how fast the user answered the question. It will be calculated based on the following:
  (a) 0 marks for each incorrect guess (b) 100 10−time remaining marks for each correct guess. time remaining is the value 
  of the countdown timer when the user pressed the # button to submit the answer. For example, if the user answered a question 
  correctly and the time remaining was 4 secs, then the points received for the question are 100/(10-4) = 100/6=17 points.
  Points are rounded to the closest integer value We assume that the user usually cannot answer in less than 0 secs in order 
  to avoid a denominator of 0. If the user answers a question with 10 secs remaining, then the points awarded are 100
  (for a correct guess), i.e. we don’t use the above formula.
  </p>
  <p align="center">
  <img src="https://cloud.githubusercontent.com/assets/23357240/26764105/074ca5ba-497e-11e7-8835-224879a8786c.png" width="350"/>
</p>

  
