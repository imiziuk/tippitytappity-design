# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
  Controlller <|-- UI
  class UserData{
        + speed: float
        + wpm: float
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
```
