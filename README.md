# modulo-framework
Mini framework for css modules

#### What is Modulo?
Modulo aims to provide a set of modular, simple, semantic and infinitely nestable components for small projects where you don't need the bloat of Bootstrap or similar libraries, but don't want to reinvent the wheel every time either.
Currently, Modulo is entirely CSS but will be extended with plain JS components when I find the time.

See this general, ridiculously nested fiddle to quicky see the abilities of the library:  
http://jsfiddle.net/gh/get/library/pure/Radiergummi/modulo-framework/tree/master/Demo


###How to use it?
To work with the modules provided by Modulo, first include the main stylesheet modulo.lib.css. You should now be able to create simple components like those in the wiki. Currently they bring minimal default styling but that will be moved into optional themes later on.  
To fill the modules with explanatory example content, add the class ´modulo-demo´ to your document body (Note: This feature is not included in the minified CSS file modulo.lib.min.css, as it is merely there to understand how everything works).  

Let's assume you want to build a modal window, so you append the following HTML to your document:

```html
<div class="modal">
  <!-- content here -->
</div>
```

The modal appears upon reload (if not, put that IE back into it's grave!) and is positioned in the window center. To add any styling to it, position it elsewhere or address it with JS, you should definitely add an own class or id, maybe like this:  

```html
<div class="modal social" id="#gplus">
  <!-- content here -->
</div>
```

Now you could add styles for all social network sharing dialogs and use simple JS to work with this one in particular (`document.getElementById('#gplus')`).  
Please refrain from hacking the base code and use additional identifiers! That helps building clean code with containers and content separated.  
