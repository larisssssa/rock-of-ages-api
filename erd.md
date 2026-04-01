```mermaid

erDiagram

User {
  id int pk
  first_name varchar
  last_name varchar
  email varchar
  username varchar
}
User ||--o{ Rock : collects
Rock {
  id int pk
  name varchar
  weight decimal
  type int
  user int
}
Rock ||--|{ Type : contains
Type {
  id int pk
  label varchar
}


```
