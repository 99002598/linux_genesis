#Running the code in Linux Terminal

Running the code:
make

Then to obtain the output:
./final

Then input one number:n
2*n players will be totally picked
n referees

1) I have assumed that if a player has a probability > 0.5 of being picked then I pick a player else a referee.
2) I have also assumed that the number of courts are infinity since it is not mentioned in the question.
3) I have changed it from 0.5 sleep time to 1 because I had difficulty in compiling it.

Use of mutexes

I have 3 mutexes. One for the count of the referees yet to meet the organiser. One for the count of the players yet to meet the organiser.
One for the organiser himself.
The players and referees enter. Until a group is formed, the organiser is not bothered. Once a group is formed we check if the
organiser is free or not (determined by the organiser mutex).We wait till the organiser is free. Once the organiser is free the group takes that
organiser(locks the organiser mutex) and enters the court. The players warmUp (player thread is now created) and referee adjusts the equipment.
Once this is done (find out using thread_join) you leave the organiser (unlock mutex) and start the game.




[![Codacy Badge](https://api.codacy.com/project/badge/Grade/32334a753d26480eba6bff7cc9960e6a)](https://app.codacy.com/manual/99002598/linux_genesis?utm_source=github.com&utm_medium=referral&utm_content=99002598/linux_genesis&utm_campaign=Badge_Grade_Settings)

![cppcheck-action](https://github.com/99002598/linux_genesis/workflows/cppcheck-action/badge.svg)
![C/C++ CI](https://github.com/99002598/linux_genesis/workflows/C/C++%20CI/badge.svg)
![Unit testing](https://github.com/99002598/linux_genesis/workflows/Unit%20testing/badge.svg)

![Unit testing](https://github.com/99002598/linux_genesis/workflows/Unit%20testing/badge.svg)



