---
permalink: /
title: "Scott (Seongwon) Lee"
author_profile: false   # profile shown in the home header
redirect_from: 
  - /about/
  - /about.html
---

{% assign author = site.author %}
<header class="home-hero">
  <img class="home-hero-photo" src="{{ author.avatar | prepend: '/images/' | relative_url }}" alt="{{ author.name }}">
  <div class="home-hero-content">
    <h1 class="home-hero-name">{{ author.name }}</h1>
    <p class="home-hero-bio">Ph.D. Candidate &middot; Robotics<br>University of Illinois Urbana-Champaign</p>
    <ul class="home-hero-links">
      {% if author.email %}<li><a href="mailto:{{ author.email }}"><i class="fas fa-fw fa-envelope" aria-hidden="true"></i> Email</a></li>{% endif %}
      {% if author.googlescholar %}<li><a href="{{ author.googlescholar }}"><i class="ai ai-google-scholar" aria-hidden="true"></i> Google Scholar</a></li>{% endif %}
      {% if author.linkedin %}<li><a href="https://www.linkedin.com/in/{{ author.linkedin }}"><i class="fab fa-fw fa-linkedin" aria-hidden="true"></i> LinkedIn</a></li>{% endif %}
      {% for link in site.data.navigation.main %}{% if link.title == "Resume" %}<li><a href="{{ link.url | relative_url }}"><i class="fas fa-fw fa-file-alt" aria-hidden="true"></i> Resume</a></li>{% endif %}{% endfor %}
    </ul>
    <p class="home-hero-availability"><mark>Open to full-time opportunities</mark> &middot; <a href="mailto:{{ author.email }}">Get in touch</a></p>
  </div>
</header>

<aside class="demo-rail" aria-label="Interactive demo">
  <a class="demo-shortcut" href="https://sl148.github.io/reconfigurable-factory-demo/">
    <span class="demo-shortcut-label">Interactive demo <span aria-hidden="true">&#8599;</span></span>
    <span class="demo-shortcut-title">Reconfigurable <span class="demo-lego-label">LEGO <svg class="demo-lego-brick" viewBox="0 0 24 18" aria-hidden="true" focusable="false"><path fill="#b32624" d="M2 7h20v9H2z"/><path fill="#e4443e" d="M2 7l4-3h16v9l-4 3V7z"/><path fill="#f05a50" d="M2 7l4-3h16l-4 3z"/><path fill="#cf3530" d="M5 2h5v4H5zm9 0h5v4h-5z"/><ellipse cx="7.5" cy="2" rx="2.5" ry="1.3" fill="#f36a60"/><ellipse cx="16.5" cy="2" rx="2.5" ry="1.3" fill="#f36a60"/></svg></span> Factory</span>
    <picture class="demo-preview">
      <source media="(prefers-reduced-motion: reduce)" srcset="{{ '/images/reconfigurable_factory_demo.png' | relative_url }}">
      <img src="{{ '/images/workcell_clip.gif' | relative_url }}" alt="Robot arms assembling LEGO in a workcell">
    </picture>
  </a>
</aside>

<div class="intro">
  <p>I study <strong>task and motion planning, multi-robot systems, and agentic systems</strong> with <a href="https://siebelschool.illinois.edu/about/people/all-faculty/namato">Nancy M. Amato</a> at UIUC&nbsp;<img class="inline-logo" src="{{ '/images/uiuc_logo.png' | relative_url }}" alt="">.</p>
  <p>Previously, as a Ph.D. Resident at <a href="https://x.company/">X, the Moonshot Factory</a>&nbsp;<img class="inline-logo" src="{{ '/images/moonshot.png' | relative_url }}" alt="">, I worked on wet-lab automation with robotics and multi-agent LLMs. I earned my bachelor&rsquo;s in Mechanical Engineering at Yonsei University&nbsp;<img class="inline-logo" src="{{ '/images/yonsei_logo.png' | relative_url }}" alt=""> (2021), advised by <a href="https://mlcs.yonsei.ac.kr/Professor.html">Jongeun Choi</a>.</p>
</div>

<!-- News
------  -->

## Research

<div class="entries entries--research">
  <!-- ### Lazy-DaSH -->
  <div class="entry">
    <div class="entry-thumb"><img src="../images/lazydash.gif" alt="Lazy-DaSH Image"></div>
    <div class="entry-body">
      <div class="entry-title">Lazy-DaSH: Lazy Approach of Hypergraph-based Multi-robot Task and Motion Planning</div>
      <div class="entry-authors"><strong>Seongwon Lee</strong>, James Motes, Isaac Ngui, Marco Morales, Nancy M. Amato</div>
      <div class="entry-meta">
        <a class="entry-venue" href="https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=8860">IEEE Transactions on Robotics (T-RO), 2026</a>
        <span class="entry-links">
          <a href="../files/lazy_hype_tro_arxiv.pdf">Paper</a>
          <a href="https://arxiv.org/abs/2504.05552">arXiv</a>
          <a href="../files/ICRA@40_poster.pdf">Poster</a>
          <a href="https://drive.google.com/file/d/1T53N-vW6U0LH1WA1w9WLaOhstgMNJTP8/view?usp=sharing">Simulation</a>
          <a href="https://drive.google.com/file/d/1fAJ8TNFg8BKuut13hG3sdsWv_wC8lJcw/view?usp=sharing">Hardware Exp.</a>
        </span>
      </div>
    </div>
  </div>
  <!-- ### Reconfigurable Factory -->
  <div class="entry">
    <div class="entry-thumb"><img src="../images/Task_assignment.png" alt="Reconfigurable Factory Image"></div>
    <div class="entry-body">
      <div class="entry-title">A Hierarchical Approach to Workstation-based Task Allocation and Motion Planning</div>
      <div class="entry-authors"><strong>Seongwon Lee</strong>, James Motes, Isaac Ngui, Marco Morales, Nancy M. Amato</div>
      <div class="entry-meta">
        <a class="entry-venue" href="https://ieee-iros.org/">IROS 2023 Workshop</a>
        <span class="entry-links">
          <a href="../files/RAFF_2023_Submission.pdf">Paper</a>
          <a href="../files/IROS2023Poster.pdf">Poster</a>
          <a href="https://sl148.github.io/reconfigurable-factory-demo/">Interactive Demo</a>
        </span>
      </div>
    </div>
  </div>
  <!-- ### Quadrotor -->
  <div class="entry">
    <div class="entry-thumb"><img src="../images/quadrotor.gif" alt="Driving Image"></div>
    <div class="entry-body">
      <div class="entry-title">Output Feedback Control Design for Quadrotors Using Recursive Least Square Dynamic Inversion</div>
      <div class="entry-authors"><strong>Seongwon Lee</strong>, Joohwan Seo, Connor J. Boss, Joonho Lee, Jongeun Choi</div>
      <div class="entry-meta">
        <a class="entry-venue" href="https://www.sciencedirect.com/journal/mechatronics">Elsevier Mechatronics</a>
        <span class="entry-links">
          <a href="../files/Outputfeedbackcontroldesignforquadrotorusingrecursiveleast square dynamicinversion.pdf">Paper</a>
          <a href="https://youtu.be/ltcx1X3WuIU">YouTube</a>
        </span>
      </div>
    </div>
  </div>
  <!-- ### Helicopter -->
  <div class="entry">
    <div class="entry-thumb"><img src="../images/helicoptor.gif" alt="Driving Image"></div>
    <div class="entry-body">
      <div class="entry-title">Nonaffine Helicopter Control Design and Implementation Based on a Robust Explicit Nonlinear Model Predictive Control</div>
      <div class="entry-authors">Joohwan Seo, <strong>Seongwon Lee</strong>, Joonho Lee, Jongeun Choi</div>
      <div class="entry-meta">
        <a class="entry-venue" href="https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=87">IEEE Transactions on Control Systems Technology</a>
        <span class="entry-links">
          <a href="../files/NonaffineHelicopterControlDesignandImplementationBasedonaRobustExplicitNonlinearModelPredictiveControl.pdf">Paper</a>
          <a href="https://www.youtube.com/watch?v=aLQ-Ar9PMv4">YouTube</a>
        </span>
      </div>
    </div>
  </div>
  <!-- ### Driving -->
  <div class="entry">
    <div class="entry-thumb"><img src="../images/autonomous_driving.gif" alt="Quadrotor Image"></div>
    <div class="entry-body">
      <div class="entry-title">Unexpected Collision Avoidance Driving Strategy Using Deep Reinforcement Learning</div>
      <div class="entry-authors">Myunhoe Kim, <strong>Seongwon Lee</strong>, Jaehyun Lim, Jongeun Choi, Seong Gu Kang</div>
      <div class="entry-meta">
        <a class="entry-venue" href="https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=6287639">IEEE Access</a>
        <span class="entry-links">
          <a href="../files/UnexpectedCollisionAvoidanceDrivingStrategyUsingDeepReinforcementLearning.pdf">Paper</a>
        </span>
      </div>
    </div>
  </div>
</div>

## Projects

<div class="entries">
  <!-- ### Reconfigurable LEGO Factory demo -->
  <div class="entry entry--featured">
    <a class="entry-thumb" href="https://sl148.github.io/reconfigurable-factory-demo/"><picture><source media="(prefers-reduced-motion: reduce)" srcset="{{ '/images/reconfigurable_factory_demo.png' | relative_url }}"><img src="{{ '/images/workcell_clip.gif' | relative_url }}" alt="Reconfigurable LEGO Factory workcell demo"></picture></a>
    <div class="entry-body">
      <span class="entry-badge">Interactive demo</span>
      <div class="entry-title">Reconfigurable LEGO Factory: Interactive Web Demo</div>
      <p class="entry-desc">An interactive 3D factory where multi-arm workcells assemble LEGO models while mobile manipulators fetch bricks, planned by a hierarchy of order assignment (MILP), multi-robot task planning and multi-arm motion planning. Configure a workcell's robot arms yourself, or watch the factory run with a live Gantt chart.</p>
      <div class="entry-meta">
        <a class="entry-cta" href="https://sl148.github.io/reconfigurable-factory-demo/">Try the Demo</a>
      </div>
    </div>
  </div>
  <!-- ### Driving -->
  <div class="entry">
    <div class="entry-thumb"><img src="../images/MiV.gif" alt="Quadrotor Image"></div>
    <div class="entry-body">
      <!-- <p>In this section, provide details about your research on quadrotors, including any unique approaches, challenges, and achievements.</p> -->
      <div class="entry-title">Mind in Vitro (MiV)</div>
      <p class="entry-desc">Developing an robotics automation system for a biology lab, funded by National Science Foundation (NSF)</p>
      <div class="entry-skills">
        <span class="entry-skills-label">Skills</span>
        <img src="../icons/ros.png" alt="ROS Icon"><!-- <span>ROS</span> -->
        <img src="../icons/c++.png" alt="Python Icon"><!-- <span>C++</span> -->
        <img src="../icons/ephys.png" alt="Python Icon"><!-- <span>Open Ephys</span> -->
      </div>
      <div class="entry-meta">
        <span class="entry-links"><a href="https://mindinvitro.illinois.edu/">MiV</a></span>
      </div>
    </div>
  </div>
  <!-- ### Driving -->
  <div class="entry">
    <div class="entry-thumb"><img src="../images/EOH.gif" alt="Quadrotor Image"></div>
    <div class="entry-body">
      <!-- <p>In this section, provide details about your research on quadrotors, including any unique approaches, challenges, and achievements.</p> -->
      <div class="entry-title">Factory Automation Demo</div>
      <p class="entry-desc">Demonstrated a simple factory automation demo to pre-college students at the Engineering Open House (EOH) at UIUC</p>
      <div class="entry-skills">
        <span class="entry-skills-label">Skills</span>
        <img src="../icons/ros.png" alt="ROS Icon"><!-- <span>ROS</span> -->
        <img src="../icons/python.png" alt="Python Icon"><!-- <span>Python</span> -->
        <img src="../icons/ur.png" alt="Python Icon"><!-- <span>Universal Robot Arms</span> -->
        <img src="../icons/realsense.png" alt="Python Icon"><!-- <span>Universal Robot Arms</span> -->
      </div>
      <div class="entry-meta">
        <span class="entry-links"><a href="https://eohillinois.org/">EOH</a></span>
      </div>
    </div>
  </div>
  <!-- ### Driving -->
  <div class="entry">
    <div class="entry-thumb"><img src="../images/ECE470.gif" alt="Quadrotor Image"></div>
    <div class="entry-body">
      <!-- <p>In this section, provide details about your research on quadrotors, including any unique approaches, challenges, and achievements.</p> -->
      <div class="entry-title">Robotics Course Project: Handoff Operation for Mobile Manipulators</div>
      <p class="entry-desc">Designed a vision-based system for handoff operations between a workstation and a mobile manipulator</p>
      <div class="entry-skills">
        <span class="entry-skills-label">Skills</span>
        <img src="../icons/ros.png" alt="ROS Icon"><!-- <span>ROS</span> -->
        <img src="../icons/gazebo.png" alt="Python Icon"><!-- <span>Gazebo</span> -->
        <img src="../icons/python.png" alt="Python Icon"><!-- <span>Python</span> -->
      </div>
      <div class="entry-meta">
        <span class="entry-links"><a href="https://youtu.be/vK7W6ffZrBM">Youtube</a></span>
      </div>
    </div>
  </div>
  <!-- ### Driving -->
  <div class="entry">
    <div class="entry-thumb"><img src="../images/Robomaster.gif" alt="Quadrotor Image"></div>
    <div class="entry-body">
      <div class="entry-title">Robomaster AI Challenge ICRA2019</div>
      <p class="entry-desc">Implemented cooperative planning algorithms for fully autonomous combat robots (Achieved 3rd place)</p>
      <div class="entry-skills">
        <span class="entry-skills-label">Skills</span>
        <img src="../icons/ros.png" alt="ROS Icon"><!-- <span>ROS</span> -->
        <img src="../icons/gazebo.png" alt="Python Icon"><!-- <span>Gazebo</span> -->
        <img src="../icons/c++.png" alt="Python Icon"><!-- <span>C++</span> -->
        <img src="../icons/python.png" alt="Python Icon"><!-- <span>Python</span> -->
      </div>
      <div class="entry-meta">
        <span class="entry-links">
          <a href="https://www.robomaster.com/en-US">Robomaster AI Challenge</a>
          <a href="https://www.youtube.com/watch?v=oJdBfSafWjM">Youtube</a>
        </span>
      </div>
    </div>
  </div>
</div>

<!-- ### Driving -->
<!-- <div style="display: flex; flex-direction: row; align-items: flex-start; margin-bottom: 10px;">
  <div style="width: 30%; padding-right: 8px;">
    <img src="https://via.placeholder.com/150" alt="Quadrotor Image" style="max-width: 100%; height: auto;">
  </div>
  <div style="width: 70%; font-size: 15px;">
    <strong>BMW Korea Research Competition</strong><br>
    Myunhoe Kim, Seongwon Lee, Jaehyun Lim, Jongeun Choi, Seong Gu Kang<br>
    <a href="https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=6287639">[IEEE Access]</a> / <a href="https://icra40.ieee.org/">[Paper]</a> 
  </div>
</div> -->

<!-- Experience
------ -->

## Professional Service

- **Reviewer**
  - RAL, ICRA, IROS, WAFR (2022 - 2024)
- **Teaching & Mentoring**
  - **Research Program Mentor (CS)**, UIUC – Fall 2023, Summer 2024, Spring 2024
  - **Fluid Mechanics (ME 310)**, UIUC – Fall 2022, Spring 2024, Fall 2024
  - **Mathematical Methods (TAM 541)**, UIUC – Fall 2021
{: .service-list}

<!-- Contact
------ 
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/), the [growing wiki](https://github.com/academicpages/academicpages.github.io/wiki), and you can always [ask a question on GitHub](https://github.com/academicpages/academicpages.github.io/discussions). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful. -->
