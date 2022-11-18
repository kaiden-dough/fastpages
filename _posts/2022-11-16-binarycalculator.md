---
toc: true
layout: post
author: Kaiden Do
permalink: /frontend/binarycalculator
categories: [markdown, week13]
title: Binary Calculator
---

{% include navbarsubmenu.html %}

<div class="container bg-primary">
    <header class="pb-3 mb-4 border-bottom border-primary text-dark">
        <span class="fs-4">Decimal to Binary Calculator</span>
    </header>
    <form>
        <div class="form-group row">
            Input a decimal number:
            <div>
                <input oninput="convert('decimal', 'binaryfin')" type="text" class="decimal"  name="decimal" maxlength="16"><br>
            </div>
        </div>
        <div class="form-group row">
            Binary : <span id="binaryfin" >___</span>
        </div>
    </form>
    <form>
        <div class="form-group row">
            Input a decimal number:
            <div>
                <input oninput="convert('decimal2', 'binaryfin2')" type="text" class="decimal" name="decimal2" maxlength="16"><br>
            </div>
        </div>
        <div class="form-group row">
            Binary : <span id="binaryfin2" >___</span>
        </div>
    </form>
    <div class="form-group row">
        Choose an operation: <br>
        <button type="button" id="plus" onclick="add()">+</button>
        <button type="button" id="minus" onclick="subtract()">-</button>
        <button type="button" id="times" onclick="multiply()">*</button>
        <button type="button" id="slash" onclick="divide()">/</button>
        <br>
        Answer :  <span id="ans">___</span> <---> Binary Answer : <span id="binaryans" >___</span>
    </div>
</div>

<script>
    function add(){
        var array = document.getElementsByName('decimal');
        if (array[0].value.length != 0) {
            var decimal = parseInt(array[0].value);
            console.log("add:"+decimal);
        }
        var array2 = document.getElementsByName('decimal2');
        if (array2[0].value.length != 0) {
            var decimal2 = parseInt(array2[0].value);
            console.log("add:"+decimal2);
        }
        var added = parseInt(decimal) + parseInt(decimal2);
        console.log(added); 
        document.getElementById('ans').innerHTML = added;
        resultConvert(added);
    }
    function subtract(){
        var array = document.getElementsByName('decimal');
        if (array[0].value.length != 0) {
            var decimal = parseInt(array[0].value);
            console.log("add:"+decimal);
        }
        var array2 = document.getElementsByName('decimal2');
        if (array2[0].value.length != 0) {
            var decimal2 = parseInt(array2[0].value);
            console.log("add:"+decimal2);
        }
        var added = parseInt(decimal) - parseInt(decimal2);
        console.log(added); 
        document.getElementById('ans').innerHTML = added;
        resultConvert(added);
    }
    function multiply(){
        var array = document.getElementsByName('decimal');
        if (array[0].value.length != 0) {
            var decimal = parseInt(array[0].value);
            console.log("add:"+decimal);
        }
        var array2 = document.getElementsByName('decimal2');
        if (array2[0].value.length != 0) {
            var decimal2 = parseInt(array2[0].value);
            console.log("add:"+decimal2);
        }
        var added = parseInt(decimal) * parseInt(decimal2);
        console.log(added); 
        document.getElementById('ans').innerHTML = added;
        resultConvert(added);
    }
    function divide(){
        var array = document.getElementsByName('decimal');
        if (array[0].value.length != 0) {
            var decimal = parseInt(array[0].value);
            console.log("add:"+decimal);
        }
        var array2 = document.getElementsByName('decimal2');
        if (array2[0].value.length != 0) {
            var decimal2 = parseInt(array2[0].value);
            console.log("add:"+decimal2);
        }
        var added = parseInt(decimal) / parseInt(decimal2);
        console.log(added); 
        document.getElementById('ans').innerHTML = added;
        resultConvert(added);
    }
    function resultConvert(num){
        console.log(num);
        var binary = [];
        var rem;
        if (num == "0") {
                console.log("go");
                binary.unshift("0");
            }
            else {
                console.log("go");
                while (num != 0){
                    rem = num%2;
                    console.log(rem);
                    num = Math.floor(num/2)
                    binary.unshift(rem);
                }
            }
            const final = binary.join('');
            console.log("binarrr:"+final)
            document.getElementById('binaryans').innerHTML = final;  
    }
    function convert(named, binaryfin){
        console.log("start");
        var array = document.getElementsByName(named);
        console.log("arr:"+array);
        if (array[0].value.length != 0) {
            console.log("go");
            var binary = [];
            var decimal = parseInt(array[0].value)
            console.log("-----in:"+decimal);
            var rem;
            if (decimal == "0") {
                console.log("go");
                binary.unshift("0");
            }
            else if(parseInt(array[0].value)) {
                console.log("go");
                while (decimal != 0){
                    rem = decimal%2;
                    console.log(rem);
                    decimal = Math.floor(decimal/2)
                    binary.unshift(rem);
                }
            }
            const final = binary.join('');
           
            console.log("thing:"+binary);
            console.log("fin:"+final);
            console.log("name:"+binaryfin);
            document.getElementById(binaryfin).innerHTML = final;    
            console.log("bin:"+final);    
        }
    }

</script>
