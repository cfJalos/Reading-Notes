[Home page](https://cfjalos.github.io/Reading-Notes/)
# Online Readings

## [EJS Partials](https://medium.com/@henslejoseph/ejs-partials-f6f102cb7433)

**EJS Partials**
* Partials - can reuse the same HTML across multiple views. Think of them as functions, make large websites easier to maintain as you don’t have to go and change a piece of text in every page it appears in. Instead, you define that reusable bundle of code in a file and include it wherever you need it.
* When making a partial, create a ejs file that will contain only HTML for the partail you are defining, and now you can use the partails in your other ejs templates. 
  - In EJS, any JavaScript or non-HTML syntax you include in your templates is always surrounded by <% %> delimiters. Use this for a partial in EJS, which is where the partial file is relative to the template you use it in: <%- include( PARTIAL_FILE ) %>
  - The <%- %> tags allow us to output the unescaped content onto the page (notice the -). This is important when using the include() statement since you don’t want EJS to escape your HTML characters like ‘<’, ‘>’, etc…
* Next create the homepage template and include the partial you created in it.

## [Watch EJS tutorial from WalkThroughCode on YouTube, Video 7, Partials](https://www.youtube.com/watch?v=3_xEEH4fTEk&t=0s&index=7&list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt)

**Video Notes**
* Video Notes
  - Partials are native to EJS
  - Use case for partials would be a nav bar or footer that remains static
  - Go to layout.ejs and within the body tag put another body tag that's for the partial <%- body %>, and underneath it put <%- include('partial/onepartial')%>
  - Then create a new file for the parial/onepartail.ejs. In that new file make a header with a sentence in it and put nodemon in the terminal to see if the partail works. After you put in nodemon, refresh the web page to see what you wrote in the header.
  - This is how you set up a partail.