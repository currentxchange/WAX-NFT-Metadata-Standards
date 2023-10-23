# Literature Media Standard
Use this for any literature-focused NFT schema/category, like a short story, poem, article, or a book you want to publush as a NFT.

> 📺 [Watch the Youtube Tutorial](https://www.youtube.com/watch?v=eSlmOtpiNaM)

# Additional Fields 

| Field | Type | Description |
| :----:  | :----: | :----: |
| series | string | Series the work is part of. |  
| pages | int64 | Number of pages in the work. |  
| isbn | string | ISBN identifier for the work.  |  
| publisher | string | Publisher of the work. |  

## Changed Fields
`artist` is called `author`
`nsfw` field is absent 

| Field | Type | Description |
| :----:  | :----: | :----: |  
| author | string | The primary author(s) of the work or their pen name. |


# 🛠 Literature NFT Standard 

# Light Version 🌞

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
    "name": "promo", 
    "type": "ipfs"
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
    "name": "labels",
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

# Spacetime Version 🛸
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
    "name": "promo", 
    "type": "ipfs"
  },
  {
    "name": "timestamp",
    "type": "int64"
  },
  {
    "name": "date",
    "type": "string"
  },
  {
    "name": "year",
    "type": "int64"
  },
    {
    "name": "month",
    "type": "string"
  },
    {
    "name": "day",
    "type": "int64"
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
    "name": "labels",
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
