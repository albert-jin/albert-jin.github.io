---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


<style>
    @keyframes deprecated-gradient-shift {
        0% { background-position: 0% 50%; }
        50% { background-position: 100% 50%; }
        100% { background-position: 0% 50%; }
    }

    #site-deprecated-overlay {
        position: fixed;
        inset: 0;
        z-index: 99999;
        display: flex;
        align-items: center;
        justify-content: center;
        background: linear-gradient(135deg, #ff7eb3 0%, #7afcff 45%, #f9f871 100%);
        background-size: 220% 220%;
        animation: deprecated-gradient-shift 9s ease infinite;
        padding: 1.2rem;
    }

    #site-deprecated-overlay::before {
        content: "";
        position: absolute;
        inset: 0;
        background:
            radial-gradient(circle at 15% 20%, rgba(255, 255, 255, 0.35), transparent 32%),
            radial-gradient(circle at 85% 80%, rgba(255, 255, 255, 0.28), transparent 30%),
            linear-gradient(to bottom right, rgba(255, 255, 255, 0.22), rgba(255, 255, 255, 0.08));
        pointer-events: none;
    }

    .site-deprecated-modal {
        position: relative;
        width: min(760px, 100%);
        border-radius: 24px;
        padding: 2.3rem 1.6rem 1.8rem;
        text-align: center;
        color: #102a43;
        background: rgba(255, 255, 255, 0.92);
        backdrop-filter: blur(8px);
        box-shadow: 0 22px 52px rgba(16, 42, 67, 0.28);
    }

    .site-deprecated-badge {
        display: inline-block;
        margin-bottom: 0.85rem;
        padding: 0.32rem 0.7rem;
        border-radius: 999px;
        font-size: 0.75rem;
        letter-spacing: 0.08em;
        font-weight: 700;
        text-transform: uppercase;
        color: #ffffff;
        background: linear-gradient(90deg, #0ea5e9, #f97316);
    }

    .site-deprecated-modal h2 {
        margin: 0 0 0.9rem;
        font-size: clamp(1.55rem, 4.3vw, 2.05rem);
        font-weight: 800;
    }

    .site-deprecated-modal p {
        margin: 0 auto;
        max-width: 640px;
        line-height: 1.72;
        font-size: 1.02rem;
    }

    .site-deprecated-link {
        color: #075985;
        font-weight: 700;
        text-decoration: underline;
        text-underline-offset: 2px;
        word-break: break-all;
    }

    .site-deprecated-countdown {
        margin-top: 1.2rem;
        font-size: 0.93rem;
        color: #334e68;
    }

    .site-deprecated-confirm {
        margin-top: 0.88rem;
        min-width: 132px;
        padding: 0.56rem 1.18rem;
        border: 0;
        border-radius: 10px;
        cursor: pointer;
        font-size: 1rem;
        font-weight: 700;
        color: #ffffff;
        background: linear-gradient(90deg, #0284c7 0%, #0f766e 100%);
        box-shadow: 0 10px 24px rgba(2, 132, 199, 0.33);
    }

    .site-deprecated-confirm:hover {
        filter: brightness(1.06);
    }

    #site-deprecated-overlay.is-closing {
        opacity: 0;
        transition: opacity 0.24s ease;
    }
</style>

<div id="site-deprecated-overlay" role="dialog" aria-modal="true" aria-labelledby="site-deprecated-title">
    <div class="site-deprecated-modal">
        <span class="site-deprecated-badge">Website Notice</span>
        <h2 id="site-deprecated-title">该个人网站已废弃</h2>
        <p>
            最新更新请访问
            <a class="site-deprecated-link" href="https://albert-evans.github.io/" target="_blank" rel="noopener">
                https://albert-evans.github.io/
            </a>
        </p>
        <div class="site-deprecated-countdown" id="site-deprecated-countdown">5 秒后自动关闭</div>
        <button type="button" class="site-deprecated-confirm" id="site-deprecated-confirm">确定</button>
    </div>
</div>

<script>
    (function () {
        var overlay = document.getElementById("site-deprecated-overlay");
        var confirmBtn = document.getElementById("site-deprecated-confirm");
        var countdownText = document.getElementById("site-deprecated-countdown");
        var secondsLeft = 5;
        var timerId = null;

        if (!overlay || !confirmBtn || !countdownText) {
            return;
        }

        function closeOverlay() {
            if (timerId) {
                clearInterval(timerId);
            }
            overlay.classList.add("is-closing");
            setTimeout(function () {
                if (overlay && overlay.parentNode) {
                    overlay.parentNode.removeChild(overlay);
                }
            }, 240);
        }

        function renderCountdown() {
            countdownText.textContent = secondsLeft + " 秒后自动关闭";
        }

        confirmBtn.addEventListener("click", closeOverlay);
        renderCountdown();

        timerId = setInterval(function () {
            secondsLeft -= 1;
            if (secondsLeft <= 0) {
                closeOverlay();
                return;
            }
            renderCountdown();
        }, 1000);
    })();
</script>

I, Weiqiang Jin, received the Computer Science Master's degree from Shanghai University, and I am currently an Artificial Intelligence-related PhD Candidate at Xi`an Jiaotong University, China. 

Making eminent contributions to the scientific research community is my biggest dream, which is also deeply engraved on the mind of me. My personal representative works are displayed on [Github](https://github.com/albert-jin/) and my brief intro are in the [Link3 Electronic Postcard](https://link3.cc/albert0309jin).

Served as the Academic Editor for [Plos One](https://journals.plos.org/plosone/) since 2024.03 to 2025.10 (about 1 year and a half).
<br/><img width='35%' src='/images/PLOSEdBoardBadge_ONE.png'><br/><br/>

Research Interests
======
1. Natural Language Processing, including Knowledge Graph-related Question Answering, Aspect-term Based Sentiment Analysis, Information Retrieval, Fake News Detection and Checking, and Prompt Learning. 
1. Reinforcement Learning, especially in researching the multi-agents information interaction mechanism based on large multi-modal model. 
1. Drug-Drug Interaction Prediction (DDI).
1. Large Medical Language Models and Applications. 

Education
======
Since September 2022: Ph.D. Candidate student in Information and Communication Engineering, Xi'an Jiaotong University. (Tutor: [Gui](https://std.xjtu.edu.cn/info/1072/15975.htm)[zhong](https://gr.xjtu.edu.cn/web/liugz) [Liu](https://dice.xjtu.edu.cn/info/1720/1807.htm))

June 2019 - April 2022: Master of Computer Engineering and Technology, Shanghai University. (Tutor: [Xiangfeng Luo](https://cs.shu.edu.cn/xygk1/xrld.htm))

September 2015 - June 2019: Bachelor's degree in Computer Science and Technology, Anhui University of Technology.

Achievements
======
1. Academic Achievements: Published over **20** academic papers, including SCI index journals and EI index conferences, with citations exceeding **100** on Google Scholar;
1. Project Experiences: Participated in numerous national and provincial-level major projects in the field of natural sciences;
1. School Honors: Received multiple school scholarships during undergraduate, master's, and doctoral studies, as well as a national scholarship during doctoral studies;
1. Competition Honors: Attained various competition honors, including the National Graduate Mathematical Modeling Second Prize, Internet Plus, Tengfei Cup, and so on;
<!-- Challenge Cup Innovation and Entrepreneurship Competition -->
1. Internship Experiences: Front-end Software Engineer in eBay for foreign trade Corporation, Shanghai, and Unity3D and Python Software Development Engineer in Shanghai Youhao Network Technology Co., Ltd;
1. Language Proficiencies: CET (Chinese College English Test) Level 4 and Level 6 and IELTS (International English Language Testing System) level **7.0**;
1. Open-source Community Contributions: Actively contributing to the open-source community on platforms like [GitHub](https://github.com/albert-jin/) and [other Internet platforms](https://github.com/albert-jin/FintechKP-frontend/), currently with over **300+** stars, wathcings and forks;
1. Review Contributions: Serving as a reviewer for multiple renowned international journals and conferences about Artificial Intelligence, reviewing dozens of articles;
1. Skills and Hobbies: Rich project experience, proficient in programming, passionate about scientific research, enthusiastic about fitness, interested in photography, and love traveling.

------
**School Honors**

- Undergraduate Academic Scholarship: First Prize twice, Second Prize twice;

- Graduate Academic Scholarship: First Prize once, Second Prize once;

- Outstanding Graduate Commendation Award in doctoral study;

- National Scholarship for PhD studies once.

------
**Internship Experiences**

+ Front-end Software Engineer
: Front-end interface development, maintenance and optimization of IaSS infrastructure, and back-end Python application development, eBay for foreign trade Corporation, Shanghai, Jan 2021 - Jun 2021.

+ Unity3D and Python Software Development Engineer
: Participate in frontend scene development for e-commerce platforms, as well as lead the backend application and user barrage management and monitoring, Shanghai Youhao Network Technology Co., Ltd, Shanghai, May 2022 - Sep 2022.

------
**Open-source Community Contributions**

My [GitHub](https://github.com/albert-jin/) Homepage.
![GitHub Main page of albert-jin until 2024-02-22.](/images/github-main-page.JPG)

------
**Review Contributions**

I have served as a reviewer for <span style="color: red; font-size: large;">multiple international journals and conferences</span>, including:

* Journals: [Information Fusion](https://www.sciencedirect.com/journal/information-fusion), [Expert Systems With Applications](https://www.sciencedirect.com/journal/expert-systems-with-applications), [Knowledge-Based Systems](https://www.sciencedirect.com/journal/knowledge-based-systems), [Information Processing & Management](https://www.sciencedirect.com/journal/information-processing-and-management), [Artificial Intelligence Review](https://link.springer.com/journal/10462) , [Recent Advances in Electrical & Electronic Engineering
](https://benthamscience.com/public/journals/recent-advances-in-electrical-and-electronic-engineering), [Plos One](https://journals.plos.org/plosone/), [IEEE Transactions on Knowledge and Data Engineering](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=69), [Resources, Conservation & Recycling](https://www.sciencedirect.com/journal/resources-conservation-and-recycling), [Frontiers in Artificial Intelligence](https://www.frontiersin.org/journals/artificial-intelligence), [Artificial Intelligence Review](https://link.springer.com/journal/10462), [Web Intelligence](https://www.iospress.com/catalog/journals/web-intelligence), [Data Mining and Knowledge Discovery](https://link.springer.com/journal/10618), [ISA Transactions](https://www.sciencedirect.com/journal/isa-transactions), [International Journal of Intelligent Systems](https://onlinelibrary.wiley.com/journal/1098111x), [Journal of Advanced Research in Applied Sciences and Engineering Technology](https://semarakilmu.com.my/journals/index.php/applied_sciences_eng_tech/index), [Natural Language Processing Journal](https://www.sciencedirect.com/journal/natural-language-processing-journal), [Qeios](https://www.qeios.com/) and so on.

* Conferences: [CogSci 2024](https://cognitivesciencesociety.org/), [MIDL 2024](https://2024.midl.io/), and so on.

![My experience in peer reviewing.](/images/reviewer.JPG)

------

Chinese Invention Patents
======
- 一种基于多维度焦点问题生成的谣言检测数据增强方法及装置. (独立一作) 
<br>
<span style="font-size: large;">A rumor detection data augmentation method and device based on multi-dimensional focus issue generation. (sole first author)</span>
<span style="color: red; font-size: medium;">(During qualification examination...)</span>

- 一种借助谣言检测任务数据增强的少样本监督中文事实核查方法. (独立一作)
<br>
<span style="font-size: large;">A few-shot supervised Chinese fact-checking method aided by rumor detection task data augmentation. (sole first author)</span>
<span style="color: red; font-size: medium;">(During qualification examination...)</span>

- 一种大语言模型驱动知识图谱多跳推理的军事问答方法与系统. (独立一作)
<br>
<span style="font-size: large;">A military question-answering method and system driven by large language model-enabled knowledge graph multi-hop reasoning. (sole first author)</span>
<span style="color: red; font-size: medium;">(During qualification examination...)</span>

- 一种基于大语言模型的具身多智能体协同博弈决策方法. (独立一作)
<br>
<span style="font-size: large;">A multi-agent cooperative decision-making method based on large language model-driven embodied intelligent agents. (sole first author)</span>
<span style="color: red; font-size: medium;">(During qualification examination...)</span>

- 一种大语言模型驱动的具身智能体零样本目标导航方法. (独立一作)
<br>
<span style="font-size: large;">A zero-shot target navigation method driven by large language model-enabled embodied intelligent agents. (sole first author)</span>
<span style="color: red; font-size: medium;">(During qualification examination...)</span>

- 一种基于焦点注意网络增强的海陆空微小目标检测方法. (独立一作)
<br>
<span style="font-size: large;">A tiny target detection method based on enhanced attention networks for sea, land, and air. (sole first author)</span>
<span style="color: red; font-size: medium;">(During qualification examination...)</span>

- 基于人类模糊直觉驱动的关键目标定位与分割方法与系统. (除一老师外一作)
<br>
<span style="font-size: large;">A method and system for key target localization and segmentation driven by human fuzzy intuition. (except a teacher from Northwestern Polytechnical University, sole first author)</span>
<span style="color: red; font-size: medium;">(During qualification examination...)</span>

Works in Submission
------
<!--[KR 2024](https://kr.org/KR2024/)--> <!-- Bridging Rumor Detection and Fact Verification through Cross-Task Linguistic Synergies -->
* UniFake: Bridging Rumor Detection and Fact Verification through Cross-Task Linguistic Synergies for Fake News Identification. ([ICASSP 2025](https://2025.ieeeicassp.org/) Under Review.) 

<!--* Can Rumor Detection Enhance Fact Verification? Unraveling Cross-Task Synergies Between Rumor Detection and Fact Verification. ([IEEE Transactions on Big Data](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=6687317) Under Review.)-->

<!--* DisCo-FEND: Social Context Veracity Dissemination Consistency-Guided Case Reasoning for Few-Shot Fake News Detection. ([ISWC 2024](https://iswc2024.semanticweb.org/) Under Review.)-->

* PMTL-DisCo: A Prompting MulTi-task Learning-based Veracity Dissemination Consistency Reasoning Augmentation for Few-Shot Fake News Detection ([Neurocomputing](https://www.sciencedirect.com/journal/neurocomputing) Under Review.)

<!--* A veracity dissemination consistency-based few-shot fake news detection framework by synergizing adversarial and contrastive self-supervised learning (Writing...)-->

<!--% [ECAI](https://www.ecai2024.eu/calls/main-track)-->

* Self-adaptive LLM instructions optimization for aspect-based sentiment analysis by incorporating emotion-oriented in-contexts. ([Computational Intelligence](https://onlinelibrary.wiley.com/journal/14678640) Under Review.)

Works in Conducting
------
* A Comprehensive Survey on Multi-Agent Cooperative Decision-Making Scenarios, Approaches, Challenges and Perspectives. ([Artificial Intelligence Review](https://link.springer.com/journal/10462) Preparing for.) 

TBD
------
.

Some Secrets
------
The following are some of secrets. 🙊🙊🙊 <a href="#secret-access-enter">(Need Secret Access)</a>

<div class="SecretContainer" style="display: none;">
    <!-- <img src="/images/secrets/lifephotos/eating.jpg" alt="beauty life image show 1.">
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
    <img src="/images/secrets/lifephotos/slim.jpg" alt="beauty life image show 5."> -->
    <img src="/images/secrets/secret-tbd.jpg" alt="Secret-TBD.">
    <br/>
    <br/>
    <!-- <img src="/images/secrets/XXX.jpg" alt="XXX."> -->
</div>

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
