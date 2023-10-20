## How to Use the WAX NFT Metadata Standards

Using the WAX NFT Metadata Standards to create your own NFT project involves three key steps:

    1. Set up a collection
    2. Add the schema
        a. Copy one of the JSON objects found at [standards.cXc.world/media](https://standards.cXc.world/media)
            Pick the media type
            Pick the version, Light or Spacetime
            Click the copy button at the top-right of the code block 
        b. Paste the code into the `idata`` field using the [createschema](https://waxblock.io/account/atomicassets?action=createschema#contract-actions) action.
    3. Create templates for each piece of art you'll mint
    *Now, mint as many NFTs as you want..*

## 1. Set Up a Collection

First, you need to set up your own collection on AtomicHub. Follow the marketplace’s process for registering a new collection.

For example, on AtomicHub you would:

 1. Click “View Profile” after clicking the three lines in top right

 2. Click “Collections”

 3. Click the “+ Create New Collection” button

 4. Fill out details + click “Save” at the bottom.

 > See the (aging) [instructions from the Pink, creators of Atomic Assetd](https://pinkgg.medium.com/guide-using-the-atomichub-nft-creator-7bd2b017224b) for more info, and return when you have a collection, as implementing the standard is much faster using the method described here.

## 2. Add the Schema
Once your collection is created, you need to add the one of the NFT standards, which are implemented as schemas (called categories on the new Atomichub site). There are two options:

**[Recommended] Option 1:  Paste the Code on Waxblock.io** — The easier way is to copy the schema code from the [GitHub repo](https://standards.cxc.world/media/) and paste it into the idata field when using the [createschema](https://waxblock.io/account/atomicassets?action=createschema#contract-actions) action on Atomic Assets. 

![This is the “easy” way if you’re comfortable sending an action from waxblock.io](https://files.peakd.com/file/peakd-hive/currentxchange/23uQJGQZ6KhzbpjxZ7EgZ4oUaGjG3E6cEox5GnqBZfABBGYGC1yybGisj7eJsZYnYxSnQ.png)


**Option 2: Manually through Atomichub** — You can manually re-create the schema in your collection by adding each field one-by-one through the UI.

 1. Go to your new collections page at profile > collections > manage collection

 2. Click the “Templates” tab, then click “+ Create New Category”

![This way may seem easier if you’re code-shy, but it takes more time to fill in each field and is easier to make a typo or other mistake](https://files.peakd.com/file/peakd-hive/currentxchange/23tGTdnDbeQRK1hFemKJKNCKHxT7Ln1HDQykKLH4qBUJy4hTYZJ43aTqrGRpKrLyqjQ6A.png)

3. Fill in each field manually


## 3. Create Templates

Use your schema to generate NFT templates in your collection. On AtomicHub, you would:

 1. From profile > collections, find your collection and click “Manage collection”

 2. Click the “Templates” tab, then click “+ Create New Template”

 3. Fill in the fields + click “Save”




### Once you’ve created a template, you can mint NFTs from it anytime.

Platforms like [Atomichub](https://wax.atomichub.io/) and [Neftyblocks](https://neftyblocks.com/) make it easy to generate templates from your schema + NFTs from your templates without needing to code. Platforms like [cXc.world](https://cXc.world/f/nft) let you compete with other NFT artists, and tools like [waxdao.io](https://waxdao.io/) let you incentivize your NFT holders with token rewards.

![Go the NFTs tab and click “Create new NFT”, Select the category, fill out the fields, hit save](https://files.peakd.com/file/peakd-hive/currentxchange/23uQNzCAu7YbbVZPLvyCba4oApqQYvgdRAGnVTyUD5msw5eHAjm7XP4FFSjPEgw3uviSo.png)


# Visual learner? Here's an [Instructional Video](https://www.youtube.com/watch?v=GXjBQnV_Xm8).