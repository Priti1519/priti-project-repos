# priti-project-repos

all: README.md

README.md: guessgame.sh
	echo "##Unix course assignment" > README.md
	echo "*by Priti Na on(https://www.coursera.org/).*" >> README.md
	echo "\n**Description**: You need to make a program called *guessgame.sh*.This program will ask the user continously  to guess the number of files present in the current directory,until the number is correct. The user will be informed if their guess is too high if the number they guessed is larger than the number of files or too low if the number they guessed is smaller than the number of files.Once the user guesses the correct number of files in the current directory they should be congratulated." >> README.md
	echo -n "\n**Make date**: " >> README.md
	date >> README.md
	echo -n "\n**Number of lines in guessgame.sh:** " >> README.md
	grep -c '' guessgame.sh >> README.md

clean:
	rm README.md
