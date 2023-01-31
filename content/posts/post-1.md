+++
title="Japanese explained to programmers"
date=2023-01-31

[taxonomies]
+++

Being born in France, I was immersed in Japanese culture from a very young age. Whether it was some imported Yu-Gi-Oh card found in a local store that taught me my first kanji (ideogram) at 11 (水), to a constant stream of Anime culture and video games.

I've always been fascinated by the language, learning it during recess at school, in some class in university, and more recently with the help of [WaniKani](https://www.wanikani.com/), a pretty neat SRS (spaced repetition system) app that teaches you kanji and vocabulary.

But as a programmer, something about Japanese has always felt natural. Whereas English and French can feel a bit chaotic, there is a sense of order in the Japanese language that reminds me of functional programming of all things. Let's examine this.

<!-- more -->

**Note : this is not a lesson in Japanese, but an introduction to how different language can be has different as Haskell and C. I'll purposedely focus on the most idiomatic parts of the language**

If japanese was a programming language, it would feature the following concepts:

## 1. Primitive types: Hiragana, Katakana and Kanji

```typescript
const ha:Hiragana = "は";
const ha2:Katakana = "ハ"; // same sound as hiragana version
const day:Kanji = "日";
```

Hiraganas and Katakanas are a phonetic alphabet, that allow to represent sound. Kanjis are logograms, that represent concepts.

## 2. Japanese Standard Library

The japanese standard library offers a bunch of chainable functions to add meaning to your primitive types.

```typescript
const me:Kanji = "私";
const eat:Kanji = "食";
const cow: Kanji = "牛";
const meat:Kanji = "肉";

const iEatBeef = word(me)
    .setRole("subject")
    .add(
        combinedWord(cow, meat)  // combining cow and meat you get beef
        .setRole("object")
    ),
    .add(
        word(eat)
        .transform("polite-present-verb")
    );
```

In actual japanese, that looks like

> 私 (me) + は (set role of subject) + (牛 (cow) + 肉 (meat)) + を (set role of object) + 食 (eat) + ます (transform to polite present tense)

The order does matter, it is quite different to english but very similar to functional programming.


```typescript
//You would not do the english order "Send the request to the server"
  send().request.setURL("serverurl")

  // you woudl do the japanese order "For this request, with the URL xxx, send it to the server"
  request.setURL("serverurl").send()
```

The neat thing about the japanese standard library is that it is very consistent. You can always expect the same result from the same input. It's a very predictable language. Verbs conjugate in a very predictable way (which coming from French is a breath of fresh air).

## 3: Even Kanjis themselves can be functions

It's not immediately obvious to our western eyes, but Kanjis are offten composed of multiple components. A pretty neat exemple are the types of fish.

```typescript
const fish:Kanji = "魚";
const blue:Kanji = "青";
const mackerel:Kanji = composeKanji(fish, blue); //"鯖"

const salmon:Kanji = "鮭";
const tuna:Kanji = "鮪";
```

You can see here as an example that all the kanjis for the various type of fish are composed of the kanji for fish, and a secondary kanji stuck together. This is a very common pattern in japanese. For instance here, Mackerel is **鯖**, composed of 魚 + 青, aka the "blue fish".


## 4: This extends to other parts of the language

I won't go into detail (although depending on the receiption of this I might do a part 2), but similar parallels can be made for prepositions, adjectives, adverbs... I did not go into the pronounciation of Kanji as that's a whole other conversation. 

I hope this triggered your curiosity for the language. Of course might have gotten stuff wrong, if so feel free to send me a message, tweet, comment on HackerNews or whatever you prefer. I'm always happy to learn more about Japanese and I'm sure I'll be making more mistakes in the future.
    
[![shrine](/images/shrine.png)](/images/shrine.png)