## Usage

Visit `http://localhost:1111/` to see a GraphiQL interface and query the data.

### Query

```graphql
{
  places {
    id
    name
    description
    email
    phone
    location {
      lat
      long
    }
    images {
      url
      banner
    }
  }
}
```

### Mutation

```graphql
mutation {
  createPlace(name: "Partybus", email: "party@example.com") {
    id
    name
    email
    phone
  }
}
```
