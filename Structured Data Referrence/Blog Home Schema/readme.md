# Home Page Structured Data

হোম পেজে বাধ্যতামুলক থাকতে হয় ওয়েব সাইট স্কীমা । ওয়েব সাইট স্কীমার মুল উদ্দেশ্য হচ্ছে ব্রান্ড আইডেন্টিটি ও সাইট লিংক সার্চ বক্স ।

```json
{
  "@type": "WebSite",
  "@id": "https://gimbalsinsider.com/#website",
  "url": "https://gimbalsinsider.com/",
  "name": "Gimbals Insider",
  "publisher": {
    "@id": "https://gimbalsinsider.com/#organization"
  },
  "potentialAction": {
    "@type": "SearchAction",
    "target": "https://gimbalsinsider.com/?s={search_term_string}",
    "query-input": "required name=search_term_string"
  }
}
```
উপরে সাইটের সার্চ লিংক অনুসারে রিপ্লেস হবে 


## অর্গানাইজেশন স্কীমা 

অর্গানাইজেশন স্কীমার মুল উদ্দেশ্য হল নলেজ গ্রাফ, ব্রান্ড ট্রাস্ট , লোগো , সোশ্যাল প্রোফাইল । মুলত EEAT তে সাহায্য করে 

```json
{
  "@type": "Organization",
  "@id": "https://gimbalsinsider.com/#organization",
  "name": "Gimbals Insider",
  "url": "https://gimbalsinsider.com/",
  "logo": {
    "@type": "ImageObject",
    "url": "https://gimbalsinsider.com/wp-content/uploads/2025/05/cropped-favicon-02-scaled-1.png"
  },
  "sameAs": [
    "https://www.facebook.com/gimbalsinsider",
    "https://www.instagram.com/gimbalsinsider/",
    "https://www.linkedin.com/company/gimbalsinsider/"
  ]
}

```

##  কালেকশন পেজ 
এটা মুলত  হোম পেজ যদি কালেকশন পেজ হয় অনেক ব্লগের তাহলে দরকার । নাহলে দরকার কনাই । 

```json
{
  "@type": "CollectionPage",
  "@id": "https://gimbalsinsider.com/#webpage",
  "url": "https://gimbalsinsider.com/",
  "name": "Gimbals Insider | Where Gimbal Enthusiasts Level Up",
  "isPartOf": {
    "@id": "https://gimbalsinsider.com/#website"
  },
  "about": {
    "@id": "https://gimbalsinsider.com/#organization"
  },
  "inLanguage": "en-US"
}
```

## আইটেম লিস্ট
ফিচার্ড পোষ্ট ও ইন্টারলিংক এ হেল্প করে । 
```
{
  "@type": "ItemList",
  "name": "Featured Post",
  "itemListOrder": "Descending",
  "numberOfItems": 3,
  "itemListElement": [
    {
      "@type": "ListItem",
      "position": 1,
      "url": "https://gimbalsinsider.com/how-does-a-gimbal-work/"
    },
    {
      "@type": "ListItem",
      "position": 2,
      "url": "https://gimbalsinsider.com/how-to-use-a-gimbal/"
    },
    {
      "@type": "ListItem",
      "position": 3,
      "url": "https://gimbalsinsider.com/difference-between-gimbal-and-stabilizer/"
    }
  ]
}
```
## এফ এ কিউ ( FAQ )
যদিও হোম পেজে এফ এ কিউ দেখানো হয় বাট এইটা না দেওয়াই ভালো । 

## হোম পেজের সব স্কীমা একসাথে 

```json
{
  "@context": "https://schema.org",
  "@graph": [
    { "WebSite" },
    { "Organization" },
    { "CollectionPage" },
    { "Blog" },
    { "ItemList" }
  ]
}
```