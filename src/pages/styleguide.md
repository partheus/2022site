---
title: "Styleguide"
description: 'A simple text styleguide for layout and UI practice'
date: 2022-03-11
---

# Header 1

Text: **Bold**, _Italic_, or ~~Strikethrough~~.

[Link](/about).

## Header 2

> This is a blockquote following a header.

### Header 3

<!-- ```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require("./lang/" + l);
  return true;
};
``` -->

#### Header 4

- This is an unordered list following a header.
- This is an unordered list following a header.
- This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

### There's a horizontal rule below this.

---

### Here is an unordered list:

- Item foo
- Item bar
- Item baz
- Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

<br>
<div class="irevamp-section slide-up">
    <h5>Test 3-Up Cards:</h5>
    <ul class="irevamp-column-container">
      {%- for page in collections.pages | reverse -%}
      <li class="irevamp-card">
        <div class="irevamp-card__content">
          <a href="{{ page.url }}" class="irevamp-card__title bold600">{{ page.data.title }}</a>
          <p class="irevamp-lead">{{ page.data.description }}</p>
          <p class="irevamp-card__date">{{ page.data.date | postDate  }}</p>
        </div>
      </li>
      {%- endfor -%}
    </ul>
</div>