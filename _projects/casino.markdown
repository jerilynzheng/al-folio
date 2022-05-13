---
layout: descrip
title: Casino
description:
img: /assets/img/casino.jpg
importance: 3
category:
---

**Casino**

Project Lead + Code / Fall 2020

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="center" src="{{ '/assets/img/casino.jpg' | relative_url }}" alt="" title="casino"/>
    </div>
</div>
<div class="caption">
    Casino
</div>

This casino project imitates a real-life casino environment. Players can play 2 games: <mark>slot machine and blackjack</mark>.

---

**Overview**

**Team**

This project was from October 2020 to December 2020. It was the final project for CS 3110.

There were three group members. 
- Jerilyn
- Mahak
- Carter

In addition to splitting the Ocaml coding with my other team members, I acted as the liason between our TA and the rest of our group, working to make sure that our team was on track and making good progress. I also led out team meetings and worked with the other members to set realisitic deliverables.

**Features**

The player can access games from the casino. They can play 2 games: slot machine and blackjack. The player can <mark>win</mark> money and <mark>gamble</mark> money across multiple games and then leave with their final balance. Multiple players can join the casino and make wagers.

One person can play the slot machine at a time, and as many players in the casino can choose if they want to play blackjack and make their own wagers. After playing a game, each players’ balance will be <mark>updated based on the wagers</mark> that they made. After playing the game, players can choose to stay or leave the casino. If they choose to stay, they can pick the game they want to <mark>play again</mark>, and can continue to be in the casino as long as everyone’s balance is greater than 0.

**Product**

Coded entirely in Ocaml, the casino is played through the terminal.

**Outcome**

We managed to complete the project and present something that can be played and mimics a real casino. 

Before, Blackjack only worked with one player, but now <mark>multiple players</mark> can play at once. We also upgraded the casino so that each player and their wagers are stored, and can be updated after playing games. We also made our project a lot more user friendly. Instead of having the user call multiple functions in utop, there is one overarching function that brings everything together and requires <mark>only user inputs</mark>.

The Blackjack compilation unit was upgraded so that it reflected more of the <mark>quirks in blackjack rules</mark>. The game now factors in wins, losses, and ties. The game also accounts for the values of face cards as 10, and also factors in how the values of aces change from 1 to 11 depending on the total sum. The game can be played with multiple players against the dealer.

In Casino, we managed to work a lot on user input and specifically, continuing to prompt for inputs until the user gives one that works for the casino. For example, if a user bets more money than they have in their balance, the casino will continue asking them for a bet until it is valid. Another example of this is when a player enters in a non-integer value for the balance. The system detects this and continues asking, rather than failing and forcing the user to start again. After playing a game, players can choose to stay or leave if everyone in the casino still has a positive balance. This reflects an actual casino environment, and encapsulates the idea of playing <mark>multiple different games in the casino</mark>. 

**Learnings**

The project was split into three milestones: milestone 1, milestone 2, and milestone 3.

Throughout each milestone, we utilized the following:
- <mark>Productivity</mark>: We were productive as a team. It was tricky finding times to meet together, especially near the end of the semester with finals, so we would usually give each other updates on what we had accomplished.
- <mark>Partner Programming</mark>: We (Jerilyn and Mahak) also utilized partner programming, which was very helpful for debugging and also deciding how to implement functions. Because we could run ideas through each other, the process became much more collaborative and faster.
- <mark>Testing</mark>: Because our system ran through the terminal, much of the testing was from user inputs. Manually testing the many user inputs was quite time consuming, as the recursion made it so that it was sometimes hard to debug. We managed to complete the project and present something that can be played and mimics a real casino.
- <mark>Feedback</mark>: We asked our TA and other people who were playing the game on what could be improved. This allowed us to reach a better user interface where it was intuitive and have a multi-player mode.