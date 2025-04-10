# Sitecore Content Hub GraphQL Queries

This repository contains example GraphQL queries for retrieving content and assets from **Sitecore Content Hub** using its headless delivery endpoints.

These queries can be used with both the **Preview API** and **Delivery API** (depending on your use case) via the GraphQL IDE or programmatic HTTP requests.

## 🔧 Setup

To test or run these queries:

1. Access the GraphQL IDE:
   - **Preview:** `https://yourinstance-url/api/graphql/preview/ide`
   - **Delivery:** `https://edge.sitecorecloud.io/api/graphql/ide`

2. Add your API key to the HTTP headers:
```json
{
  "X-GQL-Token": "your-api-key"
}
