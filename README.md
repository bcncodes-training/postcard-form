# postcard-form

Partiendo del html que se facilita construir el siguiente formulario:

![postal](https://imgur.com/BtKM9i1.png)

Add the above code into the body of your HTML.

Organizing your assetsSection
This is where the fun begins! Before we start coding, we need three additional assets:

The postcard background — download this image and save it in the same directory as your working HTML file.
A typewriter font: The "Secret Typewriter" font from fontsquirrel.com — download the TTF file into the same directory as above.
A handdrawn font: The "Journal" font from fontsquirrel.com — download the TTF file into the same directory as above.
Your fonts need some more processing before you start:

Go to the fontsquirrel Webfont Generator.
Using the form, upload both your font files and generate a webfont kit. Download the kit to your computer.
Unzip the provided zip file.
Inside the unzipped contents you will find two .woff files and two .woff2 files. Copy these four files into a directory called fonts, in the same directory as before. We are using two different files for each font to maximise browser compatibility; see our Web fonts article for a lot more information.
The CSSSection
Now we can dig into the CSS for the example. Add all the code blocks shown below inside the <style> element, one after another.

First, we prepare the ground by defining our @font-face rules, all the basics on the <body> element, and the <form> element:
Now we can position our elements, including the title and all the form elements:
  That's where we start working on the form elements themselves. First, let's ensure that the <label>s are given the right font:
  
  The text fields require some common rules. Simply put, we remove their borders and backgrounds, and redefine their padding and margin:
When one of these fields gains focus, we highlight them with a light grey, transparent, background. Note that it's important to add the outline property, in order to remove the default focus highlight added by some browsers:
<textarea> elements default to being rendered as a block element. The two important things here are the resize and overflow properties. Because our design is a fixed-size design, we will use the resize property to prevent users from resizing our multi-line text field. The overflow property is used to make the field render more consistently across browsers. Some browsers default to the value auto, while some default to the value scroll. In our case, it's better to be sure every one will use auto:
  The <button> element is really convenient with CSS; you can do whatever you want, even using pseudo-elements:
