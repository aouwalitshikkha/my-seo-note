# Contact Us Page Schema
This Contact Us page is a functional communication page, not content.

স্কীমা হবে অনেকটাই এবাউট আসের মত ।

```
Organization
WebSite
WebPage (type: ContactPage)
```

## কন্টাক্ট আস স্কীমার কোড 

```json
{
  "@context": "https://schema.org",
  "@graph": [

    {
      "@type": "Organization",
      "@id": "https://gimbalsinsider.com/#organization",
      "name": "Gimbals Insider",
      "url": "https://gimbalsinsider.com/",
      "logo": {
        "@type": "ImageObject",
        "url": "https://gimbalsinsider.com/wp-content/uploads/2025/05/cropped-favicon-02-scaled-1.png"
      },
      "contactPoint": {
        "@type": "ContactPoint",
        "email": "Informations@gimbalsinsider.com",
        "telephone": "+1-555-486-8736",
        "contactType": "customer support",
        "availableLanguage": "English"
      },
      "sameAs": [
        "https://www.facebook.com/gimbalsinsider",
        "https://www.instagram.com/gimbalsinsider/",
        "https://www.linkedin.com/company/gimbalsinsider/"
      ]
    },

    {
      "@type": "WebSite",
      "@id": "https://gimbalsinsider.com/#website",
      "url": "https://gimbalsinsider.com/",
      "name": "Gimbals Insider",
      "publisher": {
        "@id": "https://gimbalsinsider.com/#organization"
      },
      "inLanguage": "en-US"
    },

    {
      "@type": "ContactPage",
      "@id": "https://gimbalsinsider.com/contact-us/#contactpage",
      "url": "https://gimbalsinsider.com/contact-us/",
      "name": "Contact Gimbals Insider",
      "description": "Get in touch with Gimbals Insider for support, partnerships, or general inquiries.",
      "isPartOf": {
        "@id": "https://gimbalsinsider.com/#website"
      },
      "about": {
        "@id": "https://gimbalsinsider.com/#organization"
      },
      "inLanguage": "en-US"
    }

  ]
}
```