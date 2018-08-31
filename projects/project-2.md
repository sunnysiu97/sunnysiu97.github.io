---
layout: project
type: project
image: images/icshead.jpg
title: ICS Head
permalink: projects/icshead
# All dates must be YYYY-MM-DD format!
date: 2017-04-30
labels:
  - Java
  - Eclipse
  - EZ.JAVA
  
summary: A simple java 2d- Arena shooter game.
---


ICS Head was a game our group made during ICS111, with the implementation of EZ.java. I was in charge of creating the character movement, zombie movement, and bullet collision of how it looks when it shoots and how it affects the zombie. 

In this project I gained experience with for java video game design and how hard coding the collision hitboxes were even for such a simple game. Even with the help of our group memebers and the TA, we were having a hard time figuring out how to solve it. It was a good experience because it opened my eyes as to how many lines of code and the amount of effort was needed to program even such a simple game. Even though it was hard, the project was still a lot of fun to us because it taught us about leadership and how to work together as a group.

This is a part of the code of how we implemented the bullet collision and Hero movement:

```js
while(Hero.HERO_ALIVE == true){
			Hero.go(); //hero movemnt
			MoveZombie(); // zombie move towards 
			/*if (Hero.touchingZombie(zX, zY)){
				Hero.HERO_ALIVE = false;
				EZ.removeAllEZElements();
			}*/
			 HeroX = Hero.GetXCenter();
			 HeroY = Hero.GetYCenter();
	 
		for (int i = 0; i < 20; i++) {
			
			if (EZInteraction.wasKeyPressed('j') && Hero.moveleft == true) { // if j was pressed, character looking left, shoot left
				bulletright = false; // call all booleans false, except for character facing left
				bulletup = false;
				bulletdown = false;
				Bullet[i].translateTo(HeroX, HeroY); //create bullet.
				bulletleft = true;
			
			}
```
 

