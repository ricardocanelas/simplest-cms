[API-First CMS]

# Simplest CMS

It's a Content Management System for SPA (single-page application) websites.

- No database
- Simple authentication
- You create your own structure
- License MIT

You will need to make sure your server meets the following requirements:

- PHP >= 5.4.0
- JSON PHP Extension


## 🔹 Get Started

### Install

```
npx simplest-cms <your-directory>
```

### Config

After install, edit the file "**config.php**":

### To Access

By standard the file is *data.json*

---

## 🔹 API

⚠️ *Working...*

### Fields

**Types**

- [x] text
- [x] textarea
- [ ] select
- [ ] checkbox
- [ ] radio
- [ ] number
- [ ] email
- [ ] range
- [ ] search
- [ ] time
- [ ] datetime
- [ ] datetimelocal
- [ ] week
- [ ] month
- [ ] year
- [ ] editorhtml
- [ ] editormarkdown
- [ ] url
- [ ] image
- [ ] created_at
- [ ] updated_at
- [ ] one
- [ ] many
- [ ] slug

**Options**

- [ ] unique
- [x] required
- [x] not-required
- [x] default
- [ ] min
- [ ] max
- [ ] mask

### Schema

**Config**

- [ ] limit

---

## 🔹 Example

In config.php

```php
// ...

"collections" => [
  "people" => [
    "firstname" => "text",
    "lastname" => "text not-required",
    "work" => "text"
  ],
]
```

In JavaScript:

```js
const getData = fetch(`./data.json`)
 .then(res => res.json())

getData().then(data) => {
  console.log('All data:', data)
}
```