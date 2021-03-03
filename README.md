# quizButInGerman
Clone of the bsd quiz game but in German only and uses TTS

## STEP 1
Make sure you have BASH. If you're on windows, it's possible to run bash scripts. Here's a link that I haven't tried:

https://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/

## STEP 2
Make sure you have Anna's voice for the TTS (text to speech). These come pre-installed with MacOS (I pressume this will continue to be. I am using Big Sur as of today). One way to test this is to issue this command on the CLI: 

```
say -v Anna 'Deutsche'
```

Make sure to turn up your speakers. 

## STEP 3
Put the file named deutsche in your ~/bin/ directory. But first, you need to make sure it is executable by issuing this command:

```
chmod u+x deutsche
```

in the directory where this file is in.

## STEP 4

Use emacs or sublime or nano or any other editor. To edit the shell script.

```
vim deutsche
```

look for these variables:

```
FILE_PATH=""
TEMP_PATH=""
TEMP_INCORRECT_PATH=""
```

Write the path to the german-to-english file for FILE_PATH and write the path to the /tmp/ directories in the last two. If you don't have a temp directory, just pick any directory that you rarely look at. I left the ones I use as an example (which will work on macos and also linux I believe). The error messages you'll get if you didn't read this and ran the program should also help because you I bet your username is not yourusername or fernandozegada (depends on whether I remembered to change that).

## STEP 5
Check out the original quiz in the BSD games created around the 70s. I don't know by who but I like them whoever they are.
