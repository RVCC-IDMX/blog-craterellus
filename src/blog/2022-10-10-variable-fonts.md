---
title: Variable Fonts
author: Sarah Lopez
description: Everything about how to get started using variable fonts.
date: 2022-10-10T00:08:08.866Z
tags:
  - variablefonts
  - webdev
image: /assets/blog/markus-spiske-cz-s645zbho-unsplash.jpg
imageAlt: Typefaces of a font family on a computer screen.
---
Intro

Variable fonts are accepted by most major browsers, so now is as good a time as any to learn how to use them. They’re more convenient, take up less space, and give you more control over your design. As a web developer, you have everything to gain from utilizing variable fonts in your designs. If you’d like to know how to use variable fonts in your projects, read on!

What is a variable font?

A variable font is similar to a static font in that it can have attributes like bold, italic, oblique, etc. Where they differ, though, is in how they’re implemented. You’re able to change the font’s appearance on a sliding scale. It’s kind of like the difference between an SVG and a bitmap image. The browser does the math to generate the image that you see.
For instance, you may be accustomed to using the font-weight property in CSS with static fonts. With this property, you’re able to adjust your font’s weight in 9 different levels. With a variable font like Roboto Serif, you’re able to adjust your font’s weight in 800 levels—basically any number from 100 to 900.

Why should I use one (instead of a static font)?

A big reason why it’s good to choose variable fonts is that they take up way less space. Traditionally, if you wanted different typefaces from the same font family, you’d have to import them as different files. For example: A font’s “thin” version and “light italic“ version are two different files. When it comes to variable fonts, there is pretty much one file for everything. You’re able to access a wide range of styles and do a whole lot more with a relatively small amount of space.

Finding a Variable Font

There are a huge number of both static and variable fonts that you can use in your projects for free on Google Fonts. Check it out! (INSERT LINK)
When you browse Google Fonts, there is a little checkbox just under the search bar that says: “Show only variable fonts”. Make sure that’s checked!
(INSERT IMG)
When you find a font that you like, you can download it and add it to the fonts folder in your own project. Generally, it’s a good idea to host a variable font locally while using it for a project.

Add a variable font to your project
(INSERT IMG)

In the example I’m using the font Roboto Serif. You can find it here. (INSERT LINK)
You can add the font to your project using the @font-face CSS rule. Here’s what it looks like:

(INSERT CODE)

Variable font axes
	So here’s the fun part. Now that you have the font hosted locally, you can start playing with it. Roboto Serif has five variable axes—Italic, (OPSZ), width, weight, GRAD, so there are an endless amount of possibilities.
And here they are in action!
This is some sample text. Hello!
This is some more sample text. Meow.
The cats are taking over. They know how to make sample text now. 
And there you have it! Just find a font, locally install it into your project, and you’re ready to go. Variable take up very little space for the amount of (use? Work?) you get out of them. It’s simple and (better) to use them, so go nuts!

(INSERT ADDITIONAL READING)



Photo by <a href="https://unsplash.com/@markusspiske?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Markus Spiske</a> on <a href="https://unsplash.com/?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>