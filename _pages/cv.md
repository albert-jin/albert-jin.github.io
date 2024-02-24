---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

⚠️⚠️⚠️ <span style="color: red; font-size: larger;">My personal resume in PDF format</span> can be downloaded via [Personal Resume-Albert Evans](https://raw.githubusercontent.com/albert-jin/albert-jin.github.io/master/files/Weiqiang%20Jin%20Resume.pdf) or [个人简历-金伟强](https://raw.githubusercontent.com/albert-jin/albert-jin.github.io/master/files/金伟强%20简历.pdf).

Education
======
* **(Until Now)** Ph.D Candidate in Information and Communication Engineering, Xi'an Jiaotong University, 2022~2026
* M.S. in Computer Engineering and Technology, Shanghai University, 2019~2022
* B.S. in GitHub, Computer Science and Technology, Anhui University of Technology, 2015~2019

Work (Intern) experience
======
* Spring 2024: Academic Pages Collaborator
  * eBay for foreign trade Corporation, Shanghai
  * Duties includes: Front-end interface development
  * Supervisor: eBay IaSS Team

* Fall 2015: Unity3D and Python Software Development Engineer
  * Shanghai Youhao Network Technology Co., Ltd, Shanghai
  * Duties included: frontend scene development for e-commerce platforms, backend application management, user barrage and monitoring
  * Supervisor: CEO of Shanghai Youhao Network Technology

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching (TBD)
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Skills (Secret)
======
* Skill 1
* Skill 2
  * Sub-skill 2.1
  * Sub-skill 2.2
  
Service and leadership (Secret)
======
* Service 1
  * Sub-Service 1.1
  * Sub-Service 1.2
* Leadership 1
  * Sub-Leadership 1.1
  * Sub-Leadership 1.2

Beautiful Life Records
------
The following are some of my beautiful life photos and records. 🙊🙊🙊 <a href="#secret-access-enter">(Need Secret Access)</a>

<div class="SecretContainer" style="display: none;">
    <img src="/images/secrets/lifephotos/eating.jpg" alt="beauty life image show 1.">
    <br/>
    <br/>
    <img src="/images/secrets/lifephotos/drinking.jpg" alt="beauty life image show 2.">
    <br/>
    <br/>
    <img src="/images/secrets/lifephotos/toilet.jpg" alt="beauty life image show 3.">
    <br/>
    <br/>
    <img src="/images/secrets/lifephotos/WryMouth.jpg" alt="beauty life image show 4.">
    <br/>
    <br/>
    <img src="/images/secrets/lifephotos/slim.jpg" alt="beauty life image show 5.">
</div>

TBD
------
.

Secret Access
------
<h3 id="secret-access-enter" style="color: red;">Would you like to see more of my confidential information? Crack the password below to find out more.</h3>
<input type="password" id="password" placeholder="Enter password ... Otherwise contact me via email: weiqiangjin@stu.xjtu.edu.cn">
<button onclick="checkPassword()">click</button>

<!-- <script>
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
</script> -->