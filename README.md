# HappyTeams
Priority Team Picking

This program recieves a few commands from the command line to put together teams from a given file with names and their preferences.

To run:

javac  src/main/java/HappyTeams.java \n
java -cp src/main/java HappyTeams -t 3 -v 2 -n 1 -l 1000 -r 4 -p 6 < choice/testFinal.txt

-t = teamsize (how big each team will be)

-v = verbosity (how much is outputted 0-4)

-n = loops (how many times the names reset to maybe find a better route)

-l = swaps (how many random swaps on the names to find good combinations)

-r = anti-hill climbing (go down -r% of times)

-p = preferences (how many picks each person gets)

< choice/testFinal.txt = the csv styled sheet of names and preferences (see example files in HappyTeams -> choice)

----------------------------------------
Outputs names placed in teams in the command prompt with Total Happiness of the class, team happiness and individual happiness

Happiness is gained by having somone in a persons preference list in that persons team at the end.

Happiness is lost if some loses a person from their team that they want.
(This only happens if a combination that gives higher happiness is found)
