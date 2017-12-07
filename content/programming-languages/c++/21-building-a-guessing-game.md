---
date: 2017-11-07T01:21:26-05:00
title: "Building A Guessing Game"
seo_title: "Building A Guessing Game | C++ | Giraffe Academy"
subheader:
     greeting: C++ - Programming Language
     description: This course covers the basics of programming in C++. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers building a guessing game in C++.
author: Mike Dane
image: building-a-guessing-game.png
video: xJ4jhhOtyAk
url: /programming-languages/c++/building-a-guessing-game/
weight: 21
---

## Code

{{< code lang="cpp" >}}
int secretNum = 7;
int guess;
int guessCount = 0;
int guessLimit = 3;
bool outOfGuesses = false;

while(guess != secretNum && !outOfGuesses){
     if(guessCount < guessLimit){
          cout << "Enter a guess: ";
          cin << guess;
          guessCount++;
     } else {
          outOfGuesses = true;
     }
}

if(outOfGuesses){
     cout << "You Lose!" << endl;
} else {
     cout << "You Win!" << endl;
}
{{< /code >}}