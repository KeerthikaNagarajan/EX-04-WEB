# Ex-04:
## CREATE A WEB-LAYOUT USING GRIDBOX
### AIM:
The aim of this code is to create a web layout using CSS Grid, which provides a powerful grid system for arranging elements on a webpage.
### ALGORITHM:
1. Create an HTML document with the necessary structure, including the doctype declaration, title tag, and style tag.
2. Set the CSS to make the body element a grid container using the display property set to "grid".
3. Add a grid-gap to create some spacing between the grid items.
4. Apply styles to the header, footer, article, nav, and div elements to set their background color and padding.
5. Use the grid-area property to assign specific grid areas to each element, matching the names defined in the grid-template-areas property.
6. Close the style tag and include the header, article, nav, div, and footer elements within the body of the HTML document, assigning them corresponding IDs to match the grid areas.
### PROGRAM:
```html
<!doctype html>
<title>Example</title>
<style>
body { 
  display: grid;
  grid-template-areas: 
    "header header header"
    "nav article ads"
    "footer footer footer";
  grid-template-rows: 60px 1fr 60px;
  grid-template-columns: 20% 1fr 15%;
  grid-gap: 10px;
  height: 100vh;
  margin: 0;
  }
header, footer, article, nav, div {
  padding: 20px;
  background: rgb(63, 97, 102);
}
#pageHeader {
  grid-area: header;
}
#pageFooter {
  grid-area: footer;
}
#mainArticle { 
  grid-area: article;      
  }
#mainNav { 
  grid-area: nav; 
  }
#siteAds { 
  grid-area: ads; 
  }
</style>
<body>
  <header id="pageHeader">Header</header>
  <article id="mainArticle">Article</article>
  <nav id="mainNav">Nav</nav>
  <div id="siteAds">Ads</div>
  <footer id="pageFooter">Footer</footer>
</body>

```
### OUTPUT:
<img width="1279" alt="1" src="https://github.com/KeerthikaNagarajan/WEB-LAYOUT-USING-GRIDBOX/assets/93427089/c9ab66b2-31f9-45c4-b878-7ab9f2ceeecd">

### RESULT:
The code will generate a webpage with a grid layout. 
