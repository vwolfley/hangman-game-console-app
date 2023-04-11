# Hangman Game Console App in C#

A simple command line application or console app hangman game, written in C#

## What is Hangman

Hangman is a classic word game in which you must guess the secret word one letter at a time.  At the start of a game, you are presented with an set of blank lines representing the missing letters of the word.  Each correct guess of a letter fills in the blanks.  Each incorrect guess of a letter, another part of the hangman's gallows is drawn.  The aim of the game is to find the hidden word before the hangman's gallows is fully drawn.  The word to guess is chosen from the list of over 1,300 commonly used English vocabulary or from topical word lists like - sports, seasons, and colors.

* Guess one letter at a time to reveal the secret word.
* Each incorrect guess adds another part to the hangman gallows. 
* You only get 7 incorrect guesses.

- [Hangman Game](https://en.wikipedia.org/wiki/Hangman_(game))

## Helpful Utilities

To work with this you may need the following:

- [Visual Studio Code](https://code.visualstudio.com/) installed on your development machine. If you do not have Visual Studio Code, visit the previous link for download options. (**Note:** This tutorial was written with Visual Studio Code version 1.52.1. The steps in this guide may work with other versions, but that has not been tested.)
- [.Net Core SDK](https://dotnet.microsoft.com/en-us/download/dotnet/7.0)
- [C# extension for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.csharp)


# Configuring launch.json for C# debugging
The launch.json file is used to configure the debugger in Visual Studio Code.

Visual Studio Code generates a launch.json with almost all of the required information. 
If your workspace has only one launchable project, the C# extension will offer to automatically generate this file. 
If you missed this prompt, you can force the generation by executing the command `.NET: Generate Assets for Build and Debug` from the VS Code command palette.
The generated file contains two sections. One that configures debugging for launch and a second that configures debugging for attach.

If you have more than one launchable project, then you will need to modify your launch.json file by hand. 
Visual Studio Code will still generate a basic template, but you will need to fill in the 'program' field to point at the executable dll that you would like to debug.

## Console (terminal) window
`"integratedTerminal"` : the target process will run inside [VS Code's integrated terminal](https://code.visualstudio.com/docs/editor/integrated-terminal). Click the 'Terminal' tab in the tab group beneath the editor to interact with your application.
