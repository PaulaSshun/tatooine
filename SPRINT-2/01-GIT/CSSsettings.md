# CSS: Cascading Style Sheet
**CSS** is a language that describes the style of an **HTML** document.  
**CSS** describes how HTML elements should be displayed, with a lot of elements to use for a good view in the document.
This short tutorial will explain it.

![Css](https://2r4s9p1yi1fa2jd7j43zph8r-wpengine.netdna-ssl.com/files/2017/08/04.png)

First of all, to make a **css** document we have to make a file name extension in our **html** document, that's because if we don't vinculate the html and css codes, our html file will don't ubicate the CSS code and the style will doesn't work .

We can use **< link>** to vinculate files html and css together.  
The **< link>** must be placed within the *header* of the HTML file.  
This **< link>** have three atributes:  
- **href:** like the anchor element, the value of this attribute must be the address, or path, to the CSS file.  
The href attribute specifies the location (URL) of the external resource (most often a style sheet file).
- **type:** describe the kind of the document that you are linking (in this case is css). The value is *text/css*.  
- **rel:** This is the relationship between the HTML file and CSS file. Because you are linking to a stylesheet, the value should be to *stylesheet*.  

When linking an HTML file and CSS file together, the **< link>** element will look like this:    
*An absolute URL - points to another web site (like href="http://www.example.com/theme.css").  
A relative URL - points to a file within a web site (like href="/themes/theme.css").*
~~~
<link href="http://www.example.com/theme.css"
  type= "text/css" rel="stylesheet"/>
~~~
#### CSS Rule Structure  

![structure css](http://gottheknack.com/a_htmlCss/weeks/week8/cssRuleStructure/images/ruleParts.gif)

#### Tag name
CSS can select HTML elements by using an element's tag name. A tag name is the word (or character) between HTML angle brackets.
For example, in HTML, the tag for paragraph element is **< p>**. The CSS syntax for selecting < p> element is:   
`p {
  }`  
In the example above, all the paragraph elements will be selected using a CSS *selector*. The selector in the example above is **p**.

#### Class Name
CSS is not limited to selecting elements by tag name. HTML elements can have more than just a tag name; they can also have *attributes*. One common attribute is the **class** attribute. It's also possible to select an element by its **class** attribute  
For example:  
~~~
<p class="brand">Paula Company AC</p>
~~~  
The paragraph element in the example above has a **class** atribute within the < p> tag. The **class** attribute is set to **"brand"**. To select this element using CSS, we could use the following CSS selector:  
`.brand {
  }`

#### Multiple class
We can add multiple class to the atribute class of a HTML element with a space.  
For example:
~~~
HTML:
< h1 class="green bold">Hola Paula< /h1>

CSS:
.green {color: green;}
.bold {font-weight:bold;}
~~~
#### ID name
If a HTML element need a unique style, we can add a ID to the element. To add an ID to the element, we need an atribute of ID.
~~~
HTML:
<h1 id="large Title">...</h1>

CSS:
#large-Title {
}
~~~

#### Font Family
This element we use for change the font text in the file. We don't should use too much font size. When the name of some font have two words we use "".
~~~
h1 {
    font-family: "Courrier new";
}
~~~
#### Font size
This element change the size of the font. We use in pixel
~~~
p {
  font-size: 18px;
}
~~~
#### Font weight
In CSS, the font-wight property controls how bold or thin text appears.
~~~
p {
  font-size: 18px;
}
~~~
#### Text align
Our text for default appears left side, so with this property can modificative how it can looks. This have 3 attributes:
- **Right**
- **Left**
- **Center**

~~~
h1 {
    text-align: right;
}
~~~
#### Color
There are two kind: **Foreground** and **Background**.  
- **Foreground**: This is the element color.
- **Background**: The Background color.
- **Color**: This propriety use the color element.
- **Background-color**: Show the Background color of an element.  
~~~
h1 {
   Color: red;
   background-color: blue;
}
~~~

#### Background image
CSS has the ability to change the background of an element. One option is to make the background of an element an image.
The value provided to **background-image** is a url. The url should be a url to an image. The **url** can be a file within your project, or it can be a link to an external site.
~~~
.main {
    background-image: url("www.example.com");
}
.main { background-image: url("our file.jpg")
}
~~~

#### Box model

![Box model](https://coursework.vschool.io/content/images/2016/08/boxmodel.gif)

1. **Width & height**: is the amount of space the content of the element itself takes up. How much space your actual body takes up.
2. **Padding**: it's about the additional space that you occupy to the amount space. If theres no padding, it will be like you don't have space between your body and your clothes. So as the padding increases, the elements get larger and larger. The text by itself determines the height and the widht of the element, but if we want to extend the size of the element (even the amount of space for the background color), we can use *padding*.
 - **Padding-top**
 - **Padding-right**
 - **Padding-left**
 - **Padding-bottom**  
3. **Border**: it represents the separation between the element itself and any other elements that may be nearby of another element. Some of the most common properties we change are: *widht*, *style*, *color*, *radius*.      
 - **Widht**: is the thickness of the border itself. It colud be *px*, *thir*, *medium*, *thick*.
 - **Style**: is the patter of the border. There are a lot of options, example: *none*, *dotted*, *solid*.
 - **Color**: is the color of the border. You can use some kind of color using a different ways.
 - **Radius**: you can create a border that it could be a perfect circle with the element 'radius' using *100%*. Is the roundness of the corners of the border.  
4. **Margin**: specifies the space between the inner border and the outside border of the element. The greater the margin, the more space between each border.
 - **Margin-top**
 - **Margin-right**
 - **Margin-left**
 - **Margin-bottom**

![box model](https://librosweb.es/img/css/f0403.gif)

`Paula Sshun 2018 ® `
