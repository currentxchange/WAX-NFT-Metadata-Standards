# Image Media Standard
Use this for any image-focused NFT schema/category that isn't a photograph. 

# Additional Fields 

| Field | Type | Description |
| :----:  | :----: | :----: |
| filetype | string | The filetype of the image | 
| fullsize | ipfs | Unedited max-resolution image, useful if you want a loadable preview, and the real deal | 
| resolution | string | Width x Height of the largest-version image in pixels e.g. 3840 x 2160 or 4k |
| ratio | string | Aspect ratio of the image, e.g. 16:9 |
| generative | bool | Was AI used to make this image? Give credit to the model/app in the `credits` field |


## Changed Fields
None of the default fields are changed. 


# 🛠 Image NFT Standard 

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
    "name": "artist", 
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
    "name": "filetype",
    "type": "string"
  },
  {
    "name": "resolution",
    "type": "string"
  },
  {
    "name": "ratio",
    "type": "string"
  },
  {
    "name": "generative",
    "type": "bool"
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
    "name": "nsfw",
    "type": "bool"
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
    "name": "artist", 
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
    "name": "filetype",
    "type": "string"
  },
  {
    "name": "resolution",
    "type": "string"
  },
  {
    "name": "ratio",
    "type": "string"
  },
  {
    "name": "generative",
    "type": "bool"
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
    "name": "nsfw",
    "type": "bool"
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
