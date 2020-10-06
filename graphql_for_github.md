GQL Query

```
query repository { 
  repository(owner: "USER名", name: "リポジトリ名") { 
    id
    name
    description
    issues(first: 10, states: OPEN){
      totalCount
      nodes{
        title
        body
      }
    }
  }
}
```