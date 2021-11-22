# Creating gravity effect with Kaboom.js

Kaboom is a fun library for creating simple javascript games.

This library provides a lot of useful functions that make programming game objects easier to understand and use.

In this tutorial, we're going to learn how to create the gravity effect for game objects. You can find the code we use at https://replit.com/@ritza/gravity-tutorial or you can try the code in the embedded repl below.

# Getting started with the code

The first thing we want to do is load the `kaboom()` library and initialize a Kaboom context. 

```
import kaboom from "kaboom";

kaboom();
```

Next, we're going to load the assets we'll be using during the game. In this case, our player sprite, Bean.

```
loadSprite("bean", "/sprites/bean.png")
```

## The gravity function

`gravity()` allows us to pull the character towards the bottom of the game screen. When we give characters the `body()` component, we're giving them a "physical body" with the ability to react to gravity in the game. 

```
const player = add([
	sprite("bean"),
	body(),
])
```

We can alter the acceleration of the gravitational pull by passing the number of pixels we want our character to move per second into `gravity()`, for example 

```
gravity(30)
```

where 30 is the number of pixels a character would accelerate per second, towards the source of gravity. The higher this value is, the faster a character would move.

Another fun example would be to simulate the force of gravity which is $$9.82m/s^2$$. 

```
gravity(9.82 **2)
```

Keep in mind, converting the actual value of the force of gravity to pixels would be a fairly large number and 9.82 would be passed as pixels and our characters would move entirely too slow. Thus, adding the exponent 2 will create a fairly acceptable acceleration rate.


# Things to try

Here are some suggestions to try out:

- Add other components to your game, for example, a surface for your player to land on. 
- Can you make your player jump after touching the ground?
- Try to reverse the gravity in the game and make your player gravitate upwards


### You can take a look at the repl below

<iframe frameborder="0" width="100%" height="500px" src="https://replit.com/@ritza/Gravity?embed=true"></iframe>
