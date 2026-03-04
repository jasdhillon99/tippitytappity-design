# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
class WordBank{
  string[] words 
  string get_random_word()
}

class Word{
  string text
}

class Score{
  float wpm
  float accuracy
}

WordBank --> Word : contains

class Users{
  string userID
  float highScore
  string[] historyScores

}
Users --> Score : contains
```
