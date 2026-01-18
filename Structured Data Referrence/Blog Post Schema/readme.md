# Blog Post Schema

ব্লগ পোষ্ট স্কীমাতে নিচের গুলা প্রয়োজনীয় 

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

## ওয়েব পেজ স্কীমা 

```json
 {
      "@type": "WebPage",
      "@id": "https://gimbalsinsider.com/dji-osmo-mobile-6-vs-dji-osmo-mobile-7p/#webpage",
      "url": "https://gimbalsinsider.com/dji-osmo-mobile-6-vs-dji-osmo-mobile-7p/",
      "name": "DJI Osmo Mobile 6 vs DJI Osmo Mobile 7P: Who Really Wins",
      "isPartOf": {
        "@id": "https://gimbalsinsider.com/#website"
      },
      "primaryImageOfPage": {
        "@id": "https://gimbalsinsider.com/wp-content/uploads/2025/11/DJI-Osmo-Mobile-6-vs-DJI-Osmo-Mobile-7P-Who-Really-Wins-scaled.webp"
      },
      "datePublished": "2025-11-17T13:36:39-06:00",
      "dateModified": "2025-11-17T14:21:11-06:00",
      "inLanguage": "en-US"
    }
```

## পার্সন স্কীমা 

যদি মাল্টিপল অথর ইউজ করে তখন পার্সন স্কীমা দিতে হয়  । নাহলে দরকার নাই 
```json
    {
      "@type": "Person",
      "@id": "https://gimbalsinsider.com/author/shuvo/",
      "name": "Gimbals Insider Team",
      "url": "https://gimbalsinsider.com/author/shuvo/"
    }
```

## ব্লগ পোষ্টিং স্কীমা 

```json
 {
      "@type": "BlogPosting",
      "@id": "https://gimbalsinsider.com/dji-osmo-mobile-6-vs-dji-osmo-mobile-7p/#blogposting",
      "headline": "DJI Osmo Mobile 6 vs DJI Osmo Mobile 7P: Who Really Wins",
      "description": "Confused about DJI Osmo Mobile 6 vs DJI Osmo Mobile 7P? Compare setup, tracking, battery, and creator tools to see which smart gimbal truly suits you best.",
      "image": {
        "@id": "https://gimbalsinsider.com/wp-content/uploads/2025/11/DJI-Osmo-Mobile-6-vs-DJI-Osmo-Mobile-7P-Who-Really-Wins-scaled.webp"
      },
      "author": {
        "@id": "https://gimbalsinsider.com/author/shuvo/"
      },
      "publisher": {
        "@id": "https://gimbalsinsider.com/#organization"
      },
      "articleSection": "Gimbal Buying Guides",
      "keywords": [
        "DJI Osmo Mobile 6 vs DJI Osmo Mobile 7P",
        "DJI Osmo Mobile comparison",
        "best smartphone gimbal"
      ],
      "datePublished": "2025-11-17T13:36:39-06:00",
      "dateModified": "2025-11-17T14:21:11-06:00",
      "mainEntityOfPage": {
        "@id": "https://gimbalsinsider.com/dji-osmo-mobile-6-vs-dji-osmo-mobile-7p/#webpage"
      },
      "inLanguage": "en-US"
    }
```
## আর্টিকেল স্কীমা 

কিছু ক্ষেত্রে আর্টিকেল স্কীমা ইউজ করা যায় । নিচে পার্থক্য দেওয়া হল কখন  ইউজ করা যায় । 
```
{
  "@context": "https://schema.org",
  "@type": "Article",
  "@id": "https://example.com/what-is-a-gimbal/#article",
  "headline": "What Is a Gimbal? A Complete Beginner’s Explanation",
  "description": "Learn what a gimbal is, how it works, and why it is used for video stabilization in cameras and smartphones.",
  "image": {
    "@type": "ImageObject",
    "url": "https://example.com/wp-content/uploads/what-is-a-gimbal.webp",
    "width": 1200,
    "height": 675
  },
  "author": {
    "@type": "Person",
    "name": "John Doe"
  },
  "publisher": {
    "@type": "Organization",
    "name": "Example Media",
    "logo": {
      "@type": "ImageObject",
      "url": "https://example.com/logo.png",
      "width": 600,
      "height": 60
    }
  },
  "datePublished": "2025-01-10T08:00:00+00:00",
  "dateModified": "2025-01-12T10:30:00+00:00",
  "mainEntityOfPage": {
    "@type": "WebPage",
    "@id": "https://example.com/what-is-a-gimbal/"
  },
  "inLanguage": "en-US"
}
```


## কখন ব্লগ পোষ্টিং বা আর্টিকেল 
| Feature           | Article Schema              | BlogPosting Schema                  |
| ----------------- | --------------------------- | ----------------------------------- |
| Schema Type       | `Article`                   | `BlogPosting` (subtype of Article)  |
| Content Nature    | Neutral, factual, reference | Editorial, opinionated, guide-style |
| Writing Tone      | Objective, encyclopedic     | Conversational, explanatory         |
| Author Style      | Expert or editorial team    | Individual or brand team            |
| Update Frequency  | Low                         | Medium to high                      |
| Monetization      | Usually none                | Often affiliate / ads               |
| Best For          | Definitions, explanations   | Guides, reviews, comparisons        |
| Google Discover   | Rare                        | Common                              |
| Typical Site Type | Knowledge base, docs        | Blogs, magazines                    |
| Can be combined?  | ❌ No                        | ❌ No                               |


## বাস্তব উদাহরন 

### আর্টিকেল স্কীমার উদাহরন 

| Page Title | Why Article Fits |
| ---------- | ---------------- |
| What Is a Gimbal? | Pure definition |
| How Camera Stabilization Works | Educational explanation |
| Types of Gimbals Explained | Reference-style content |
| History of Gimbal Technology | Informational article |

---

### ব্লগ পোষ্টিং স্কীমার উদাহরন 

| Page Title | Why BlogPosting Fits |
| ---------- | -------------------- |
| DJI Osmo Mobile 6 vs DJI Osmo Mobile 7P | Product comparison |
| Best Smartphone Gimbals in 2025 | Buying guide |
| DJI Osmo Mobile 7P Review | Review article |
| How I Shot Travel Videos With OM 7P | Experience-based post |
