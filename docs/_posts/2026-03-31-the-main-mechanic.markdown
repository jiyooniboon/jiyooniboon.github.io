---
layout: post
title:  "The Main Mechanic"
date:   2026-03-31 16:00:24 +0900
categories: game-design
---
Since March 2025, I've been trying to make a game. Mostly to graduate, because I need to complete a project to get my degree and move on with my life. But also because I do like games, and I think the world could use a bit more fun. I took the two game design courses that were available when I was enrolled (more courses have been opened afterward, but I digress), I watched game playthroughs on Youtube (as entertainment more than research, but still research), and I played games myself. Then I had some weekly meetings with the professor that gives the game design courses for a semester, and came up with something of a game. 

Even though I'd learned the basics of game design - the formal elements, dramatic elements and so on - it took a long time to use that knowledge to then organize my ideas into the format of a game. There were some points from the game design sessions that I hope will help other beginner game devs! A lot of people will tell you that the best approach is to just start, try making it, try playing it, and make it better. But if you're like me and you can't "just start" without some sort of structure, maybe this blog could be somewhere to start. 

### What is the main mechanic? 
I already knew that the main mechanic had to be designed first, and iterated on the most, and fun on its own, etc. But it took a lot longer to really figure out what it really was. This was partly because I was imagining an adventure game, and the only "main mechanic" I could think of was "You walk around. You.. adventure." The answer to this was to think about *how* you walk around, and how you would be good or bad at walking around, and what rules would be in place to define the how, the good, and the bad. 

- There has to be some way to be good or bad at the game, and a way to get better at the game. This confused me because of the genre of game that I wanted to make. Obviously for combat centered games, or racing games, or score based games, or the vast majority of games honestly, the win/lose conditions are clear; get hit too many times, take too long to reach the goal point, get a low score, lose all your lives, and so on. Based on the win conditions, improving is also simple: dodge attacks better, make your weapon stronger, drive faster, and so on. But I didn't get how someone could be bad at adventure games, especially the ones without combat. For example, point-and-click adventure games, which are basically puzzle adventure games. To this my professor said puzzle games have a very prominent lose condition: if you can't solve the puzzle, you can't progress at all. Basically, just because there isn't a Game Over screen doesn't mean you can't lose a game. 
- There have to be concrete rules to define the mechanic. Once you've defined the how, the good and the bad, the rules are a bit easier to figure out. This is kind of when you start thinking about numbers behind the ideas and how they would be implemented. How many health points, how much damage, how much time, how many points, etc. 

Based on this information, I took some time to think of the main mechanic of some of my favorite games.

### Case Study: Good Pizza, Great Pizza
Good Pizza, Great Pizza is a restaurant management / simulation game, so it wasn't really the genre I was interested in making. Still, since the gameplay loop is relatively simple, it was a good starting point to understand main mechanics. At a glance, the main mechanic would be "make pizza, sell pizza, make money, repeat," but it helps to think about the details of "make pizza."
How: make and sell pizzas according to each order and make money.
Good: make the correct order, including types of toppings, number of slices, cooking time, etc. use enough toppings to make the customer happy, but not too much to lose money. serve the pizza before the customer loses patience. 
Bad: get the order wrong, take too long to make the pizza, use up too much toppings.
Rules: There are a set of possible orders that each customer can make. The price of the pizza is determined by the number of toppings/requests in the order (dough = $X, sauce = $X, each topping = $X). The tip is calculated when the pizza is served, based on the patience of the customer and the accuracy of the order. (base = X% of pizza price, -$X for each factor missed). The customer will wait X seconds before they lose their patience and leave, and the oven baker takes X seconds to bake 1 pizza. Each topping has a specified cost that is immediately subtracted from total funds upon use (1 pepperoni = $0.0X, etc.). 

### Case Study: Sneaky Sasquatch
Sneaky Sasquatch was one of the adventure games I brought up as a reference, and we spent some time identifying the main mechanic (beyond "you walk around"). In this game, you have to walk around without being seen or heard by the people. This means you have to hide in bushes or tents, or tip-toe around sleeping campers, or run away when the rangers are alerted. Later on, you can buy disguses which is a huge change but this would have been the main mechanic at the beginning of development (probably. uhh.. you know. from a learning point of view.)
How: explore the campsite to find food and treasure map pieces, but avoid being seen or heard by humans.
Good: hide or stay out of sight, keep quiet
Bad: get caught, either by being seen or being heard
Rules: If you stay in the field of vision of a human or are too loud for x seconds, the ranger is alerted. The ranger runs to catch you at x speed, and if you reach a loading zone in time, you have successfully run away. If you are caught by the ranger, you are forced out of the campsite.

### Case Study: Tiny Thief / Love You to Bits
Two of my favorite point and click adventure games! Unfortunately Tiny Thief has been deleted from the App Store, but Love You to Bits is very similar in style and available to play. 
Something to remember is that "point-and-click" isn't a genre or mechanic, but rather the player action/controls. A more accurate genre would be environmental puzzle adventure game. Like other adventure games, you walk around, but for these games you have to find objects and identify where to use them, usually to reach the goal of the level. The objects and problems are more specific to each game and each level, but that's the broad explaination.
How: find interactable objects, and where to use each object. 
Good: thorough search, finding the key to each lock.
Bad: miss relevant objects, use wrong key in given lock. 
Rules: In every level, there are a set of "locks" (problems to solve) and "keys" (solutions to each problem) in the form of interactable objects. The player can explore the map to pick up or interact with game objects. If the player finds the right key to each lock, they have solved the level. If they don't the game doesn't progress further. 

... 