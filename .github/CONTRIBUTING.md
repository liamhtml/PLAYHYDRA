# (DONT USE THIS YET ITS NOT DONE AND WONT WORK)
# contributing
when adding a new game, there are two steps:
## 1. add game image
add an image representing the game to the [assets/images/](https://github.com/liamhtml/PLAYHYDRA/tree/main/assets/images) folder. this is what will be on the main page of the site.
## 2. edit `index.html`
[in index.html](https://github.com/liamhtml/PLAYHYDRA/edit/main/index.html), paste this group of elements at the bottom of the `search-items` div.
```html
<div class="search-item">
    <img src="assets/images/game title.png" alt="Game Title" class="search-img" />
    <a href="/game.js?title=Game Title&url=https://thegame.com/the-game/index.html">Game Title</a>
</div>
```
then change it for the new game you're adding:
<br>
- the image src attribute should point to the game's corresponding image in the [assets/images/](https://github.com/liamhtml/PLAYHYDRA/tree/main/assets/images) folder.
- the image alt attribute should be set to the title of the game, properly capitalized, punctuated, and stylized.
- the anchor href attribute should point to a link with two params:
  - title: the full title of the game, properly capitalized, punctuated, and stylized.
  - url: the full link leading directly to the game for embedding in an iframe. check that you can open this raw link on your chromebook first, and that it is not blocked. if it is, it'll just be blocked on the site. to find a working link I reccommend inspecting the code of unblockedgames google sites, as often these ones work and it's just that sites.google.com is blocked.
- the value of the anchor should be the full title of the game, properly capitalized, punctuated, and stylized.
