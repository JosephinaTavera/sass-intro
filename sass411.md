# Sass

## Learning Objectives

- Be able to explain what Sass is and why it's used
- Use variables to make code more flexible
- Understand how to use nesting to help DRY up selectors and properties
- Differentiate between `@extend`, `@import`, `@mixin` & `@include`, and `@function`

## Framing: What is Sass? (5 minutes / 1:30)

![Sass Icon](http://sass-lang.com/assets/img/logos/logo-b6e1ef6e.svg)


### CSS 

Stylesheets can be repetitive. Colors, properties, etc. 

Imagine having to change a color, and it needs to be done in several locations of a large CSS file.  

CSS is anything but DRY. 

Fortunately, there are options to help us out here, and one of them is Sass.

---

### Syntactically Awesome Stylesheets

Sass is a superset of CSS that adds power and elegance to the basic language. You can do all the normal CSS things plus way more!
- You write a combination of CSS and SassScript, which compiles to proper CSS.
- It allows you to use variables, nested rules, mixins, inline imports and more, all with a fully CSS-compatible syntax.
- Sass helps keep large stylesheets well-organized, and helps get small stylesheets up and running quickly...


## You Do: Teachbacks (35 minutes / 2:20)
> 20 minutes exercise. 15 minutes presentations.

Now that we have a case for using SASS, let's get into groups and learn more about it. 

Deliverables
* Create one lesson plan repo for all the concepts your group has been assigned. Use this markdown cheatsheet to help format your readme.md files: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
* Answer questions provided to each group 
* For each concept, provide two demos showcasing the SASS.
* Create one example of how the feature would have been implemented in Vanilla CSS.
* Present your group's findings to the class. Be prepared to talk about the concepts and demonstrate your implementations. Each group will have 10 minutes to present. Plan to have three minutes at the end for questions. All group members must speak.

Group 1

### I. Variables

#### Questions

* What are Sass variables? What problem do they solve?
* How do you define a variable?
* What values can you store in a variable?
* What are some common use cases?
* How does scope work with Sass variables?

#### Resources

* [Sass Documentation](http://sass-lang.com/guide)
* [Sass Variables](https://robots.thoughtbot.com/sass-variables)
* [Getting Started with Sass](http://alistapart.com/article/getting-started-with-sass)

Group 2 

### II. Nesting

#### Questions

* What does "nesting" mean in Sass? What problem does it solve?
* What does `&` mean?
* What's the difference between selector nesting and property nesting? Show examples of each.
* How much nesting is too much nesting?

#### Resources

* [Sass Documentation](http://sass-lang.com/guide)
* [The Inception Rule](http://thesassway.com/beginner/the-inception-rule)


Group 3
### III. Extends & Inheritance

#### Questions

* What is Sass inheritance? What problem does it solve?
* How do we use `@extend` to implement inheritance?
* What does an `@extend` example look like when compiled to vanilla CSS.
* What are some common use cases?

#### Resources

* [Sass Documentation](http://sass-lang.com/guide)
* [Extending In Sass Without A Mess](https://www.smashingmagazine.com/2015/05/extending-in-sass-without-mess/)
* [The Extend Concept](https://css-tricks.com/the-extend-concept/)

Group 4
### IV: Mixins

#### Questions

* What are mixins? What problem do they solve?
* How do we define and use a mixin?
* In what way might a mixin resemble a programming language?
* What is a common example of a mixin?

#### Resources

* [Sass Documentation](http://sass-lang.com/guide)
* [The Mixin Directive](https://www.sitepoint.com/sass-basics-the-mixin-directive/)
* [Handy Sass Mixins](https://web-design-weekly.com/2013/05/12/handy-sass-mixins/)
* [The Extend Concept](https://css-tricks.com/the-extend-concept/)

### BONUS  V: Functions

If you're group finishes early, look into Sass functions!

#### Resources

* [Sass Documentation](http://sass-lang.com/documentation/Sass/Script/Functions.html)
* [Pure Sass Functions](http://thesassway.com/advanced/pure-sass-functions)

## Break (10 minutes / 1:45)


### 
To quote the official Sass website:

Sass makes CSS fun again. Sass is an extension of CSS3, adding nested rules, variables, mixins, selector inheritance, and more. It’s translated to well-formatted, standard CSS using the command line tool or a web-framework plugin.



## You Do: Explore Sass Examples (10 min / 1:40)

Explore these Codepens. When you open them, you'll notice that the CSS column has a header of CSS (scss). This means that you're currently looking at Sass. Compare this to what you see when you click on the drop-down arrow at the top-right of the column and click "View Compiled CSS". Now you're looking at the CSS after it's been compiled from Sass.

Some things to consider...
* In what ways does Sass look different than Vanilla CSS?
* How might writing out Sass be easier / faster than writing out vanilla CSS?

#### Sass Examples

- [BAMSAY](http://codepen.io/jshawl/pen/cLJal)
- [Boxes](http://codepen.io/jshawl/pen/nHDLz)
- [Bullseye](http://codepen.io/jshawl/pen/wpeit)
- [A Button](http://codepen.io/jshawl/pen/bcjyH)
- [Forest](http://codepen.io/jshawl/pen/cJjIm)
- [Space Invader](http://codepen.io/jshawl/pen/cnyrJ)

> We don't expect you to understand exactly what the Sass is doing in these examples. Just think about it on a higher level.



## Compiling to CSS

Webpages don't know what to do with raw Sass/SCSS, these files need to be compiled to regular CSS to be used.

This can be done a number of different ways...
- Installing the sass gem `gem install sass` and compile with `$ sassc <whatever-input-filename.scss> <whatever-output-filename.css>`
  - There is also a `--watch` flag that allows you to watch a file and auto-compile every time you save it.
- Using a GUI program/plugin like `sass-autocompile`
  - `apm install sass-autocompile`
- Letting a build tool like Grunt/Gulp/Webpack/npm-scripts handle the compilation with an additional package/plugin.

------

### Libraries/Frameworks

There a good number of [libraries](http://www.hongkiat.com/blog/mixin-library-for-sass/) of mixins and functions that can extend the functionality of Sass. Most are used by `@import`ing the library `@include`ing the mixins where desired.

- [Bourbon](http://bourbon.io/) is "a simple and lightweight mixin library."
  - [Neat](http://neat.bourbon.io/) is "a lightweight semantic grid framework for Sass and Bourbon."


# Exercise: Flash (15 minutes)

> If there's time left, give this exercise a shot.

[Flash Exercise](http://codepen.io/adambray/pen/bEgMXr)

Use Sass to style the provided elements to recreate the image at bottom of the Codepen. You shouldn't need to modify the HTML at all.

Don't try to implement all the above Sass features at once. Instead, take the following steps...
* Complete the exercise, making sure to use variables for repeated values and nesting selectors where applicable.
* Once you're done, identify repeated chunks of code and define them in single selectors. Then apply them throughout your code using `@extend` statements.
* **BONUS:** Use mixins and/or functions to to generate the font and background colors for each button.

<details>
  <summary>
	 **SOLUTION:**
  </summary>
  [Only take a peek. No copy-and-pasting.](http://codepen.io/adambray/pen/yegjdj)
</details>

# Conclusion

- Name 3 benefits of Sass.
- Describe how variables work in Sass
- Understand how to use nesting to help DRY up selectors and properties
- Differentiate between `@extend`, `@import`, `@mixin` & `@include`, and `@function`

### Want more?  

- [Super cool custom framework](http://www.sassmeister.com/gist/0a041d0fb2d72758c280)
  - From the scotch.io tutoral - [build your own framework](https://scotch.io/tutorials/getting-started-with-sass#function-directives)
]
- Or, check out the follow-up lesson, [Sass Directives](https://github.com/ga-wdi-lessons/sass-directives)

### References

Guides:
- [Official getting started guide](http://sass-lang.com/guide)
- [Scotch.io - Build your own framework](https://scotch.io/tutorials/getting-started-with-sass#function-directives)
- [TheSassWay - Pure sass functions](http://thesassway.com/advanced/pure-sass-functions)
- [Sitepoint - Function basics](https://www.sitepoint.com/sass-basics-function-directive/)
- [Sitepoint - Control directives](https://www.sitepoint.com/sass-basics-control-directives-expressions/)
- [Docs for functions](http://sass-lang.com/documentation/Sass/Script/Functions.html)

Examples:
- [3D Buttons with Sass](https://jesse.sh/makes-3d-buttons-with-sass/)
- Github's Style Guide, [Primer CSS](http://primercss.io/about/)
