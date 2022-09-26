---
toc: true
layout: post
author: Kaiden Do
categories: [week5]
title: HTML Program Purpose
---

.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
}
<html>
  <img src="Imageforproject.jpg">

  <button onclick="aText()" class="button">A</button>
  <button onclick="bText()" class="button">B</button>
  <button onclick="cText()" class="button">C</button>
  <button onclick="dText()" class="button">D</button>


  <p id="textbox"></p>

  <script>
  function aText() {
    document.getElementById("textbox").innerHTML = "The program would give the user two cards. After that, the user is prompted to either hit or stand. If they hit the program would give them another card. If they stand, the user can no longer do anything for the rest of the round.";
  }
  function bText() {
    document.getElementById("textbox").innerHTML = "Once the user stands, it is the dealers turn. The program would give the dealer a random card and if the cards add up to less than 16, the dealer would hit no matter what. After the dealer would play until the program decides the cards the dealer has is good enough.";
  }
  function cText() {
    document.getElementById("textbox").innerHTML = "The card deck would be visual, so the user would be able to see the cards moving across the screen.";
  }
  function dText() {
    document.getElementById("textbox").innerHTML = "The round ends when either the dealer or user busts or when the dealer stands. If the dealer busts but the user does not, the user wins chips. If the user busts, then the user gets nothing. Then the cards of the dealer and user are compared and the one closer to 21 wins.";
  }
  </script>

  </body>
</html>