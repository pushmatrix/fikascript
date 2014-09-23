[FikaScript](http://fikascript.se)
==========
![Swedish Flag](/assets/img/flag.png)  
FikaScript lets you write JavaScript in Swedish; Finally there is a way for Swedes to code in their native language!
It is named after [fika](http://en.wikipedia.org/wiki/Fika_(coffee_break)), the sacred Swedish coffee break.

See it in action [here](http://fikascript.se). 
### Including FikaScript files in your HTML

- Include [fikascript.js](dist/fikascript.js) and [fikascript.browser.js](dist/fikascript.browser.js).
- Make sure your html is set to allow utf-8 characters (add `<meta charset="utf-8">` in the <head>).

FikaScript supports the `text/fikascript` MIME type. Any script tag with that type will be compiled and run automatically:
```html
<script type="text/fikascript">
  om (x < 5) {
    konsol.log("hej!");
  } annars {
    konsol.log("nej!");
  }
</script>
```

You can also specify a `src` for your script tags: 
```html
<script type="text/fikascript" src="snaps.fika"></script>
```

#### Optional

##### Convert from FikaScript to JavaScript:

```javascript
FikaScript.swedishToEnglish(code); // returns a string representing the translated code
```

##### Convert from JavaScript to FikaScript:

```javascript
FikaScript.englishToSwedish(code); // returns a string representing the translated code
```

### Missing/incorrect translations?
You can see the translations over [here](https://github.com/pushmatrix/fikascript/blob/gh-pages/dist/fikascript.js#L4). Feel free to submit a pull request!

###TO-DOs
- Syntax highlighting for unicode chars
- npm support for command line compiling
- Add more translations!!! (ex: Array.pop, push, etc...)
