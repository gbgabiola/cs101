# Week 1

## Table of Contents <!-- omit in toc -->

- [Introduction](#introduction)
- [Code Writing](#code-writing)
- [Code Variables](#code-variables)
- [Digital Images](#digital-images)
- [Image Code](#image-code)


## Introduction

- **Fundamental Equation of Computers**
  > fundament equation of computer is: Computer = Powerful + Stupid
  - **Powerful**
    - look through large amounts of data quickly
    - can literally perform billions of _operations_ per second
  - **Stupid**
    - operations are simple and mechanical
    - nothing like a human _insight_ or _understanding_
    - a typical operation in the language of computers is adding two numbers together
    - stupid, but very useful
    - in movies - the mechanical stupidity of computers is missing
  like [HAL 9000](http://www.youtube.com/watch?v=HwBmPiOmEGQ#t=31s) from the movie 2001: A Space Odyssey
  - we should not be intimidated by the computer as if it's some sort of brain
    - computer is a mechanical tool which can do amazing things, but it requires a human to tell it what to do
- **High Level**
  - computer is driven by _code_ instructions
  - simple instructions, mechanical, e.g., add 2 numbers
  - computer _runs_ a long series of instructions, purely mechanical
- **Computers are very useful**
  - messaging, email
  - MP3 audio
  - red-eye reduction
  - and much more
- **Programmers**
  - make use the power of computer
  - thinks of a useful feature
  - thinks through the solution
  - algorithm - steps to accomplish
  - breaking it down to a simple instruction
  - dumbing it down for the computer


## Code Writing

**Code** refers to the language the computer can understand

- **Before Coding - Patience**
  - start with some simple coding
  - Code is like lego bricks...
  - individual pieces are super simple
  - eventually build up great combinations
  - but we have to start small
- **Javascript Computer Langauge**
  - "JavaScript" is a popular computer language
  - CS101 coding: Javascript + some CS101 specific features
  - not the whole Javascript language, just bits
  - just enough code to experiment with key ideas
- **Print**
  - **Run** executes each line once, running from top to bottom
  - **`print`** is a function like a verb in the code
  - numbers within the parenthesis ( ... ) are passed in to the `print` function
  - multiple values separated by commas
  - **syntax** of the code is very limited and strict
    - a reflection of the inner, mechanical/dumb nature of the computer
  - **Note**: `print` is not a normal part of Javascript, just added it for CS101
- **Print String**
  - **string** is a sequence of letters written within quotes to be used as data within the code, e.g., `"hello"`
    - strings work with the `print` function, in addition to numbers
    - strings in the computer store text, such as urls or the text of paragraphs, etc.
  - **comment** begins with `//` and extends through the end of the line
    - a way to write notes about the code, ignored by the computer
  - Code vs. Data
    - Code = instructions that are Run
    - Data = passive numbers, strings, handled by the code
  - **Note**: comments can be used to temporarily remove a line of code, _commenting out_ the code, by placing `//` in the beginning
    > Thinking About Syntax and Errors (key message!)
    - **syntax** - code text structured for the computer
    - very common error - you type in code, with slight syntax problem
    - Professional programmers make that sort of _error_ or syntax error all the time
    - not a reflection of some author flaw
    - beginners can be derailed by syntax errors, thinking they are making some big error
    - fixing these little errors is a small, normal step


## Code Variables

- **variables** in code
  - **variable** is like a box that holds a value, e.g., `x = 7;`
  - stores the value 7 into the variable `x`
  - later `x` in the code retrieve the value from the box
  - `x` becomes a shorthand for 7 (whatever is in the box)
  - using `=` in this way is called _variable assignment_
- variables is CS101
  - assign a value into a variable once
  - then use that variable many times
  - a convenient shorthand in the code


## Digital Images

- **Digital Images**
  - digital images are everywhere
  - look natural, smooth
  - behind the scenes: lots of little numbers
- **Zoom In - Pixels**
  - zoom in 10x
  - image is made of _pixels_
  - each pixel: small, square, one color
  - perceive the whole scene, not tiny pixels
  - _megapixel_ is 1 million pixels
  - image 800 pixel wide, 600 pixels high image
    - multiply: 800 x 600 = 480,000 pixels = 0.48 megapixels
  - typical digital camera 5-20 megapixels
- **X/Y Grid of Pixels**
  - pixels are organized as a x/y grid
  - x=0, y=0 _origin_ **upper left corner** - aka (0, 0)
  - X grows going to the right
  - Y grows going down
  - just like typesetting a page of text
  - x=0, y=0 _origin_ at upper left - (0, 0)
  - x=1, y=0 neighbor to the right of origin - (1, 0)
  - x=0, y=1 neighbor below the origin - (0, 1)
- **Newton's Color Prism**
  - Newton's famous experiment
  - white light - broken up into pure colors, continuous
  - red, orange, yellow, green, blue, indigo, violet (ROY G BIV)
  - pure colors as a palette
  - run the experiment backwards to make white
- **RGB Color Scheme**
  - RGB - red/green/blue scheme
  - make any color by combining red/green/blue lights
  - there are other schemes, but RGB is very common
  - **Note**: mixing lights works differently from mixing paints
  - **Aside**: technically color is a 3-dimensional space
    - The Newton prism shows the _hue_ dimension
    - other dimensions are brightness and saturation (pastel)
- **RGB - Three Numbers**
  - make any color by combining red/green/blue light
  - each red/green/blue light is represented by a number 0-255
    - 255 = maximum brightness
    - 0 = turned off
  - any color can represented by three numbers
  - not just 0 and 255, intermediate values 12, 238, 39
    - e.g., r:250 g:10 b:240 - purple, or just say "250 10 240"
    - e.g., r:100 g:100 b:0 - dark yellow, or just say "100 100 10"
  - don't memorize all colors, just understand the basic RGB scheme
- **Image Diagram with RGB**
  - pixels in a grid, each with an x,y address
  - each pixel has 3 numbers to define its color
  - written as "red:6 green:250 blue:7", or just "6 250 7"
- **Theme: Digital Atomization**
  - complex whole - _atomized_
  - broken down into lots of little numbers
  - "Lots of little numbers" - the domain of the computer
  - visual change to the image image
  - phrase as changes to the numbers in the computer


## Image Code

- x.png
  - x.png - tiny example image (10 x 10)
  - PNG format, like JPG
- x.png code example
  - three line program
  - `image = new SimpleImage("x.png");` loads into variable
  - `image.setZoom(20);` - sets zoom option to 20 (10, 20, 30, ...)
  - `print(image);` prints image to the right
  - zoom: each pixel shown 20x size here

  ```js
  image = new SimpleImage("x.png");
  image.setZoom(20);
  print(image);
  ```

- `pixel.setRed(255)` example
  - `pixel = image.getPixel(0, 0);` - upper left pixel
  - `pixel.setRed(255);`  sets red value of that pixel

  ```js
  image = new SimpleImage("x.png");
  image.setZoom(20);

  pixel = image.getPixel(0, 0);
  pixel.setRed(255);

  print(image);
  ```

- **Pixel Set Red/Green/Blue Functions**
  - `pixel.setRed(number);` sets the red value of the pixel to be the given number (0..255)
  - `pixel.setGreen(number);` sets the green value
  - `pixel.setBlue(number);` sets the blue value
