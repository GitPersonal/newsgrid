# News Grid notes

## link for mobile

We only want the mobile.css to show if the screen is less than 768px

```html

<link rel="stylesheet" media="screen and (max-width: 768px)" href="css/mobile.css">

```

---

Using `Font Awesome`
[Font Awesome](https://fontawesome.com/account/cdn)

     - start free
    - login to account
    - click on profile icon
    - click font awesome cdn
    - scroll down to copy link icon
    - paste above the first stylesheet

---

Convert logo to favicon
[Dynamicdrive favicon](https://tools.dynamicdrive.com/favicon/)

    - upload png image
    - click create icon button
    - download
    - take the downloaded icon over to the root folder. Not to the image folder
    - copy the link snippet from the bottom of the Dynamicdrive favicon page and paste it as the last stylesheet.
    - in the link, remove the / in the href="/favicon"
    - refresh the page to see the favicon. You might need a hard refresh. comand + shift + R
    
---

## Create root variables for colors

```css
    :root {
        --primary-color: #c72727;
        --secondary-color: #f99500;
        --light-color: #f3f3f3;
        --dark-color: #333;
        --max-width: 1100px;
    }
```

Go to Google Fonts to search for both fonts.

Seach for Lato and add the font to use. Go in the search box and search for Staatliches. Add this font also. Copy the link css stylesheet.

Paste the link stylesheets above all the other stylesheets.

[Google Fonts](https://fonts.google.com/)

[Google Fonts Lato](https://fonts.google.com/)

[Google Fonts Staatliches](https://fonts.google.com/specimen/Staatliches?query=staat&preview.text_type=custom)

---

Include a rest

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Lato', sans-serif;
    line-height: 1.5;
    background: var(--light-color);
}

a{
   color: #333;
   text-decoration: none;
}

```

---

When aligning the actual item itself use `justify-self`. 

If using the parent use `justify-content`

---

Use this hover css to style buttons. Will have effect on buttons.

```css
.btn:hover {
    opacity: 0.9;
}
```

---

Could use this to target the first child in `.article`.

```css

#home-articles .articles-container .article:first:first-child {
  
}

```

Could use this to target the first child in any element.

```css

#home-articles .articles-container > *:first-child {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
}

```

`Grid is good for layout like building boxes`

`Flex is good for the inner elements aligning and menu`
