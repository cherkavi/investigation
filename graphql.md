* [tutorial](https://www.howtographql.com/)  
* [guides](https://www.graphql.com/guides/)  
* [specification](https://graphql.github.io/graphql-spec/)  
* [start point](https://graphql.org/)   
* [landscape](https://landscape.graphql.org/)   
* [graphql example app](https://github.com/APIs-guru/graphql-apis)  
* [graphql online editor](https://lucasconstantino.github.io/graphiql-online/)  

# GraphQL vs REST
## http request
![GraphQL vs REST](https://i.postimg.cc/rw5CZRBC/graph-QL-vs-REST.png)
## return data explanation
![data layer](https://i.postimg.cc/PxHxHbJz/graph-QL-explanation.png)
## how it is works
![working process](https://i.postimg.cc/N0gTNJ7B/graph-QL-HIW.png)
## URL Driven vs Query Language
![Query language](https://i.postimg.cc/PqhbgrhG/graph-QL-QL.png)
## Query
### [Online example](https://anilist.co/graphiql)
#### request
```
{
    "query"{
        Page{
            pageInfo {
            total
            perPage
            currentPage
            lastPage
            hasNextPage
            },
            users(id:2, name: "matchai") {
            id,
            name
            }
        }
    }
}
```
#### response
```json
{
  "data": {
    "Page": {
      "pageInfo": {
        "total": 1,
        "perPage": 50,
        "currentPage": 1,
        "lastPage": 1,
        "hasNextPage": false
      },
      "users": [
        {
          "id": 2,
          "name": "matchai"
        }
      ]
    }
  }
}```
### Operations
* query
* mutation
* subscription ( WebSockets )
