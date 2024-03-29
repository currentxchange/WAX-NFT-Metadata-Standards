## WAX NFT Metadata Standards

```Javascript
// -- Stats -- \\
Version: 1.0.1
Supported Types: Image, Photo, Literature, Music, Video
Published: standards.cXc.world
```

### Mint professional-looking NFTs
The WAX NFT metadata standards are a collection of fields to use when creating your schema on Atomic Assets. We provide copy-paste, plug-and-play schemas that work with the most popular markets on WAX, starting with [Atomichub](https://wax.atomichub.io/), [NFThive](https://nfthive.io/), [WAXdao](https://waxdao.io/) and more.

## Let's GOO!!! 🚀 

Take the [Tutorial to start your collection](https://standards.cxc.world/tutorial)

### ⚡️ Use the new UI to easily create your schema [tools.cXc.world](https://tools.cXc.world)

Find each standard below

|         Use Case        | Link                                                                                      |
| :---------------------: | ----------------------------------------------------------------------------------------- |
|        Literature       | [media/literature.md](https://standards.cxc.world/media/literature)   |
|          Video          | [media/video.md](https://standards.cxc.world/media/video)                             |
|          Image          | [media/image.md](https://standards.cxc.world/media/image)                             |
|          Photo          | [media/photo.md](https://standards.cxc.world/media/photo)                             |
|          Music          | [media/music.md](https://standards.cxc.world/media/music)                             |
| Original Music Standard | [currentxchange/Music-NFT-Standard](https://github.com/currentxchange/Music-NFT-Standard) |

## About the Standards

Each standard uses these basic fields, and expands to a type-specific list of fields.

The individual standards are linked farther down, and exist in the [standards.cxc.world/media](https://standards.cxc.world/media) directory.

`string` just means text, `ipfs` is an [ipfs hash](https://www.pinata.cloud/) of the data.

|     Field     |  Type  | Description                                                                                                                                                                                                                 |
| :-----------: | :----: | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|      name     | string | NFT name                                                                                                                                                                                                                    |
|      img      |  ipfs  | Primary image, because this is an IPFS field, you can use a video here as well, under 7mb weight recommended                                                                                                                |
|     artist    | string | The artist, for multiple creators see the credits field                                                                                                                                                                     |
|     title     | string | The title of the work                                                                                                                                                                                                       |
|     about     | string | Description field with main info about the work                                                                                                                                                                             |
|    backimg    |  ipfs  | Back of the art/book, or used as supplementary artwork                                                                                                                                                                      |
| collectionimg |  ipfs  | Extra image for Collection, optional                                                                                                                                                                                        |
|      <hr>     |  <hr>  | <hr>                                                                                                                                                                                                                        |
|     genre     | string | Genre of the work                                                                                                                                                                                                           |
|      mood     | string | Mood of the work                                                                                                                                                                                                            |
|     format    | string | Main medium and/or format of the work. This may be used to declare a type/category like "short story" for literature                                                                                                        |                                                                                                                          |
|      <hr>     |  <hr>  | <hr>                                                                                                                                                                                                                        |
|    credits    | string | List creator credits, suggested format "Script: Gudasol, Director: Pixy the Unicorn"                                                                                                                                        |
|      link     | string | A link or links where the work can be purchased or interacted with. You can link to multiple platforms for purchase, playback, etc. Suggested format "Platformone: link.to/platformone \| Platformtwo: link.to/platformtwo" |
|     promo     |  ipfs  | Promotional video or photo related to work or project                                                                                                                                                                       |
|    license    | string | Declare license (Copyright \[Year], CC0, MIT, etc)                                                                                                                                                                          |
|      labels     | string | Topics related to the NFT as a comma-separated list                                                                                                                                                                         |
|     rarity    | string | How scarce is this NFT? Abundant Common Uncommon Rare Epic Mythic Unique                                                                                                                                                    |

## Web 4 Options

Web4 adds **space** and **time** information on top of web3. You'll find timespace + light options for each available for each standard:

### Full timespace options

|   Field   |  Type  | Description                                                                                                                                                                                                                                                               |
| :-------: | :----: | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| timestamp |  int64 | Timestamp for the publication of the work (simplifies + supercedes date)                                                                                                                                                                                                  |
|    date   | string | Date when the work was published (supercedes / replaces Year/Month/Day) Recommended format is ISO 8601 "YYYY-MM-DD" because "MM-DD-YYYY" can be confused with "DD/MM/YYYY" but it's up to you. To cover all bases, set timestamp field as a backup, or use year/month/day |
|    year   |  int64 | Year when the work was published. Format: "YYYY". ⚠️ It's best to use either date or year/month/day, not both.                                                                                                                                                            |
|   month   | string | Month when the work was published. Format: "MM" or English abbreviation (e.g., "Jan", "Feb", etc.) or full month name                                                                                                                                                     |
|    day    |  int64 | Day when the work was published. Format: "DD" or "D"                                                                                                                                                                                                                      |
|    <hr>   |  <hr>  | <hr>                                                                                                                                                                                                                                                                      |
|  location | string | Full location information in one field, format: "City, State, Nation" ⚠️ Use this or nation/state/city, not both                                                                                                                                                          |
|   nation  | string | Three-letter ISO country code (e.g., "USA", "BRA", "AUS", etc.) Please don't use anything else, as this is the easiest format for any application to integrate                                                                                                            |
|   state   | string | State or province for the location, format: Abbreviation convention used in nation (e.g., California as "CA", Antioquia as "ANT")                                                                                                                                         |
|    city   | string | City for the location, format: "City Name"                                                                                                                                                                                                                                |
|   geotag  | string | TopoJSON Point stored as string, format "lat,lng" (e.g., "37.7749,-122.4194"), or a "\[lat,lng]" coordinate array (e.g., "\[37.7749, -122.4194]")                                                                                                                         |

> You may inpmement all options to allow templates of he same schema to choose what's best for them, instead of modifying it and keeping it for future unknown templates.

### Implementation Options

You'll find code blocks for the various NFT Standards.

You can either copy/paste them, as shown in the [Instructional Video](https://www.youtube.com/watch?v=GXjBQnV\_Xm8) or simply create a new schema on [Atomichub.io](https://wax.atomichub.io/) and type in each field you would like to implement.

For **detailed instructions** on how to use, see this [article](https://medium.com/p/5b3f951bff05).

#### RAM Usage

While you may see more fields than you'd like to implement in your final NFT, it's okay to use them for the schema. This will make the [RAM requirement](https://anyobservation.medium.com/basic-wax-account-management-d956d74ff103) of schema creation slightly larger, but you'll only be charged for the fields you use when creating templates + NFTs.

> This metadata is written specifically for Atomic Assets' [NFT standard](https://github.com/pinknetworkx/atomicassets-contract) on the [atomicassets contract](https://wax.bloks.io/account/atomicassets).

Feel free to fork, or open an issue to see improvement.

## 🛠 WAX NFT Metadata Standard

For specific use cases, use these versions: [standards.cxc.world/media](https://standards.cxc.world/media)

|         Use Case        | Link                                                                                      |
| :---------------------: | ----------------------------------------------------------------------------------------- |
|        Literature       | [media/literature.md](https://standards.cxc.world/media/literature)      |
|          Video          | [media/video.md](https://standards.cxc.world/media/video)                             |
|          Image          | [media/image.md](https://standards.cxc.world/media/image)                             |
|          Photo          | [media/photo.md](https://standards.cxc.world/media/photo)                             |
|          Music          | [media/music.md](https://standards.cxc.world/media/music)                             |
| Original Music Standard | [currentxchange/Music-NFT-Standard](https://github.com/currentxchange/Music-NFT-Standard) |

> Works with Atomichub UI out of the box. You can even avoid touching this code by using Create Schema on atomichub to replicate.

## Light Version 🌞

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

## Spacetime Version 🛸

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

## Mini-Changelog

1.0.0 - Initial Release - October 19, 2023 Added initial media standards released to [standards.cxc.world](https://standards.cxc.world/)

## Support this development

This development is made possible through [WAX Labs](https://labs.wax.io). Support NFT artists by purchasing + trading their NFTs.
