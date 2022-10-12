---
title: Variable Fonts for Beginners
author: Sarah Lopez
description: If you don't know anything about Variable Fonts, this is the article for you!
date: 2022-10-10T00:08:08.866Z
tags:
  - variablefonts
  - webdev
image: /assets/blog/markus-spiske-cz-s645zbho-unsplash.jpg
imageAlt: Typefaces of a font family on a computer screen.
---
Photo by <a href="https://unsplash.com/@markusspiske?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Markus Spiske</a> on <a href="https://unsplash.com/?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>

Variable fonts are accepted by most major browsers, so now is as good a time as any to learn how to use them. They’re more convenient, take up less space, and give you more control over your design. As a web developer, you have everything to gain from utilizing variable fonts in your designs. If you’d like to know how to use variable fonts in your projects, read on!

## What is a Variable Font?

A variable font is similar to a static font in that it can have attributes like bold, italic, oblique, etc. Where they differ, though, is in how they’re implemented. You’re able to change the font’s appearance on a sliding scale. It’s kind of like the difference between an SVG and a bitmap image. The browser does the math to generate the image that you see.
For instance, you may be accustomed to using the font-weight property in CSS with static fonts. With this property, you’re able to adjust your font’s weight in 9 different levels. With a variable font like Roboto Serif, you’re able to adjust your font’s weight in 800 levels—basically any number from 100 to 900.

## Smaller and Faster

A big reason why it’s good to choose variable fonts is that they take up way less space. Traditionally, if you wanted different typefaces from the same font family, you’d have to import them as different files. For example: A font’s “thin” version and “light italic“ version are two different files. When it comes to variable fonts, there is pretty much one file for everything. You’re able to access a wide range of styles and do a whole lot more with a relatively small amount of space.

## Finding a Variable Font

There are a huge number of both static and variable fonts that you can use in your projects for free on Google Fonts. [Check it out here!](https://fonts.google.com/about)

When you browse Google Fonts, there is a little checkbox just under the search bar that says: “Show only variable fonts”. Make sure that’s checked!

![A checkbox checked with text to the right of it that says "Show only variable fonts"](/assets/blog/variable-fonts-02.png)

When you find a font that you like, you can download it and add it to the fonts folder in your own project. Generally, it’s a good idea to host a variable font locally while using it for a project.

## Add a Variable Font to Your Project

You can add the font to your project using the @font-face CSS rule. Here’s what it looks like:

```css
@font-face {
  font-family: 'Roboto';
  font-style: normal;
  font-weight: 100 900;
  src: url('/fonts/RobotoSerif-VariableFont_GRAD\,opsz\,wdth\,wght.ttf') format('truetype');
}
```

In the above example I'm using Roboto Serif. Note how in the url I'm linking to my project's font folder.

## Variable Font Axes

So here’s the fun part. Now that you have the font hosted locally, you can start playing with it. Roboto Serif has five variable axes—italic, optical size, width, weight and grade, so there are an endless amount of possibilities. Different variable fonts will have different axes, so pay attention to what your font offers.

And here they are in action!

![An screenshot of a simple web page with two headings and a paragraph. They all use the same font but look very different.](/assets/blog/variable-fonts-03.png)

Here is the code that made this happen:

```css
body {
font-family: 'Roboto', serif;
}

h1 {
    font-size: 3.6rem;
    line-height: 1em;
    letter-spacing: -0.04em;
    font-style: italic;
    font-variation-settings: 'GRAD' 14, 'opsz' 144, 'wdth' 102, 'wght' 880;
  }

h2 {
    font-size: 2.1rem;
    line-height: 1em;
    letter-spacing: 0.3em;
    font-variation-settings: 'GRAD' -50, 'opsz' 95, 'wdth' 136, 'wght' 450;
    
  }

p {
    font-size: 1.5rem;
    line-height: 1.7rem;
    letter-spacing: 0.01em;
    font-style: italic;
    font-variation-settings: 'GRAD' -17, 'opsz' 132, 'wdth' 53.5, 'wght' 112;
  }
```

  Note that the axes are all in single quotes and are all given values in the font-variation-settings property.

## Summary

And there you have it! Just find a font, locally install it into your project, and you’re ready to go. Variable fonts take up very little space for the amount of mileage you get out of them. They're simple to use too, so the (typography?) world is basically your oyster.

## Additional Reading

https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Fonts/Variable_Fonts_Guide
https://variablefonts.io/implementing-variable-fonts/
https://web.dev/variable-fonts/