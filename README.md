# PGN-Book-Creator
Tool for creating chess opening book from PGN databases in a different way

Wellcome to everyone, my name is "Rubenkku" here on Github, and i have other nicks like "psycotrance" in chessbase engine room, where i play from 2008 when i discovered computer chess software Rybka 3 GUI.

This is a software i made in three days (version 0.1) created with python3 and with the help of ChatGPT AI chat.

This software reads a .PGN chess games database opensource format and creates a opening tree that you can navigate on the GUI.
This opening tree stores information for each move played on the PGN games, this information is:

- move        (the chess move 1. indicates white side, and ... indicates black side)
- frequency   (how many times this move appeared on the PGN)
- weight      (and average value, when tha game is won by white its value is 100, when is draw is 50, and when is won by black is 0)
- avg eval    (an average value of all the engine evaluations for that move)
- Last player (it just show the name of the player that did the move, in the last game where this move appeared on the PGN)
- Last Seen   (the date of the most recent game where this move appeared on the PGN)

To start using the program, you can load a PGN of your choice to create the opening book.
Consider that the bigger the database, the more time it needs to read all the games
- Below 10000 games is fast
- From 10000 to 50000 games it may take some minutes
- From 50k to 100k it may take 5 to 10 min
- From 100k to 500k it may take 15 min or more
It depends on your hardware aswell, and on your RAM memory available, start with small databases, and if you need to manage large databases, make sure you have time available.

Click on Browse to select a PGN from your computer, it will start to read it, GUI may froze or say (not responding), just give it time.

After this you will get a opening tree where you can navigate with mouseclick or using keyboard arrows, up, down, left, right

When you navigate through the tree, a notation appears, you can click on any of the notation movements to go back to that position.
Navigate back and forth with left and right arrows or by mouseclicks on the moves you want
use up and down arrows to choose different moves on that turn.

The board it's only for show the position, its not clickable (by now)

If you are studying a particular game, you can copy a PGN game, and pase over the program with the button "paste PGN" or by doing ctrl+v
By doing that, the game is added to the tree, and then is opened to the end. You can navigate back in the game, or click any of that game moves on the notation.

The name of the ECO opening and its variations appear on the bottom of the notation automatically when navigating through the games.

Other buttons are:
- left and right arrows   (same as arrown on the keyboard)
- Flip                    (turns the board to see it from the one side or another)
- Save book               (it saves the actual opening tree to a file, so you can open that particular tree without loading all the PGN again. It loads faster)
- Load book               (loads a saved opening tree, replacing the actual one)

A new book format is created, a file .book, this format is not usable by any engine or other chess softwares.
It stores new kind of information about the moves, it may store any other useful new info as the software is open to suggestions.
A new book format containing new information that may be useful or used by new engines, as code may be created to read the info stored for the moves.

This is the base software for creating more advanced functions and ideas for book creation, as we process diferent variables here, we can edit the PGN with new criteria, manipulating the PGN games to create different kind of books, like agressive books (store games only with evals > 0.35), or superdraw book (take only games where 0.00 is reached as soon as possible) and cut the game from the 0.00 position to save space. Or trimm games that X player (me or other) did played from X time ago. Or trim book branches that X player is not using that move anymore (because other more recent is now used)
Other idea maybe filter out games according to certain piece conditions, for example, show me all games where all the 8 pawns still stay at turn 50 (very closed positions) etc.
And all kind of ideas that community may apport.
This tool opens the workaround for almost any idea on how to select tha games for our books, based on certain criteria

By now, with the version 0.1, its a curious tool where you can see the author of the moves you study, and the new feature average eval, to compare moves in a different way.
I use it with my working books to see what players are attacking me on certain openings, its worth to take a look at the game you are studying with this tool.
All the potential of this tool is still to come.

The version 0.1 is a presentation for all, my friends and my enemies, i think everyone deserves this, as computerchess is what it need, something new, new users, new people, new software to enjoy the chess.
The upcoming updates will require a lot of hours of programming, trial and error, frustation, joy, etc
Version 0.1 required 3 days, and like 15 hours of job. Im giving it free
Upcoming versions will start to be closed, only for friends and people that really deserves my time and my job. People that participates in the test, find bugs, apport ideas or i see that show great interest will be wellcome. People only asking all day for updates without even say thanks, maybe ignored.
Its also possible at any given moment that i ask for a donation as a recognition for my job. I wont do it for the money, i would do it the see who deserve my job and who probably dont.

Said that, i hope you like and enjoy the software, and give it your feedback, and moreover a voluntary donation, as it would boost my moral and my will to do this project a powerful new tool.

Regards to all and thanks for your interest.
Rubenkku.
