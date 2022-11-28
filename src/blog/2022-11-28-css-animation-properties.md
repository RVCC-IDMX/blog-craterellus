---
title: CSS Animation Properties
author: Sarah
description: A deep dive into every CSS Animation property. Learn how to
  fine-tune your CSS animations to perfection!
date: 2022-11-28T00:06:37.702Z
tags:
  - post
  - css
  - animation
  - ""
image: /assets/blog/animation-article-img.jpg
imageAlt: A blurry view of a person walking mid stride.
---
# Animation Properties: What are they?
CSS Animations are easy to use, fun to make, and they can make your pages come alive. There are a bunch of ways to customize and alter your animations by using animation properties. With these tools at your disposal, you'll be able to have complete control over your animation work.

Did you know that the animation property itself is shorthand for pretty much all the individual animation properties? It combines multiple properties into a convenient one-stop-shop. The animation shorthand property takes the values of animation-duration, animation-timing-function, animation-delay, animation-iteration-count, animation-direction, animation-fill-mode, animation-play-state, and animation-name. 

We'll be going into more detail for each property below. In order to demonstrate some of these properties in action, I'll be throwing this here apple around. Hope you don't mind!

<p class="codepen" data-height="500" data-default-tab="html,result" data-slug-hash="dyKZZpx" data-user="craterellus" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/craterellus/pen/dyKZZpx">
  Apple</a> by Sarah Lopez (<a href="https://codepen.io/craterellus">@craterellus</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

## animation-name

Use this property to give your animation a name. You’ll be using this name to refer to your animation in the @keyframes CSS rule. In the example above, I gave my animation the name applespin.

## animation-duration
You can probably guess what this one does. This sets the time it takes for your animation to iterate through one cycle. The accepted units are seconds or milliseconds. You can use multiple values separated by a comma. These values will apply to the animation in the order that you specify.
Also, this property does not accept negative values.

## animation-timing-function

Animation-timing-function can add a more natural feel to your animations with values like ease-in or ease-out. With this property, you are able to determine whether or not you’d like your animation to accelerate or decelerate as it progresses. 
This property is very customizable. You can set the value to cubic-bezier() and map out a Bezier curve. This way, you’re able to control exactly when your animation slows or speeds up.

## animation-delay

With this property, your animation will start after a specified period of time. It can be in seconds or milliseconds. The default value for animation-delay is 0s. 
You can use a negative value with animation-delay. This will cause your animation to start in the middle of a cycle. For instance, if the value is set to -1s, the animation will start one second into its cycle.

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="vYrrbdX" data-user="craterellus" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/craterellus/pen/vYrrbdX">
  Apple-delay</a> by Sarah Lopez (<a href="https://codepen.io/craterellus">@craterellus</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

## animation-iteration-count

Use this property to specify how many times you’d like your animation to play. You can set the value to a positive number, or, if you’d like your animation to loop indefinitely, you can set the value to infinite. The default value of this property is 1.

## animation-direction

This property has full evergreen support. So, what does it do? It’s pretty straightforward. (Haha, get it?) With this property, you can specify the direction in which your animation plays. You can use this property to reverse your animation. So, for example, let’s say you have an animation of a person walking from one side of the screen to another. With animation-direction, you can make the person walk backwards. You can also set it to alternate, which loops between normal and reverse. The value alternate-reverse is very much the same, but...reverse!

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="GRGGzQW" data-user="craterellus" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/craterellus/pen/GRGGzQW">
  Apple-direction</a> by Sarah Lopez (<a href="https://codepen.io/craterellus">@craterellus</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

## animation-fill-mode

Animation-fill-mode is used for determining where the image you’re animating ends up at the end of its animation cycle.
This property is useful for animations that aren’t designed to loop seamlessly. Its functionality is somewhat more specific than that of the other properties. Let’s say you have an animation of an object that goes from point a to point b. When the animation is finished running, does the object stay at point b, or does it jump back to point a? This is what animation-fill-mode is for. It can be set to forwards, backwards, both, none, and inherit.
Here’s an example of this being used with our flying apple: 

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="gOKKqvW" data-user="craterellus" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/craterellus/pen/gOKKqvW">
  Apple-fill-mode-default</a> by Sarah Lopez (<a href="https://codepen.io/craterellus">@craterellus</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="qBKKgJO" data-user="craterellus" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/craterellus/pen/qBKKgJO">
  Apple-fill-mode-forwards</a> by Sarah Lopez (<a href="https://codepen.io/craterellus">@craterellus</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

## animation-play-state

With this property, you can pause your animation. This is super useful if you want your animation to be activated by a hover effect or a button. By default, it is set to ‘running’, but to pause it, you can set this property to ‘paused’.

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="PoaaVQj" data-user="craterellus" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/craterellus/pen/PoaaVQj">
  Apple-play-state</a> by Sarah Lopez (<a href="https://codepen.io/craterellus">@craterellus</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

The following two properties are experimental and don’t have functionality in most browsers yet.  

## animation-timeline

You can use this one in Firefox, but it’s not compatible with any other browser at the time of writing this article.
Using the @scroll-timeline CSS rule, you can design a timeline for your animation. You can set the name specified in @scroll-timeline as the value for the animation-timeline property.

## animation-composition

When multiple animations affect the same property at the same time, animation-composition can be used to determine the animation that gets applied. The default value is ‘replace’, but there are other values, like ‘add’ or ‘accumulate’ that involve combining aspects of multiple animation properties into one.

So, there you have it. With these animation properties, the possibilities are endless. Not only can you toss an apple from one side of the screen to another, you can make that apple accelerate (with animation-timing-function), fly backwards (with animation-direction), loop infinitely (with animation-iteration-count) and more! 
I hope this was informative. Now, go forth and animate!

