# Photo Media Standard
Use this for any photography-focused NFT schema/category. 

# Additional Fields 

| Field | Type | Description |
| :----:  | :----: | :----: |
| camera | string | The camera model used | 
| lens | string | The lens model used | 
| exposure | string | The exposure settings, e.g. "1/125 sec at f/5.6" |
| focal | number | The focal length of the lens in mm | 
| iso | number | The ISO setting used | 
| fullsize | ipfs | Unedited RAW file with max resolution image. If not shooting in RAW, provide largest image in uncompressed format | 
| resolution | string | Width x Height of the photo in pixels e.g. 3840 x 2160 or 4k |
| ratio | string | Aspect ratio of the photo, e.g. 16:9 |

## Changed Fields
`artist` is called `photographer`


| Field | Type | Description |
| :----:  | :----: | :----: |  
| photographer | string | Photographer of the work. Use `credits` field for human models, etc., and the photo standard for AI models |



# 🛠 Photo NFT Standard 

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
    "name": "photographer", 
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
    "name": "camera",
    "type": "string"
  },
  {
    "name": "lens",
    "type": "string"
  },
  {
    "name": "exposure",
    "type": "string"
  },
  {
    "name": "focal",
    "type": "int64"
  },
  {
    "name": "iso",
    "type": "int64"
  },
  {
    "name": "fullsize",
    "type": "ipfs"
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
    "name": "photographer", 
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
    "name": "camera",
    "type": "string"
  },
  {
    "name": "lens",
    "type": "string"
  },
  {
    "name": "exposure",
    "type": "string"
  },
  {
    "name": "focal",
    "type": "int64"
  },
  {
    "name": "iso",
    "type": "int64"
  },
  {
    "name": "raw",
    "type": "ipfs"
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
