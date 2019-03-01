---
title: "Traps and Treasure"
excerpt: "**(Downloadable)** Loot-- err, explore a procedurally-generated temple while dodging traps and searching for a jackpot!"
header:
  overlay_image: /assets/images/game-trapsandtreasure-prototype-3.png
  teaser: assets/images/game-trapsandtreasure-prototype-3.png
sidebar:
  - title: "Worked on:"
    text: "2017 - Present"
  - title: "Engine:"
    text: "Unreal Engine 4"
  - title: "Language:"
    text: "C++"
  - title: "Genre:"
    text: "First-Person Action Roguelike"
  - title: "Also known as:"
    text: "Imperialism, Ho!"
  - title: "Download link:"
    text: "[Prototype](https://jay2645.itch.io/traps-and-treasure)"
gallery:
  - url: /assets/images/game-trapsandtreasure-prototype-1.png
    image_path: assets/images/game-trapsandtreasure-prototype-1.png
    alt: "Prototype image 1"
  - url: /assets/images/game-trapsandtreasure-prototype-2.png
    image_path: assets/images/game-trapsandtreasure-prototype-2.png
    alt: "Prototype image 2"
  - url: /assets/images/game-trapsandtreasure-prototype-4.png
    image_path: assets/images/game-trapsandtreasure-prototype-4.png
    alt: "Prototype image 3"
  - url: /assets/images/game-trapsandtreasure-prototype-5.png
    image_path: assets/images/game-trapsandtreasure-prototype-5.png
    alt: "Prototype image 4"
  - url: /assets/images/game-trapsandtreasure-prototype-6.png
    image_path: assets/images/game-trapsandtreasure-prototype-6.png
    alt: "Prototype image 5"
---

Traps and Treasure is a prototype of the dungeon-crawling that will eventually make its way into another game I'm working on, Imperialism, Ho! The dungeon is procedurally generated each time the game is run, adapted from [Joris Dormans' "Adventures in Level Design"](https://web.archive.org/web/20180625012615/http://www.jorisdormans.nl/pdf/dormans2010_AdventuresInLevelDesign.pdf) paper.

{% include gallery caption="Some screenshots from the prototype." %}

The prototype has a few issues, namely that dungeons generated require a lot of backtracking. This is being worked on, and you can follow along with the [open-source dungeon creation algorithm.](https://github.com/Jay2645/DungeonMaker)

I created all the code for the game and adapted the core generation code from the aforementioned paper. Otherwise:

* Art is from the [Simple Temples](https://www.unrealengine.com/marketplace/en-US/item/da8740323fd74b36acc0b8a349320cd5) and [Simple Dungeons](https://www.unrealengine.com/marketplace/en-US/item/62bf02fd54014a53adb8b594f20c8bfc) packs.

* UI is from the [Cartoon UI Paper Pack](https://www.unrealengine.com/marketplace/en-US/item/b2b6853327bb4c03bdeebbdc3f0b071c).

* Cel Shader is a heavily modified version of a shader from the [Advanced Cel Shader Pack](https://www.unrealengine.com/marketplace/en-US/item/73d7b174d3dc49b4992ad2d1b5760a42).