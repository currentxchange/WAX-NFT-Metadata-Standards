# WAX NFT Metadata Standards

```Javascript
// -- Stats -- \\
Version: 0.1.0
Supported Types: 
by: [cXc](https://cxc.world)
```

The WAX NFT metadata standards are a collection of fields to use when creating your schema on Atomic Assets. We provide copy-paste, plug-and-play schemas that work with the most popular markets on both US and WAX, starting with [Atomichub](https://wax.atomichub.io/), [NFThive](https://nfthive.com/), [WAXdao](https://waxdao.com/) and more. 


# Learn how to use these in the [Instructional Video](https://www.youtube.com/watch?v=GXjBQnV_Xm8) made for our similar [Music NFT standard](https://github.com/currentxchange/Music-NFT-Standard). 

# The Standards

Are in the [./Standards](./Standards) directory.

Here's how they work

Here are the basic fields. Each type of media has a slightly different list of fields. 

`string` just means text, `ipfs` is an [ipfs hash](https://www.pinata.cloud/) of the data.

| Field | Type | Description | 
| :----:  | :----: | :---- |
| name | string | NFT name |  
| img | ipfs | Primary image, because this is an IPFS field, you can use a video here as well, under 7mb weight recommended |  
| artist | string | The artist, if you prefer a separate field to putting with other credits | 
| title | string | The title of the work | 
| about | string | Description field with main info about the work |  
| backimg | ipfs | Back cover of art, or used as supplementary artwork |  
| collectionimg | ipfs | Extra image for Collection, optional |  
|<hr>|<hr>|<hr>|
| genre | string | Genre of the work |  
| mood | string | Mood of the work |  
| format | string | Main medium and/or format of the work |  
|<hr>|<hr>|<hr>|
| credits | string | Array of song credits |  
| link | string | A link where the work can be purchased or interacted with |  

| license | string | Declare license, (Copyright, CC0, MIT, etc) |  
| rarity | string | How scarce is this NFT? Abundant Common Uncommon Rare Epic Mythic Unique |  


# Web 4 Options
Web4 adds **geographic** and **temporal** information on top of web3. You'll find full + lite options for each available for each standard: 

## Full geotemporal options 
| Field | Type | Description | 
| :----:  | :----: | :---- |
| timestamp  | string | Timestamp for the publication of the work (simplifies + supercedes date) |
| date | string | Date when the work was published (supercedes / replaces Year/Month/Day) Recommended format is ISO 8601 "YYYY-MM-DD" because "MM-DD-YYYY" can be confused with "DD/MM/YYYY" but it's up to you. To cover all bases, set timestamp field as a backup |
| year       | string | Year when the work was published. Format: "YYYY". ⚠️ It's best to use either date or year/month/day, not both. |
| month      | string | Month when the work was published. Format: "MM" or English abbreviation (e.g., "Jan", "Feb", etc.) or full month name |
| day        | string | Day when the work was published. Format: "DD" or "D" |
|<hr>|<hr>|<hr>|
| location   | string | Full location information in one field, format: "City, State, Nation" Use this |
| nation     | string | Three-letter ISO country code (e.g., "USA", "BRA", "AUS", etc.) Please don't use anything else, as this is the easiest format for any application to integrate |
| state      | string | State or province for the location, format: Abbreviation convention used in nation (e.g., California as "CA", Antioquia as "ANT") |
| city       | string | City for the location, format: "City Name" |
| geotag     | string | GeoJSON Point stored as string, format "lat,lng" (e.g., "37.7749,-122.4194"), or a "[lat,lng]" coordinate array (e.g., "[37.7749, -122.4194]") |  

> You may inpmement all options to allow templates of he same schema to choose what's best for them, instead of modifying it and keeping it for future unknown templates. 

## Implementation Options

You'll find code blocks for the various NFT Standards. 

You can either copy/paste them, as shown in the [Instructional Video](https://www.youtube.com/watch?v=GXjBQnV_Xm8) or simply create a new schema on [Atomichub.io](https://wax.atomichub.io/) and type in each field you would like to implement. 

For **detailed instructions** on how to use, see this [article](https://medium.com/p/5b3f951bff05). 


### RAM Usage
While you may see more fields than you'd like to implement in your final NFT, it's okay to use them for the schema. This will make the ram requirement of schema creation slightly larger, but you'll only be charged for the fields you use when creating templates + NFTs.


> This metadata is written specifically for Atomic Asset's [NFT standard](https://github.com/pinknetworkx/atomicassets-contract) on the [atomicassets contract](https://wax.bloks.io/account/atomicassets). 

Feel free to fork, or open an issue to see improvement. 

# 🛠 WAX NFT Metadata Standard
For specific use cases, use these versions:
[./Standards](./Standards/literature.md) 

| Use Case | Link | 
| :----:  | :---- | 
| Literature | [Standards/literature.md](./Standards/literature.md) |
| Photo | [Standards/photo.md](./Standards/photo.md) |
| Video | [Standards/video.md](./Standards/video.md) |
| Music (Pending) | [Standards/music.md](./Standards/music.md) |

> Works with Atomichub UI out of the box. You can even avoid touching this code by using Create Schema on atomichub to replicate. 

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



# Mini-Changelog

1.0.0 - Initial Release (WIP)


# Support this development

This development is sponsored by [WAX Labs](https://labs.wax.io)

