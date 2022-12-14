---
toc: true
layout: post
author: Kaiden Do
categories: [markdown, week7]
title: Group Plan
---


<body>
      <div class="px-5 py-5 mx-auto">
            <h1 style="color:red;"><strong>Lawnmowers Game Arcade</strong></h1>
            <p style="color:white;"><b>Project Purpose and Function:</b> We would like to create a website that consists of mini games like retro games and casino games.</p>
            <p style="color:white;"><b>Different Components:</b> We would like to have Retro Games: Pong and Snake + Casino Games: Blackjack and Slot Machine. Also we will have a currency.</p>
            <p style="color:white;"><b>Frontend Stuff:</b> We will use HTML and CSS to create a homepage that links to the separate games. We will have a grassy, lawnmower theme and it would have sound effects related to lawn mowing.</p>
            <ul>
                <li style="color:white;"><p style="color:white;">The <b>Pong</b> game will use grass patches as the paddles and a small lawnmower icon as the ball.</p></li>
                <li style="color:white;"><p style="color:white;">In the <b>Snake</b> game we will replace the snake with a lawnmower and it gets longer when it eats grass clumps and as it gets longer the grass holder extends.</p></li>
                <li style="color:white;"><p style="color:white;">In the <b>Blackjack</b> game we will have a blackjack table that shows buttons to pick hit or stand and bet. The cards and chips also would move around the screen.</p></li>
                <li style="color:white;"><p style="color:white;">In the <b>Slot Machine</b> game there would be a slot machine with a button that would start the spinning of the machine and then it would display the winnings and result.</p></li>
                <li style="color:white;"><p style="color:white;">The <b>Currency</b> would be a leaf icon.</p></li>
            </ul>
            <p style="color:white;"><b>Backend Stuff:</b> For our games, we will use a library called pygame and turtle. For our graphics, we will upload photos and use photoshop and our artistic skills to make different icons.</p>
            <ul>
                <li style="color:white;"><p style="color:white;">In the <b>Pong</b> game we will follow the mouse cursor and the ball will bounce off the paddles and slowly increase speed.</p></li>
                <li style="color:white;"><p style="color:white;">In the <b>Snake</b> game we will take arrow input to control the lawnmower. And the program will detect if the Snake hits itself or the wall. (<b>Algorithm Implementation</b> can be used here because the sequencing can occur while the game is starting up and prompting the user to start, the selection can happen when it detects if the user clicks a key in order to move, and the iteration can repeat the detection of the keys while the game is playing)</p></li>
                <li style="color:white;"><p style="color:white;">In <b>Blackjack</b> we will let the user hit or stand and bet their currency. Then after they stand the program would control the dealer to play its turn. Then if the player did not bust, the points of the player would be compared to the dealer to decide the winner. (<b>Procedural Abstraction</b> can be used here to set a function that would check if the player won or busted)</p></li>
                <li style="color:white;"><p style="color:white;">For the <b>Slot Machine</b> every spin will be random and if they have a 3 in a row and our program would check if they have three in a row. If it comes out true, then they would win whatever prize. (<b>Data Abstraction</b> can be implemented here to set the different images the slot machine could display and we can randomize it to display the slots)</p></li>
                <li style="color:white;"><p style="color:white;">The <b>Currency</b> would be global throughout the website and it would let them receive a reward and let them play the games. (<b>Managing Complexity</b> can be implemented here to track currency uses and amounts)</p></li>
            </ul>
            <p style="color:white;"><b>Testing:</b> While programming, we will be constantly testing our code to make sure it works and it functions are we desire it to.</p>
      </div>
  </body>