### 外部制約

```shell
rails g model memo title:string
rails g model details memotitle:string detail:string memo:references
rake db:migrate
```
