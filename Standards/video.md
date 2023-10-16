# Video Media Standard
Use this for any video NFT schema/category. This can be for a movie or a youtube video. 

# Additional Fields 

| Field | Type | Description | 
| :----:  | :----: | :----: | 
| video | ipfs | Video file via IPFS hash | 
| filetype | string | Video format e.g. MP4, MOV | 
| duration | string | Video lengths as "days : hour : minutes : seconds" "2:47" = two minutes 47 seconds | 
| resolution | string | Width x Height of the photo in pixels e.g. 3840 x 2160 | 
| fps | number | Frames per second of the video | 
| ratio | string | Aspect ratio of the photo, e.g. 16:9 | 

## Changed Fields
`artist` is called `creator`

Note: In this standard, many marketplaces will always show the img attribute. For this reason

| Field | Type | Description |
| :----:  | :----: | :----: |  
| creator | string | Director or channel-owner of the work |  



# 🛠 Video NFT Standard 
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
    "name": "video", 
    "type": "ipfs"
  },
  {          
    "name": "creator", 
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
    "name": "format",
    "type": "string"
  },
  {
    "name": "duration",
    "type": "string"
  },
  {
    "name": "resolution",
    "type": "string"
  },
  {
    "name": "fps",
    "type": "int64"
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