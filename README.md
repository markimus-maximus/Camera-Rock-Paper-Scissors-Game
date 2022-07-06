# Camera-Rock-Paper-Scissors-Game

This program is designed to simulate rock paper scissors game.

There are three functions which comprise the functionaility game: get_computer_choice, get_user_choice and get_winner

get_computer_choice uses the random function to generate one of rock, paper or scissors, which comprises the 
computer selection. 

get_user_choice takes input from the webcam in order to determine if the player input is rock scissors or paper. A model
(generated and trained on the website teacheable machine) uses an image from the camera in order to predict what the player choice 
within the game was. A timer function was added before the defining image of the round is taken in order to make the player 
experience easier to follow, as well as providing a singular prediction after the timer is over to define the user choice.   

The get_winner function decides whether the computer random choice (from get_computer_choice function) or the user choice 
(from get_user_choice function) is the winner or a draw, and communicates this with the player.

In order to keep state (score) within a single game, all of the above functions were included as methods within the class.
Rock_paper_scissors. An instance of the class called play_game calls the three methods above iteratively and keeps score. When either 
the player or the computer reaches the attribute instance attribute first_to_x then the game is over and the winner is stated. 

