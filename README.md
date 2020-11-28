# JournalingMyLearning_CSS

When I started learning web development I asked to the Bootcamp's teacher: 
"What was the best to use in css - px, rem or em?". 
He replied: 
"Just pick one and stick with it." 
FYI he didn't have a clue what was rem or em. 

Is what I did since then, I used just pixels on my projects. It worked and was realiable until I started to understand a bit more about accessibility or responsive design. I noticed that I couldn't figure out why the h1 heading didn't change on the small screens...which was very annoying. So I did what the web developers professionals do most on their daily job:

Research, googling, experimenting until I found my answers.

This article will go deep on pixels and accessibility and explain in details about px, rem and em. I hope you will enjoy it: 

https://www.24a11y.com/2019/pixels-vs-relative-units-in-css-why-its-still-a-big-deal/




/************************************************************************************/
Custom properties/variables  
:root {
  --main-xxxx: #------;
  --main-xxxx: #------;
  --main-xxx: #-----;
  --main-xxxx: #-----;
}

/* Base reset */
* {
  margin: 0;
  padding: 0;
}

/* box-sizing and font sizing */
*,
*::before,
*::after {
  box-sizing: inherit;
}

html {
  box-sizing: border-box;

  /* Set font size for easy rem calculations
   * default document font size = 16px, 1rem = 16px, 100% = 16px
   * (100% / 16px) * 10 = 62.5%, 1rem = 10px, 62.5% = 10px
  */
  font-size: 62.5%;
  scroll-behavior: smooth;
}

