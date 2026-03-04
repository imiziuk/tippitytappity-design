# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
  Controlller <|-- UI
  class UserData{
        + speed: float
        + wpm: float
        + accuracy: float
        + time : TIME
  }
  class UI{
    - current_phrase: integer
    + render_phrase
    + validate_input
  }
  class Controlller{
    - phrases: List~string~
    - current_phrase: integer 
  }
  class History{
     + add_history(user, time, acuracy, speed)
     + get history(user, time) : accuracy, speed
     + get all_history(user) : list<history(user over time)
  }
```
