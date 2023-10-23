# Video Media Standard
Use this for any video NFT schema/category. This can be for a movie or a youtube video. 

> 📺 [Watch the Youtube Tutorial](https://www.youtube.com/watch?v=0EKb60iGtWE)

# Additional Fields 

| Field | Type | Description | 
| :----:  | :----: | :----: | 
| video | ipfs | Video file via IPFS hash | 
| youtube | string | Youtube link | 
| filetype | string | Video format e.g. MP4, MOV | 
| duration | string | Video lengths as "days : hour : minutes : seconds" "2:47" = two minutes 47 seconds | 
| resolution | string | Width x Height of the photo in pixels e.g. 3840 x 2160 or 4k | 
| fps | int64 | Frames per second of the video | 
| ratio | string | Aspect ratio of the photo, e.g. 16:9 | 

## Changed Fields
`artist` is called `creator`

> Note: In this standard, many marketplaces will always show the img attribute. For this reason, you can choose to include a video in the image field through IPFS, or leave the image field blank, and fill out the video field instead. Both of these options will work on most marketplaces, but some, notably Atomichub, may not allow you to upload a video file to their free image hosting service on IPFS, or may restrict the image file size.

| Field | Type | Description |
| :----:  | :----: | :----: |  
| creator | string | Director or channel-owner of the work. Remember to use the `credits` field for multiple |  



# 🛠 Video NFT Standard 

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
    "name": "video", 
    "type": "ipfs"
  },
  {          
    "name": "youtube", 
    "type": "string"
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
    "name": "filetype",
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
    "name": "promo", 
    "type": "ipfs"
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
    "name": "video", 
    "type": "ipfs"
  },
  {          
    "name": "youtube", 
    "type": "string"
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
    "name": "filetype",
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