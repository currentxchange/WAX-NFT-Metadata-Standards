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
| raw | ipfs | Unedited max resolution of image. | 
| resolution | string | Width x Height of the photo in pixels e.g. 3840 x 2160 |
| ratio | string | Aspect ratio of the photo, e.g. 16:9 |

## Changed Fields
`artist` is called `photographer`


| Field | Type | Description |
| :----:  | :----: | :----: |  
| photographer | string | Photographer of the work |



# 🛠 Photo NFT Standard 
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
    "name": "nsfw",
    "type": "bool"
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
