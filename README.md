
#Boardz.css

![Boardz.css](http://i67.tinypic.com/2ib27oz.jpg)

Boardz.css is a simple CSS library that allows to create Pinterest-like card-boards from simple unordered lists with less than 1kB minified file size. [Live demo here.](https://karakanb.github.io/boardz/)

##What is Boardz?
Boardz is a simple, lightweight and responsive pure CSS library that creates Pinterest-like boards from simple unordered list elements. The main objective of the Boardz is to give the basic layout of the board with a simple default styling. The library is not made to be a plug-and-use file, it simply gives the layout of the board to the nested `<ul>` and `<li>` elements. It uses the powerful Flexbox model to create and maintain the layout across devices and screens. 

![Layout screenshot](http://i63.tinypic.com/53mu8i.jpg)

##How to use it?
In order to use Boardz, just wrap your unordered list with a div of class `boardz`, then the rest of the list will be styled properly. Think of every unordered list as a column in the board, and the columns will be generated for every unordered list element in your div. Boards will also give a basic style to the h1 headers in your list elements. The basic structure of a simple board with 2 columns is as follows:
```HTML
<div class="boardz">
    <!-- First column -->
    <ul>
        <li>
            <h1> Header 1</h1>
            Content
        </li>
        <li>
            <h1> Header 2</h1>
            Content
        </li>
    </ul>

    <!-- Second column -->
    <ul>
        <li>
            <h1> Header 1</h1>
            Content
        </li>
        <li>
            <h1> Header 2</h1>
            Content
        </li>
    </ul>
</div>
```
----------

##Available Classes
There are three main classes that can be given to a **Boardz** element. The `boardz` class is necessary on the wrapper `div`, and the other two are optional. Note that, all of these classes should be used on the wrapper div, e.g. `<div class="boardz beautiful">`.

`boardz`: This is the class that needs to be on the wrapper div.
`fitted`: This is the class to make columns justified vertically.
`beautiful`: This is the class to make stylish cells.

##Why does it exist?
We are trying to build more interactive and fancy interfaces everyday, and the web pages are getting bigger and bigger in terms of file sizes. I like simple interfaces with clear intentions and because of this, usually, I am trying to use small libraries wherever possible. A few days ago, I read [the great Medium article of Ohans Emmanuel on CSS Flexbox](https://medium.freecodecamp.com/understanding-flexbox-everything-you-need-to-know-b4013d4dc9af) and decided to implement a simple Pinterest-like card-board library by using pure CSS and Flexbox, which I was thinking of using for a new project, while keeping the file size at minimum. Turns out that Flexbox makes things incredibly simple and is a nice step for building more responsive web pages. 

-----

Boardz is highly customizable and a simple solution with less than 1kB minified file size. It may set a base for anyone to create more specialized card-boards, or it may not, I don't know. The project is completely open-source, so you can submit a PR whenever you want. Anyway, if you found anything wrong with it, or if you have any suggestions, please feel free to contact me.

##License
The project is licensed under MIT License.