# quizButInGerman
Clone of the bsd quiz game but in German only and uses TTS (text to speech).

## STEP 1
Make sure you have BASH. If you're on windows, it's possible to run bash scripts. Here's a link that I haven't tried:

https://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/

## STEP 2
Make sure you have Anna's voice for the TTS (text to speech). These voices should come pre-installed with MacOS (I pressume this will continue to be. As of March 2021 I am using a fully updated MacOS 11.2.1). One way to test this is to issue this command on the CLI: 

```
say -v Anna 'Deutsche'
```

Make sure to turn up your speakers. 

## STEP 3
Put the file named *deutsche* in your ~/bin/ directory. But first, you need to make sure it is executable by issuing this command:

```
chmod u+x deutsche
```

Remember that to issue this last command, you must be in the directory where the *deutsche* file is in.

## STEP 4

Use emacs, vim, sublime, nano or any other editor to edit the *deutsche* shell script:

```
${EDITOR} deutsche
```

look for these variables:

```
FILE_PATH=""
TEMP_PATH=""
TEMP_INCORRECT_PATH=""
```

Write the path to the german-to-english file for FILE_PATH (**do not put the german-to-english file in /tmp because it'll be lost when you reboot your computer**) and write the path to the /tmp/ directories in the last two. If you don't have a temp directory, just pick any directory that you rarely look at. I left the ones I use as an example (which will work on macos and also linux I believe). The error messages you'll get if you didn't read this and ran the program should also help.

## STEP 5
Check out the original quiz game in the BSD games created in the 70s or whereabouts. I don't know who created these games, but a big thank you to the creators (I assume it was CS faculty in UCB in the 70s-80s). 

Here's Mike Sharov's fork:
#https://github.com/msharov/bsd-games
