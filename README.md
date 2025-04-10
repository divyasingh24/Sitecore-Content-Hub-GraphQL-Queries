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
```

## 📁 Query List

| File                          | Description                                                        |
|-------------------------------|--------------------------------------------------------------------|
| `getAllBlogs.graphql`         | Retrieves blog title, quote, and body                              |
| `getAllBlogsWithImage.graphql`| Retrieves blog title, quote, and linked image asset info           |
| `getJPGAssets.graphql`        | Retrieves assets where filename contains `.jpg`                    |
| `gettestassets.graphql`       | Retrieves assets with filenames containing the word `test`         |
| `getRecentAssets.graphql`     | Retrieves assets created on a specific date                        |
| `filterByTypeAndDate.graphql` | Combines filters to get `.jpg` assets created on a specific date   |


## 🧠 Content Model Assumptions
These queries are built based on the following assumptions in Sitecore Content Hub:

There exists a content type named Blog with fields like blog_Title, blog_Quote, blog_Body, and possibly blog_Image.

Assets follow naming and metadata conventions such as including file types in filenames and using creation timestamps.


> 📌 Feel free to fork this repo, contribute additional query examples, or adapt them to fit your own content models.
