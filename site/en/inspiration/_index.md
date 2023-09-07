---
title: "Inspiration"
menu: "Inspiration"
weight: 3
bookCollapseSection: false
---

# Inspiration

Here are a few applications, some of which allow users to interact (two-panel preview). All these applications are grouped together in the repository at <https://github.com/epeios-q37/zelbinium>. The term in brackets is the name of the folder in which the source code for each application is located.

Clicking on an application's preview gives you access to its *repl*, from which the application can be [launched](../action/launch), [shared](../action/share), [explored](../action/explore), [modified](../action/modify) and used as inspiration to [create](../action/create) your own applications, as detailed in the [*Action!*](../action/) section.

## *Hello, World!* (`Hello`)

[*Hello, World!*](https://en.wikipedia.org/wiki/%22Hello,_World!%22_program) program showing the basics of a *Zelbinium* application. The application simply displays a message showing the contents of a text field.

<div data-demo="Hello"></div>

## *Hello, World!* shared (`Hellos`)

Same application as above, but messages are displayed to all users. Shows the basics of an application that allows users to interact.

<div data-demo="Hellos"></div>

## *Messages* (`Messages`)

This is the application used in the [*Action!*](../action/) section. It allows messages to be exchanged between all devices connected to the same application.

<div data-demo="Messages"></div>

## *Widgets* (`Widgets`)

This application shows an example of use of commonly used graphical interface components ([*widgets*](https://en.wikipedia.org/wiki/Graphical_widget)) and the corresponding source code (*HTML* and *Python*).

<div data-demo="Widgets"></div>

## *Connect Four* (`FourInARow`)

The [*Connect Four*](https://en.wikipedia.org/wiki/Connect_Four) game.

<div data-demo="FourInARow"></div>

## *Mancala* (`Mancala`)

The ancient two-player, seed-sowing game.

Grab the seeds from a pit on your side and place one in each following pit, going counterclockwise and skipping your opponent's store. If your last seed lands in an empty pit of yours, move the opposite pit's seeds into your store. The goal is to get the most seeds in your store on the side of the board. If the last placed seed is in your store, you get a free turn.

<div data-demo="Mancala"></div>

## *Flood it!* (`Flooder`)

Set the upper left color/shape, which fills in all the adjacent squares of that color/shape, by selecting a square with the desired color/shape. Try to make the entire board the same color/shape.

<div data-demo="Flooder"></div>

## *Blackjack* (`Blackjack`)

The classic card game also known as 21 (This version doesn't have splitting or insurance).

<div data-demo="Blackjack"></div>

## *Pig game* (`PigGame`)

A multi-player version of the [Pig game](https://en.wikipedia.org/wiki/Pig_(dice_game)#Gameplay).

You can choose to play against the computer, or with a partner.

<div data-demo="PigGame"></div>

<script>
  function demoLink(element) {
    const demo = element.getAttribute("data-demo");
    element.innerHTML = '\
<center>\
  <div style="font-size: smaller; font-style: oblique;">Click <a target="_blank" href="https://replit.com/@Zelbinium/' + demo + '">here</a> or on the preview to access the application.</div>\
  <div>\
    <a target="_blank" href="https://replit.com/@Zelbinium/' + demo + '">\
      <img src="./' + demo +  '.gif"/>\
    </a>\
  </div>\
</center>';
  }

  const demos = document.getElementsByTagName("div");

  for ( const demo of demos ) {
    if ( demo.hasAttribute("data-demo") )
      demoLink(demo);
  }
</script>
