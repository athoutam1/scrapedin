![](https://github.com/linkedtales/scrapedin/raw/master/logo.png)
[![Build Status](https://travis-ci.org/leonardiwagner/scrapedin.svg?branch=master)](https://travis-ci.org/leonardiwagner/scrapedin)
[![NPM version](https://img.shields.io/npm/v/scrapedin.svg)](https://www.npmjs.com/package/scrapedin)

---

Last working in May 2020

Fork of [Scrapedin](https://github.com/linkedtales/scrapedin)

## Key Differences

- Removed courses section from being scraped (unresolved issue - scraper errors if a profile doesn't have any courses listed)
- Can scrape the image from each company
- Can scrape certificates section

`yarn add scrapedin`

### Usage Example:

```javascript
const scrapedin = require("scrapedin");

const profileScraper = await scrapedin({
  email: "login@mail.com",
  password: "pass",
});
const profile = await profileScraper(
  "https://www.linkedin.com/in/some-profile/"
);
```

- If you are looking for a crawler to automatically extract multiple profiles see [scrapedin-crawler](https://github.com/linkedtales/scrapedin-linkedin-crawler)

### Start Guide:

- [Basic Tutorial](https://github.com/linkedtales/scrapedin/wiki/Basic-Tutorial)
- [Using Cookies to Login](https://github.com/linkedtales/scrapedin/wiki/Using-Cookies-To-Login)
- [Tips](https://github.com/linkedtales/scrapedin/wiki/Tips)
- [Documentation](https://github.com/linkedtales/scrapedin/wiki/Documentation)
