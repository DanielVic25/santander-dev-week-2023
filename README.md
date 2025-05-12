# Santander Dev Week 2023
java RESTful API Criada para Santander Dev Week. 

## Diagrama de Classes 

```mermaid
classDiagram
  class User {
    -String name
  }

  class Account {
    -String Number
    -String Agency
    -Float Balance
    -Float Limit
  }

  class Feature {
    -String icon
    -String description
  }

  class Card {
    -String Number
    -Float Limit
  }

  class News {
    -String icon
    -String description
  }

  User "1" *-- "1" Account
  User "1" *-- "n" Card
  User "1" *-- "1" Feature
  User "1" *-- "n" News

```
