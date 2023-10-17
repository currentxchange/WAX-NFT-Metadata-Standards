# Music Media Standard
Use this for any image-focused NFT schema/category that isn't a photograph. 

> Note: We have published another [Music NFT standard](https://github.com/currentxchange/Music-NFT-Standard) previous to the media standards. This version is fully compatible with the larger set of media standards published here. To ensure maximum compatibility, we suggest that you use this standard instead of the old standard, but they both work. Please note that there are a few changes in the standard, such as the absence of a promo image field in this version. 

# Additional Fields 

| Field | Type | Description |
| :----:  | :----: | :----: |
| audio | ipfs | The audio file, mp3 recommended for size | 
| video | ipfs | Music video file | 
| clip | ipfs | Intended to be a short video or 30 second preview common on streaming platforms | 
| youtube | string | Youtube link | 
| spotify | string | Spotify link | 
| soundcloud | string | Soundcloud link | 

> Platform Compatibility: The YouTube field is supported by Atomichub's marketplace, and will be embedded so people can easily watch it. The standard also includes fields for Spotify and SoundCloud, Which is not yet supported by any major marketplace, but may be in the future. If you would rather include other platforms, you can use the `link` field, or as a custom field by changing the name of one of these fields before you incorporate it into your schema. 

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
    "name": "audio", 
    "type": "ipfs"
  },
  {
    "name": "video", 
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
    "name": "clip", 
    "type": "ipfs"
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
    "name": "youtube",
    "type": "string"
  },
  {
    "name": "spotify",
    "type": "string"
  },
  {
    "name": "soundcloud",
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
    "name": "audio", 
    "type": "ipfs"
  },
  {
    "name": "video", 
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
    "name": "clip", 
    "type": "ipfs"
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
    "name": "youtube",
    "type": "string"
  },
  {
    "name": "spotify",
    "type": "string"
  },
  {
    "name": "soundcloud",
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
