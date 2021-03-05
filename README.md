# quizButInGerman
This script is a clone of the bsd quiz game but specifically for German words. It also uses TTS (text to speech) so that users can hear how to pronounce the words.

#Installation

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
Put the file named *deutsche* in your ~/bin/ directory. But first, you need to make sure it is executable by issuing the following command:

```
chmod u+x deutsche
```

Remember that to use this last command, you must be in the directory where the *deutsche* file is in.

## STEP 4

Edit some variables in the *deutsche* shell script:

```
${EDITOR} deutsche
```

look for these variables:

```
FILE_PATH=""
TEMP_PATH=""
TEMP_INCORRECT_PATH=""
```

For **FILE_PATH** write the path to where you'll be storing your german-to-english file (**do not put the german-to-english file in /tmp because it'll be lost when you reboot your computer**). Then for **TEMP_PATH** write something like: */tmp/d.temp*. Choose a similar name for **TEMP_INCORRECT_PATH** I'm leaving the paths I used as an example if you're not feeling creative.

## STEP 5
Be sure to check out the original quiz game and the other BSD games created in the 70s. I don't know who created these games, but a big thank you to the creators (I assume it was CS faculty at UCB in the 70s-80s). 

Here's a link to Mike Sharov's fork:
#https://github.com/msharov/bsd-games
