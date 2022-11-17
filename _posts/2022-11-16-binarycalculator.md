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
            Input a decimal number and press tab to convert it to binary:
            <div>
                <input onblur="convert()" type="text" name="decimal"/><br>
            </div>
        </div>
        <div class="form-group row">
            Binary : <span id="binary" >___</span>
        </div>
    </form>
</div>

<script>
    function convert(){
        var array = document.getElementsByName('decimal');
        if (array[array.length-1].value.length != 0) {
            var binary = [];
            var decimal = parseInt(array[0].value)
            var rem;
            if(parseInt(array[0].value)) {
                while (decimal != 0){
                    rem = decimal%2;
                    decimal = Math.floor(decimal/2)
                    binary.unshift(rem);
                }
            }
            const final = binary.join('');
            document.getElementById('binary').innerHTML = final;            
        }
    }

</script>