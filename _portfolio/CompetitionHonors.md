---
title: "Competition Honors"
excerpt: "The 17-th \"HuaWei Cup\" China Graduate Mathematical Modeling Competition.<br/><img width='50%' src='/images/secrets/competitionhonors/MathModeling-Competition.JPG'><br/><br/> Internet+ Innovation Competition.<br/><img src='/images/secrets/competitionhonors/Internet-plus-competition.JPG'>"
collection: portfolio
---

The following are the screenshot of my honor certificates of 17-th "HuaWei Cup" China Graduate Mathematical Modeling Competition. 🙊🙊🙊 <a href="#secret-access-enter">(Need Secret Access)</a>

<div class="SecretContainer" style="display: none;">
    <img src="/images/secrets/competitionhonors/huaweicup-mathmodeling.png" alt="2020 & 17-th HuaWei Cup MathModeling Competition screenshot.">
    <br/>
    <br/>
</div>

The following are the screenshot of my honor certificates of National Graduate Internet+ Innovation and Entrepreneurship Competition. 🙊🙊🙊 <a href="#secret-access-enter">(Need Secret Access)</a>

<div class="SecretContainer" style="display: none;">
<img src="/images/secrets/competitionhonors/Internet-plus-2020.png" alt="2020 Internet+ Innovation and Entrepreneurship Competition screenshot.">
    <br/>
    <br/>
</div>

Secret Access
------
<h3 id="secret-access-enter" style="color: red;">Would you like to see more of my confidential information? Crack the password below to find out more.</h3>
<input type="password" id="password" placeholder="Enter password ... Otherwise contact me via email: weiqiangjin@stu.xjtu.edu.cn">
<button onclick="checkPassword()">click</button>

<script>
    function checkPassword() {
        var passwordInput = document.getElementById("password").value;
        var inputAsNumber = parseInt(passwordInput);
        var currentTimeInMinutes = new Date().getMinutes();
        var correctPassword = currentTimeInMinutes; // 密码就是当前时间分钟指针的指向的数字.
        if (!isNaN(inputAsNumber) && inputAsNumber >= 0 && inputAsNumber <= 59 && inputAsNumber === correctPassword) {
            var secretelements = document.getElementsByClassName("SecretContainer");
            alert("😄😄😄 Access Success.");
            for (var i = 0; i < secretelements.length; i++) {
            secretelements[i].style.display = "block"; 
            }
        } else {
            alert("😖😖😖 Error password, please contact me via email: weiqiangjin@stu.xjtu.edu.cn");
        }
    }
</script>