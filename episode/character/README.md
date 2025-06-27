# 📚 Character Queries by ID – Rick and Morty GraphQL

This directory contains GraphQL queries used to fetch character details from the Rick and Morty GraphQL API by ID.

## 📌 Queried Fields

Each query requests the following fields:
- `id`
- `name`
- `status`
- `species`
- `type`
- `gender`

## 📂 Files Included

For each character ID (1–4), there are two files:
- `character-id-X.graphql`: the query for that character
- `character-id-X-output.json`: the JSON response returned by the API

## 🔗 GraphQL Endpoint

[https://rickandmortyapi.com/graphql](https://rickandmortyapi.com/graphql)

---

✅ Example query:
```graphql
query {
  character(id: 1) {
    id
    name
    status
    species
    type
    gender
  }
}
🚀 How to Run
Use Postman, Insomnia, or the GraphQL Explorer to test queries.
URL: https://rickandmortyapi.com/graphql
Method: POST
Headers: Content-Type: application/json
Body:
{
  "query": "...your query here..."
}
## 🔢 Get All Characters by Page

This section includes queries to fetch paginated lists of characters using the `characters(page: Int)` field.

Each query retrieves:
- `id`
- `name`
- `status`
- `image`

Pages included: 1 to 4.
---

## 🔢 Get All Characters by Page

These queries use the `characters(page: Int)` field to retrieve lists of characters from the API.

### Fields Queried:
- `id`
- `name`
- `status`
- `image`

### Pages Included:
- Page 1 → `characters-page-1.graphql`, `characters-page-1-output.json`
- Page 2 → `characters-page-2.graphql`, `characters-page-2-output.json`
- Page 3 → `characters-page-3.graphql`, `characters-page-3-output.json`
- Page 4 → `characters-page-4.graphql`, `characters-page-4-output.json`
