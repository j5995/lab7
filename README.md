Check Your Understanding
Authors: Gautam Mohandas and Eric Wang
Intro:
1) I would fit my automated tests as a Github action that runs whenever code is pushed (1) because the debugging and functionality is implemented through deploying the server locally, which makes testing locally a little repetitive. However, adding a linter and tester after a push would catch on the things that a human didn't pick up on.

Expose:
2) Yes, I would use an end to end test to check if a function is returning the correct output, since the input of the function will be what the user inputs, and an end to end test makes sure that the user input outputs the wanted output.



