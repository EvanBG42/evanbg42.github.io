---
author: Evan BG
title: 'Riichi Mahjong: A Digital Primer'
summary: Riichi Mahjong is a super cool game that can be daunting to learn. This primer aims to help readers get started playing a digital version to get hands-on experience quickly.
---
<style>img {max-height: 500px}</style>

![Mahjong tiles scattered]({% link /assets/images/2023/mahjong_stock.png %})

*src: [iStockPhoto](https://www.istockphoto.com/photo/mahjong-game-gm475539562-65402417)*

For westerners, mahjong brings up thoughts of tile-matching solitaire, or a game for retirees. There's a LOT more to mahjong, especially my absolute favorite version: riichi. This style of mahjong is popular in Japan, and although it can be a little tough to get into, I think it's an extraordinary game that's well worth the effort.

Unlike the solitaire version, traditional versions of mahjong take the form of a 4-player draw-and-discard game. This game includes elements reminiscent of rummy and poker, and combines the two into a delightful balance of luck and skill. It’s also an excellent social game, where players can play defensively and try to avoid giving someone the tile they need, or play offensively and swipe tiles from someone else’s discard to win.

The goal of this article is to act as a primer for playing riichi in a digital format (online or in a video game). This won't include *all* the rules and info needed to play in-person, just enough info to get started playing and get a feel for the game. If you already know riichi, there might even be parts missing that you feel are super important! The goal here is to help beginners get a grasp on the basics of the game without bogging them down with all the details.

## Big Picture

Four people draw and discard tiles until one of them has a hand that contains at least one "yaku". Players can draw either from the unplayed tiles, or from a tile someone else discarded.  A yaku is a pattern or condition that a hand must meet in order to score. They have similarities to poker hands, but there’s more variety to them, and a mahjong hand can contain multiple yaku. Once a player has a valid hand, they win the round and score points from one or all of their opponents (depending on how they got the last tile). Remember that for a hand to be valid, it has to have at least one yaku worth points. Once the points are scored, the tiles are shuffled and dealt and the game goes to the next hand. Lather, rinse, and repeat until either everyone's had a turn as dealer or you reach some score limit.

This overview may make it seem dirt simple, but there are a lot of smaller details that add nuance, strategy, and depth to the game. I think these smaller parts are most fun when you can learn them after getting some experience first.

The rest of this article is an overview of only what is absolutely needed to play a digital version of the game. In this overview, I will primarily be using English names and corresponding numerals / characters to help flatten the learning curve.

## The Tiles

![Mahjong tiles]({% link /assets/images/2023/mahjong_tiles.png %})

*src: [FluffyStuff on GitHub](https://github.com/FluffyStuff/riichi-mahjong-tiles)*

A riichi mahjong set consists of the following:

- 3 suits of tiles numbered 1-9. From top to bottom in the image above, these suits are Characters, Dots, and Bamboo. Some sets or games include Arabic numerals for the characters, which can be helpful for newbies.
- Two groups of honor tiles:
    - The winds: east, south, west, and north. Again, these sometimes have the corresponding letter in the corner to help newbies.
    - The dragons in red, white (often completely blank), and green. 

For each of these unique tiles, there are four copies in the full set. This gives a total of 136 tiles. Note that if you are using an American set of mahjong tiles, there are likely some leftovers not used in riichi.

## Hand Composition

The goal of riichi mahjong is to build a hand composed of one or more yaku, and to prevent the other 3 players from building their hands before you can. Remember that a yaku is a sort of pattern or condition to the hand. There are a whole lot of yaku, but the majority of them are built of the same parts:

- **Sets**: Three of the same tile. They must all be the exact same (same number and suit, or same honor tile). Often called a “pon”.
    - In some instances, you can have a Set with 4 of the same tile (called “kan” or “kantsu”). These count the same as a set of three for most yaku, but since it messes with the number of tiles available to you, I don’t recommend newbies do these.
- **Runs**: Three consecutive numbered tiles of the same suit. Runs are always exactly three tiles, no more. Additionally, numbers don't "wrap around" from 9 to 1. Often called a “chi”.
- **Pair**: Two of the exact same tile.

Of these 3 components, most yaku consist of 3 sets / runs and 1 pair. I recommend new players always keep this in mind and aim for yaku of this form. 

When you choose to draw a tile from an opponent’s discard, it must generally be to complete a set or run. Once you grab the tile, you place the corresponding set or run face-up in front of you. Because part of your hand is now visible to the opponents, your hand is now considered “open” (as opposed to “closed” when only you can see your tiles). Some yaku only work with closed hands, and some are worth less when open. Generally, I like to keep my hand closed unless the set or run I finish with the discarded tile gets me a yaku that’s fine being open.

## Core Yaku

There are a few yaku that are especially common and useful to know when starting out. These are not necessarily the highest scoring, but they can be reliable yaku for new players to aim for. 

- **Honor Triplet**: A hand containing at least one triplet of a dragon, the player's wind (the wind corresponding to the seat you’re sitting in), or the prevailing wind. Prevailing wind means the wind that represents the round being played, and should be visible on-screen when playing digitally. Open or closed.
- **All Simples**: A hand that only uses tiles between 2 and 8 of any suit(s). No dragon or wind tiles, and not using the numbers 1 or 9. Open or closed.
- **Three Same-Number Runs**: Three runs that have the same numbers in each group (e.g. three runs of “123”). Open or closed, but worth more closed.
- **Three Triplets**: Three sets of triplets. Must be closed.
- **Riichi**: The name of the game! This is less a pattern of tiles, and more a way you play your hand. Your hand must be closed, and you must be only one tile away from winning. When in this position, you can call "riichi" and place an additional wager of 1000 points. From here out, you can't discard any of the tiles currently in your hand -- you're just drawing and discarding until either you draw what you need to win, or an opponent discards it.

<img src="/assets/images/2023/riichi_basic_hands.png" max-height="750px" title="Basic Riichi Hands">

*src: Unknown! If you know where this is from, please let me know.*

## Gameplay

To build these hands, players take turns around the table drawing a tile from the tiles remaining after dealing (the "wall"), and discarding a tile face-up in front of them to end their turn.

This isn't the only way to get new tiles -- you can also get them from your opponents discards, but typically only if you use them to complete a set or run!

- **Completing Sets**: If the opponent immediately before you discards a tile that would complete a set, you can call "pon!" and place the set face-up in front of you.
- **Completing Runs**: If ANY player has discarded a tile you need to complete a run, you can call "chi!" to take that tile and place the run face-up in front of you.

Note that you will still need to discard a tile to end your turn after taking someone’s discard. Placing your tiles face-up in front like this opens your hand (since your opponents can see part of your hand). Some yaku either can't be made with an open hand, or their value is lowered. When in doubt, keeping your hand closed is the safest call. But like many things, the best move depends on what's going on in your game!

The only time you can make a call for the second tile in a pair is when that last tile totally completes your hand. 

Be careful about what you discard. If you discard a tile, and later realize that you need it for your hand, you won’t be able to claim it from someone else’s discard. This is the most common form of “furiten” – discarding something and needing it later. In this situation, you can still win by drawing the tile from the wall.

## Finishing a Hand

A complete hand in riichi mahjong actually requires you to have 1 more tile than you typically do. This means you can only finish a hand once you’ve drawn a tile or claimed someone else’s discard (since you temporarily have an additional tile during that time). If you’ve drawn the winning tile, you call “tsumo!”, and if you’re claiming an opponent’s tile to win the hand, you call “ron!”.

## Scoring

When it comes to roadblocks for new players, an overwhelming list of all the yaku and some fairly complex scoring are typically the main culprits. Since this guide is intended for beginners and focuses on digital play, I won't go super in-depth on how scoring works.

Players start with 25,000 points. Generally speaking, each yaku is worth a few "han" (sometimes transliterated as “fan”). Additionally, depending on the composition of the hand, you will also receive a certain amount of "fu" or "mini-points". Using both, and a bit of math, you can calculate the value of a hand. That value is subtracted from other players if the winning tile was drawn, or from the discarding player if someone discarded the winning tile. Then, that value is added to your score.

It’s a fair amount of math, but luckily there are handy tables that spell it out - no calculations required. Even better if you just don’t pay attention and just let the video game do it for you! It's worth noting that there are limits to score values. When you have a certain amount of han, the fu don't matter and you just get a flat score. The limits are given names like "mangan" or the super-rare highest possible score limit: "yakuman". A hand can even be worth a multiple of these!

Further reading: [Japanese Mahjong Scoring Rules - Japanese Mahjong Wiki](https://riichi.wiki/Japanese_mahjong_scoring_rules)

## Wrapping Up

The rounds continue until either a player reaches a negative point value, or you've played to a target number of rounds. When that happens, the ranking of the score is set, and you have 1st, 2nd, 3rd, and 4th place.

## Further Reading

The above primer should be enough to get started playing a video game version of riichi. This should be enough to play and get a feeling for what riichi is all about. This guide doesn’t cover everything, though! There are many more yaku, including some fun gimmicky ones like "bamboo forest" (all bamboo tiles), "all honors", and "thirteen orphans" (1 and 9 of each suit, and one of each honor tile). Additionally, there are a few extra nuances to certain rules that you typically don't have to worry about with digital play.

Not sure where to play? Here are some favorites:
- [Kemono Mahjong](http://cyberdog.ca/kemono-mahjong/): An excellent implementation of riichi with animal characters who have different personalities and play styles. Bonus points for a mobile implementation that plays with the screen vertical!
- [Clubhouse Games on Nintendo Switch](https://www.nintendo.com/store/products/clubhouse-games-51-worldwide-classics-switch/): The new Clubhouse Games has riichi as a part of it. I haven't played this, but it looks super polished.
- [Mahjong Soul](https://mahjongsoul.yo-star.com/): This is probably the easiest to set up and play online with friends. Minus points for having some super anime-tropey art in some not great ways. And it's a gacha game. Luckily you don't *have* to engage with that stuff to play with friends.

Once you've played some riichi, here are some great resources for learning more:
- [Japanese Mahjong Wiki](https://riichi.wiki/Main_Page): This is a community wiki for riichi. It includes yaku info, strategy tips, and info about various digital versions of the game.
- [Downloads - World Riichi Championship](https://www.worldriichi.org/player-materials): The World Riichi Championship has a great cheatsheet for all the yaku.
- [Riichi Book I by Daina Chiba (pdf)](https://dainachiba.github.io/RiichiBooks/): This is an excellent book for players looking to get better at riichi.

I hope this was helpful, and I hope you have fun playing riichi!