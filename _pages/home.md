---
title: "SoftSec Lab - Home"
layout: homelay
excerpt: "SoftSec Lab at SKKU"
sitemap: false
permalink: /
---
The Software Security Lab (SoftSec) at Sungkyunkwan University conducts research at the intersection of <b>Artificial Intelligence, Software Engineering, and Security.</b><br> 

The rapid advancement of AI, particularly large language models (LLMs) and autonomous AI agents, is transforming how software systems are developed, analyzed, and operated. While these advances create new opportunities for software engineering, they also introduce new challenges in understanding, testing, and securing increasingly complex systems.<br>

Our goal is to develop foundational principles and practical techniques for understanding, engineering, and securing software and AI systems. We aim to leverage AI to advance software engineering while applying rigorous software analysis, testing, and security techniques to improve the reliability and trustworthiness of AI systems.<br>

<div markdown="0" id="carousel" class="carousel slide" data-ride="carousel" data-interval="5000" data-pause="hover" >
    {% assign number_printed = 0 %}
    <ol class="carousel-indicators">
    {% for slider in site.data.main_slider %}
        {% if number_printed == 0 %}
            <li data-target="#carousel" data-slide-to="0" class="active"></li>
        {% else %}
            <li data-target="#carousel" data-slide-to="{{number_printed}}"></li>
        {% endif %}
    {% assign number_printed = number_printed | plus: 1 %}
    {% endfor %}
    </ol>

    {% assign slider_printed = 0 %}
    <div class="carousel-inner" markdown="0">
        {% for slider in site.data.main_slider %}
            {% if slider_printed == 0 %}
            <div class="item active">
            {% else %}
            <div class="item">
            {% endif %}
                <img src="{{slider.url}}" height="700"/>
            </div>
        {% assign slider_printed = slider_printed | plus: 1 %}
        {% endfor %}
    </div>
  <a class="left carousel-control" href="#carousel" role="button" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" href="#carousel" role="button" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>

We are interested in the following research fields.

<ul>
<li>
<b>AI Security & Trustworthiness:</b> Developing techniques to identify vulnerabilities, evaluate and verify AI agent behaviors, and improve the security and trustworthiness of AI systems.
</li>

<li>
<b>AI for Software Engineering:</b> Leveraging AI and LLMs to advance program understanding, software development, vulnerability detection, and automated testing.
</li>

<li>
<b>Software & Systems Security:</b> Developing program analysis and testing techniques to discover vulnerabilities and investigate security challenges in real-world software, mobile, embedded, and on-device AI systems.
</li>
</ul>

<!--**We are looking for passionate new PhD/MS/undergraduate students to join our lab!**-->
**Joining the Lab**<br>
Software Security Lab(SoftSec)에서는 **인공지능(AI), 소프트웨어 공학(Software Engineering), 보안(Security)**의 융합 분야에서 함께 연구할 대학원생 및 학부연구생을 모집합니다. <br>

최근 대규모 언어모델(LLM)과 AI Agent의 발전은 소프트웨어의 개발과 분석 방식을 변화시키는 동시에 새로운 보안 및 신뢰성 문제를 만들어내고 있습니다. 저희 연구실은 AI를 활용하여 소프트웨어를 보다 효과적으로 이해하고 개발하는 기술과, 소프트웨어 분석·테스팅·보안 기술을 활용하여 AI 및 실제 시스템의 신뢰성을 높이는 기술을 연구하고 있습니다. <br>

주요 연구 분야는 다음과 같습니다.

**1. AI Security & Trustworthiness:** AI Agent의 취약점 분석, 테스팅 및 행동 검증, AI 시스템의 안전성과 신뢰성 평가, Machine Unlearning 등<br>

**2. AI for Software Engineering:** LLM 및 AI Agent를 활용한 소프트웨어 개발 자동화, 취약점 및 버그 탐지, 프로그램 이해를 위한 코드 표현 및 프로그래밍 언어 설계 등<br>

**3. Software & Systems Security:** 프로그램 분석과 소프트웨어 테스팅을 통한 취약점 탐지, 모바일·임베디드·온디바이스 AI 시스템 보안, 실제 시스템 해킹 및 실증 연구 등<br>

AI, 소프트웨어 공학, 시스템 보안 분야의 새로운 문제를 발견하고 해결하는 데 관심 있는 학생 및 연구자들의 많은 지원을 바랍니다.
email: sungjaeh@skku.edu

<!--
<figure class="fourth">
  <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/Logo_Leiden.jpg" style="width: 210px">
  <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/Logo_Nanofront.jpg" style="width: 110px">
  <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/Logo_NWO.jpg" style="width: 120px">
  <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/Logo_ERC.jpg" style="width: 110px">
</figure>
-->
