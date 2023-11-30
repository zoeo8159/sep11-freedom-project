# Entry 1
##### 11/6/22

**Today **

[Next](entry02.md)

[Home](../README.md)

The tool I chose for my Freedom Project is [Kaboom](https://kaboomjs.com/). Kaboom is a platform that helps create any type of games. I decided to tinker with the sprites.

```js
import kaboom from "kaboom"

const k = kaboom()

k.loadSprite("bean", "sprites/bean.png")

k.onClick(() => k.addKaboom(k.mousePos()))
```
At first my code was not working. It was not loading. It was because I decided to take out

```js
k.add([
	k.pos(120, 80),
	k.sprite("bean"),
])
```

I was wondering what this code would do. This code was to set up the position. After a while I decided to switch around the numbers & add all my code together.

```js
import kaboom from "kaboom"

const k = kaboom()

k.loadSprite("bean", "sprites/bean.png")

k.add([
	k.pos(120, 80),
	k.sprite("bean"),
])

k.onClick(() => k.addKaboom(k.mousePos()))
```