# Magic-Journey©
<h4 align='left'>💻 This is not a large part of the front-end, in which the main menu of the site is presented. Animation works on the navigation menu, and the "Login" button also works, where the login and registration window appears with a slight animation. The code is protected by copyright.</h4>
<img src='/image_2023-08-03_21-59-06.png' alt='screenshot'>

<h3>This pseudo site is written according to the modern semantics of html and css. This pet project is great for a beginner front-end developer to get familiar with styles and get into basic JavaScript coding. Below I will provide a little documentation on the code.</h3>

<h3>HTML document:</h3>
<p>I will not go deep here. I just mark up the page with all the text and define my classes using modern HTML 5 semantics</p>

<h3>CSS document:</h3>
<p><b>1. We immediately connect our Google font</b></p>
<pre>
  1. @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800;900&display=swap');
</pre>

<p><b>2. Next, set the global file settings and include the font</b></p>
<pre>
  3.  * {
  4.    margin: 0;
  5.    padding: 0;
  6.    box-sizing: border-box;
  7.    font-family: 'Poppins', sans-serif;
  8.  }
</pre>

<p><b>3. After we style the header by setting a fixed position, setting the indents with padding and using the display flex we use the justify content together with the align item</b></p>
<pre>
  19.  header {
  20.    position: fixed;
  21.    top: 0;
  22.    left: 0;
  23.    width: 100%;
  24.    padding: 20px 100px;
  25.    display: flex;
  26.    justify-content: space-between;
  27.    align-items: center;
  28.    z-index: 99;
  29.  }
</pre>

<p><b>4. Well, then comes the usual styling of classes and animations</b></p>

<h3>JavaScript document:</h3>
<p><b>1. Well, the last thing for today, deal with JavaScript</b></p>
<p>- In the first 5 lines of code, we set the constants by referring to the selector, writing their names.</p>
<pre>
  1.  const wrapper = document.querySelector('.wrapper');
  2.  const loginLink = document.querySelector('.login-link');
  3.  const registerLink = document.querySelector('.register-link');
  4.  const btnPopup = document.querySelector('.btnLogin-popup');
  5.  const iconClose = document.querySelector('.icon-close');
</pre> 

<p>- Well, then we create a function and write the addEventListener method, which takes a click as input and, based on this, they either add or remove the window.</p>
<pre>
  6.  
  7.  registerLink.addEventListener('click', ()=> {
  8.      wrapper.classList.add('active');
  9.  });
  10.  
  11.  loginLink.addEventListener('click', ()=> {
  12.      wrapper.classList.remove('active');
  13.  });
  14.  
  15.  btnPopup.addEventListener('click', ()=> {
  16.      wrapper.classList.add('active-popup');
  17.  });
  18.  
  19.  iconClose.addEventListener('click', ()=> {
  20.      wrapper.classList.remove('active-popup');
  21.  });
</pre>

<h3>Result</h3>
Above, I very briefly explained how my code works, how it interacts and how it is connected. I hope you liked my small project, I hope for support. Pull requests are welcome)
