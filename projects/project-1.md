---
layout: project
type: project
image: images/paintbrush.jpg
title: Java paint
permalink: projects/paint
# All dates must be YYYY-MM-DD format!
date: 2015-07-01
labels:
  - Eclipse
  - EZ.Java
  - Java
summary: I developed a java paint program in ICS 111.
---



Java paint was created as our first project in ICS111, with the implementation of EZ.java. This program uses only 3 colors, and it allows the user to draw anything with the three colors. When using one color, you can always swap to the other colors to draw while it keeps your line drawing for the other color, the only way to clear it is by using the clear page button.

For this project, I was creating it by myself, responsible for programming and all the due dates. I started with the basics of creating the window and then I had to figure out how I could connect one dot to the other from a mouse click. It took a while but I was eventually able to figure it out while the rest of the code would be easy, like changing colors and clearing the paint page. 

Here is some code that illustrates how I create the program:

```js
while (true) {

			if (EZInteraction.wasMouseLeftButtonDown(EZInteraction.getXMouse(),EZInteraction.getYMouse())) {
				c = lineColor4;
				}
			
			else if(EZInteraction.wasMouseLeftButtonPressed() && picture1.isPointInElement(EZInteraction.getXMouse(), EZInteraction.getYMouse())) { 
					 c=lineColor1;
					 sound1.play();
				 }
			 else if (EZInteraction.wasMouseLeftButtonPressed() && picture2.isPointInElement(EZInteraction.getXMouse(), EZInteraction.getYMouse())) {
					 c = lineColor2; 
					 sound2.play();
				 }
```





