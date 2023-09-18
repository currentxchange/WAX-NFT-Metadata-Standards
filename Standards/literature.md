# Literature Media Standard
Use this for any literature-focused NFT schema/category.

# Additional Fields 

| Field | Type | Description |
| :----:  | :----: | :----: |
| series | string | Series the work is part of |  
| pages | number | Number of pages in the work |  
| isbn | string | ISBN identifier for the work |  
| publisher | string | Publisher of the work |  

## Changed Fields
`artist` is called `author`
`nsfw` field is absent

| Field | Type | Description |
| :----:  | :----: | :----: |  
| author | string | Author of the work |  

# 🛠 Literature NFT Standard 
```javascript
[
  {
    "name": "name",
    "type": "string"
  },
  {
    "name": "img", 
    "type": "ipfs"
  },
  {          
    "name": "author", 
    "type": "string"
  },
  {
    "name": "title",
    "type": "string"
  },
  {
    "name": "about",
    "type": "string"
  },
  {
    "name": "series",
    "type": "string"
  },
  {
    "name": "pages",
    "type": "int64"
  },
  {
    "name": "backimg",
    "type": "ipfs"
  },
  {
    "name": "collectionimg",
    "type": "ipfs"
  },
  {
    "name": "genre",
    "type": "string"
  },
  {
    "name": "mood",
    "type": "string"
  },
  {
    "name": "format",
    "type": "string"
  },
  {
    "name": "credits",
    "type": "string"
  },
  {
    "name": "link",
    "type": "string"
  },
  {
    "name": "timestamp",
    "type": "string"
  },
  {
    "name": "date",
    "type": "string"
  },
  {
    "name": "year",
    "type": "string"
  },
    {
    "name": "month",
    "type": "string"
  },
    {
    "name": "day",
    "type": "string"
  },
  {
    "name": "location",
    "type": "string"
  },
  {
    "name": "nation",
    "type": "string"
  },
  {
    "name": "state",
    "type": "string"
  },
  {
    "name": "city",
    "type": "string"
  },
  {
    "name": "geotag",
    "type": "string"
  },
  {
    "name": "isbn",
    "type": "string"
  },
  {
    "name": "publisher",
    "type": "string"
  },
  {
    "name": "license",
    "type": "string"
  },
  {
    "name": "rarity",
    "type": "string"
  }
]
```
