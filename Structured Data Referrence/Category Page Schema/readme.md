# Category Page Schema

ক্যাটাগরি পেজে নিচের স্কীমা গুলা গুরুত্বপুর্ন 

## অর্গানাইজেশন ক্সীমা 


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
## ওয়েব সাইট স্কীমা ( অপশনাল )

```json 
{
  "@type": "WebSite",
  "@id": "https://gimbalsinsider.com/#website",
  "url": "https://gimbalsinsider.com/",
  "name": "Gimbals Insider",
  "publisher": {
    "@id": "https://gimbalsinsider.com/#organization"
  },
  "inLanguage": "en-US"
}
```

## কালেকশন পেজ স্কীমা 

```
{
  "@type": "CollectionPage",
  "@id": "https://gimbalsinsider.com/gimbal-guide/gimbal-buying-guides/#webpage",
  "url": "https://gimbalsinsider.com/gimbal-guide/gimbal-buying-guides/",
  "name": "Gimbal Buying Guides",
  "description": "In-depth gimbal buying guides, comparisons, and recommendations to help you choose the best gimbal.",
  "isPartOf": {
    "@id": "https://gimbalsinsider.com/#website"
  },
  "about": {
    "@type": "Thing",
    "name": "Gimbal Buying Guides"
  },
  "inLanguage": "en-US"
}
```

## আইটেম লিস্ট 
```json
{
  "@type": "ItemList",
  "name": "Gimbal Buying Guide Articles",
  "itemListOrder": "Descending",
  "numberOfItems": 2,
  "itemListElement": [
    {
      "@type": "ListItem",
      "position": 1,
      "url": "https://gimbalsinsider.com/dji-osmo-mobile-6-vs-dji-osmo-mobile-7p/"
    },
    {
      "@type": "ListItem",
      "position": 2,
      "url": "https://gimbalsinsider.com/dji-osmo-mobile-7p-vs-insta360-flow-2-pro/"
    }
  ]
}
```

# একসাথে সব ক্যাটাগরি পেজ স্কীমা 

```json
{
  "@context": "https://schema.org",
  "@graph": [
    { "Organization": {} },
    { "WebSite": {} },
    { "CollectionPage": {} },
    { "ItemList": {} }
  ]
}
```


