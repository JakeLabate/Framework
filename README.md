## Higherarchical Content Map
Ex:

- Universal campaign
- Campaign branch
- Sub-campaign
- Content Piece (ex: email/blog post/webpage)
- Content Sections (ex: hero website section/blog section/paragraph in an email)
- Content Item (ex: Call to Action)
- Word (ex: Call)

(Of course this will changed based on the content type.)

Where does generative AI tools (like Dalle or ChatGPT or GPT4 etc etc) play in this? Can we prompt this? What should be templated in not an AI prompt? Do we design prompts for AI? etc etc... getting the 'word' perfect seems like a fools errand when we have access to these generative AI tools that can get pretty damn good at things much larger than the level of the 'word'.

Might this be broken down into (what we could call) groups?
- A 'social media' group, might be in an email signaure... which may be comprised of all links we have on a person...
- A 'name' group might be anywhere... this may comprised of a first, middle, last and nickname...
- By grouping varaibles... we can consolidate the framework. This may also make them re-usable across content types and content type variations.

## Data Storage Schema
What is the ideal schema of the stored brand variables?

Ex:
- Do we `need` a `<title>` for each `webpage`?
- Do we `need` or `want` a `title` and/or `alt` for every `image`?

```js
const brand = {
  offers: {
    offer1: {
      name: "Worlds Biggest Tomato",
      price: "$5,000",
      media: {
        images: {
          image1: {
            src: "https://i.dailymail.co.uk/i/pix/scaled/2015/01/23/24F8A1AC00000578-0-image-a-50_1422015746402.jpg",
            alt: "Image 1 Alt",
            height: "800px",
            width: "1200px"
          }
        }
      }
    }
  }
}
```

## Auto-Data Gathering Framework
How we collect data based on data we have, can infer, etc.

Ex:
- Can we get a domain from an email?
- Can we scrape a website to collect social media URLs?
- Can we get a lat/long coordinated from an address?
- Can we get a range of color schemes from a logo?
- Can we generate an alt tag from a logo via image-object regocnition AI?

This would prevent the need to ask for the data from the user.

## User Interface
### Tasks
#### Task Prioritization Framework

Assuming our `Data Gathering Framework` cannot/does not get valid info for something... how do we show prioritize how we ask for inputs from the user?

Ex:
- Does a `what-is-the-areaCode-for-this-phoneNumber-variable?` task take priority over `how-often-should-we-post-to-{{this}}-platform` task?
