---
title: "Shoot for the Moon"
excerpt: "**(Downloadable)** The evil Communists have made it into space and are trying to kick the U.S. off of the moon!"
header:
  overlay_image: /assets/images/game-sftm-3.png
  teaser: assets/images/game-sftm-3.png
sidebar:
  - title: "Worked on:"
    text: "2017 - Present"
  - title: "Engine:"
    text: "Unreal Engine 4"
  - title: "Language:"
    text: "C++"
  - title: "Genre:"
    text: "First-Person Shooter"
  - title: "Also known as:"
    text: "Knockback"
  - title: "Download link:"
    text: "[Prototype](https://jay2645.itch.io/knockback)"
gallery:
  - url: /assets/images/game-sftm-prototype-1.png
    image_path: assets/images/game-sftm-prototype-1.png
    alt: "Shoot for the Moon image 1"
  - url: /assets/images/game-sftm-prototype-2.png
    image_path: assets/images/game-sftm-prototype-2.png
    alt: "Shoot for the Moon image 2"
  - url: /assets/images/game-sftm-prototype-3.png
    image_path: assets/images/game-sftm-prototype-3.png
    alt: "Shoot for the Moon image 3"
  - url: /assets/images/game-sftm-prototype-4.png
    image_path: assets/images/game-sftm-prototype-4.png
    alt: "Shoot for the Moon image 4"
tags:
  - Downloadable
---

![Shoot for the Moon](https://thumbs.gfycat.com/SlightWhimsicalBighorn-small.gif)

Shoot for the Moon began life as [an entry for Ludum Dare 40, "The more you have, the worse it is."](https://ldjam.com/events/ludum-dare/40/knockback)  I'm proud that I placed fairly high in the "fun" category (164th out of 2886).

{% include gallery caption="Pictures of the prototype." %}

## Gameplay

The game itself takes inspiration from *Super Smash Bros.* in that it foregoes the "traditional" health system. Instead, as you take damage, a "damage percent" goes up. At higher damage percents, the player receives more knockback when they take damage. Once the player gets knocked off the stage, they are out (similar to sumo wrestling).

The twist *Shoot for the Moon* brings is you don't win by being the person with the most kills. Instead, you win by having the highest damage at the end of the round. This was added to try and discourage "camping," adding a "fast and furious" feel to the game. Even so, I was afraid that this mechanic would make players not want to shoot at one another -- there was no incentive in shooting someone, just in getting hit.

![Damage vampirism!](https://thumbs.gfycat.com/CreepyGoodnaturedAdamsstaghornedbeetle-small.gif)

The solution was to add a "vampirism" effect, where you take all the damage a player had when you successfully kill that player. With that tweak, it made "securing the kill" an important part of the game. The change also accentuated the "fast and furious" gameplay by causing damage totals to rise across the board over the course of a match. At the end of the game, people are flying absolutely everywhere, damage totals are ridiculously high, and overall the game was fun to play (as indicated by my Ludum Dare scores).

That was the game I launched as part of the Ludum Dare, and what [you can download here.](https://jay2645.itch.io/knockback)

---

After the jam, work continued on the game, with a departure from the stock Unreal Engine models and a more solid codebase. I moved from Blueprints to C++, plus added online play and local couch co-op.

## The Problem

{% include figure image_path="https://media.giphy.com/media/xTiIzFsXVqp5QvEBTG/giphy.gif" alt="It's over, Anakin. I have the high ground." caption="Demonstrated here by Obi-Wan Kenobi himself." %}

Players would get launched. What goes up must come down. And when they came down, they landed on top of a rooftop or piece of scenery, giving them the perfect vantage point to look over the battlefield and get shots in without exposing themselves much in return.

Another problem: Players could be pinned against the wall and continuously shot up into the air. They would bump against the walls and land back on top of the person who shot at them, who would shoot at them again, throwing them up in the air, they would land on top of the person who shot them, etc. -- effectively "juggling" the player unfortunate enough to get stuck against a wall.

I realized that both problems could be solved fairly simply by giving the players more aerial mobility. I gave players jetpacks which could be used to boost them high up into the air -- letting them attack people who were camping out in high places, as well as giving them the chance to escape when they were being juggled.

![Now with jetpacks!](https://thumbs.gfycat.com/InsignificantGraveLeech-small.gif)

## Charging into Battle

As a kid, I was a massive fan of the *Halo* games. *Halo* has what Bungie called the "golden triangle" of weapons, grenades, and melee. It adds depth to the game by giving the player multiple options -- grenades to help with crowd control, melee to kill unsuspecting enemies or kill off weakened enemies, and weapons to use in every other instance.

*Shoot for the Moon* only had 2 options: shoot or run. On some level, there's a certain fun in simplicity, but I wanted to try and add depth to the game. I wanted to give the player options, and I decided to take a page from Bungie's playbook and added a "charging" mechanic to try and help with crowd control. The player could choose to charge their weapon up to cause it to explode and deal knockback over a wide area. I decided to tie this into the same meter that gives fuel to their jetpack.

This caused the intended effect, but it also caused fewer shots to be fired overall, which slowed down the gameplay considerably. I'm still going back and forth over whether I want to keep this change or convert it to a secondary fire "grenade" option.

---

![Shoot for the Moon image 1]({{ site.url }}{{ site.baseurl }}/assets/images/game-sftm-1.png)
{: .full}

![Shoot for the Moon image 2]({{ site.url }}{{ site.baseurl }}/assets/images/game-sftm-2.png)
{: .full}

I created the Space Station and character models shown above. I also did all game design, level design, and code.

Otherwise:

* The skybox comes from the [StarSphere Marketplace asset](https://www.unrealengine.com/marketplace/en-US/item/03afa1548b5c4b49b3e5c8f4a0e44444).

* Props (including moons, planets, etc.) from [Simple Space Interiors](https://www.unrealengine.com/marketplace/en-US/item/d8c42ffc204e42c5864012f9226ddbe3) and [Simple Space](https://www.unrealengine.com/marketplace/en-US/item/ac79973b35514228b8853c561e26e066).

* The guns are Creative Commons Zero assets from [the always-amazing Quaternius](https://www.reddit.com/r/gamedev/comments/8n5931/free_lowpoly_scifi_guns/).

* Explosion particle effects from from the [Cartoony Impact Pack](https://www.unrealengine.com/marketplace/en-US/item/376c3ca912d14e54ae51db9a45e38ba2).

* The post-process shader is a heavily modified version of one of the shaders found in the [Advanced Cel Shader Pack](https://www.unrealengine.com/marketplace/en-US/item/73d7b174d3dc49b4992ad2d1b5760a42).