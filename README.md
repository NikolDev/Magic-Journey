<h1 align='center'>Magic-Journey©</h1>
<h4 align='left'>💻 This is not a large part of the front-end, in which the main menu of the site is presented. Animation works on the navigation menu, and the "Login" button also works, where the login and registration window appears with a slight animation. The code is protected by copyright.</h4>
<img src='/image_2023-08-03_21-59-06.png' alt='screenshot'>

<h4 align='right'>This pseudo site is written according to the modern semantics of html and css. This pet project is great for a beginner front-end developer to get familiar with styles and get into basic JavaScript coding. Below I will provide a little documentation on the code.</h4>

<h3 align='left'><b>So, what do you need to know to write this project yourself?</b></h3>
<kbd>HTML</kbd> + <kbd>CSS</kbd> + <kbd>JavaScript</kbd> + <kbd>Practice</kbd> + <kbd>Time</kbd>
<p>Of course, the most important thing is to know the basics of html & css. In JavaScript, you must be aware of functions, inputs, and methods. After that, you can safely start writing your project! Let's get to the documentation.</p>

<h3>HTML document:</h3>
<p>I will not go deep here. I just mark up the page with all the text and define my classes using modern HTML 5 semantics</p>

<h3>CSS document:</h3>
<p><b>1. We immediately connect our Google font</b></p>

```css
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800;900&display=swap');
```

<p><b>2. Next, set the global file settings and include the font</b></p>

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}
```

<p><b>3. After we style the header by setting a fixed position, setting the indents with padding and using the display flex we use the justify content together with the align item</b></p>

```css
header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  padding: 20px 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  z-index: 99;
}
```

<p><b>4. Styling the name company</b></p>

```css
.logo {
  font-size: 2em; /*set font size*/
  color: #fff; /*set white color*/
  user-select: none; /*set user-select in meaning none, this is determines whether the user can select text.*/
}
```

<p><b>5. Next, style the navigation buttons relative to the links.</b></p>

```css
.navigation a {
    position: relative; /*set relarive position*/
    font-size: 1.1em;  /*set font size*/
    color: #fff;  /*set white color*/
    text-decoration: none;  /*Using text-decoration in meaning none i remove the underlining of links*/
    font-weight: 500;  /*set weight text*/
    margin-left: 40px;   /*set margin indent in left*/
}
```

<p><b>6. Moving on</b></p>

```css
.navigation a::after { /*creates a pseudo-element that is the last child of the selected element.*/
    content: ''; /*set none content*/
    position: absolute;
    left: 0;
    bottom: -6px;    /*set indent bottom in -6px*/
    width: 100%;  /*set width in 100%*/
    height: 3px;
    background: #fff;  /*set background color white*/
    border-radius: 5px; /*set window rounding*/
    transform-origin: right; /*The transform-origin property allows you to change the position of transformed elements.*/
    transform: scaleX(0);  /*set scale 0px*/
    transition: transform .5s; /*set time animation*/
}
```
<p><b>Summing up CSS file:</b></p>
<p>This is a small part of the css file documentation. Why didn't I do more? It's simple, try to figure out the rest of the file yourself. I told you the main points, good luck!</p>

- [x] Task 1: Learn the basics of html & css, javascript
- [ ] Task 2: Show stranger code
- [ ] Task 3: More practice

<pre>
.GitHub {
  hints-one: <a href='https://devdocs.io/css/'><b>CSS Documentation</b></a>;
  hints-two: <a href='https://devdocs.io/html/'><b>HTML Documentation</b></a>;
  hints-three: <a href='https://devdocs.io/javascript/'><b>JavaScript Documentation</b></a>;

  practice-frontend-skills:
}
</pre>


<h3>JavaScript document:</h3>
<p><b>1. Well, the last thing for today, deal with JavaScript</b></p>
<p>- In the first 5 lines of code, we set the constants by referring to the selector, writing their names.</p>

```javascript
const wrapper = document.querySelector('.wrapper');
const loginLink = document.querySelector('.login-link');
const registerLink = document.querySelector('.register-link');
const btnPopup = document.querySelector('.btnLogin-popup');
const iconClose = document.querySelector('.icon-close');
``` 

<p>- Well, then we create a function and write the addEventListener method, which takes a click as input and, based on this, they either add or remove the window.</p>

```javascript
registerLink.addEventListener('click', ()=> {
  wrapper.classList.add('active');
});

loginLink.addEventListener('click', ()=> {
  wrapper.classList.remove('active');
});

btnPopup.addEventListener('click', ()=> {
  wrapper.classList.add('active-popup');
});

iconClose.addEventListener('click', ()=> {
  wrapper.classList.remove('active-popup');
});
```

<h3>Result</h3>
Above, I very briefly explained how my code works, how it interacts and how it is connected. I hope you liked my small project, I hope for support. Pull requests are welcome)
