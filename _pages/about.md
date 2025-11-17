---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi! Welcome to my homepage 👋 I’m Yan-Zhenni Bai(白岩珍妮), an M.Eng. student in Transportation at Beijing University of Technology. My current research focuses on mixed traffic flow with **connected and autonomous vehicles**, **dedicated lane management**, and **reinforcement learning** for dynamic control and optimization. I am passionate about using quantitative methods and simulation to improve the efficiency and safety of highway and urban road networks.

Education
======
- M.S., Transportation, Beijing University of Technology, Sep. 2023 - present
- B.S., Transportation, Inner Mongolia University, Sep. 2018-Jul. 2022

Research Interests
======
- Connected and autonomous vehicles and their integration into large-scale transportation systems
- Data-driven modeling, generative AI and reinforcement learning for optimization, prediction and control in intelligent transportation systems
- Mixed traffic flow modeling using traffic flow theory(car-following model, cellular au-tomata, cell-transmission model)

Research Highlight
======
  <span style="color:green; font-weight: bold;">Connected and automated vehicles (CAVs)</span> are expected to be a key component of future road traffic, enabling precise car-following, platooning, and vehicle-infrastructure cooperation. These capabilities can significantly enhance traffic efficiency and safety in mixed environments.
  
  <span style="color:green; font-weight: bold;">Dedicated lanes (DLs)</span> for CAVs have therefore emerged as a crucial strategy to segregate CAVs from human-driven vehicles (HVs), mitigate shockwaves, and fully exploit CAV potential. By forming homogeneous CAV streams with exclusive right-of-way, CAV DLs can increase roadway capacity, stabilize traffic flow, and create a safer operating environment with fewer disturbances from human driving, while also providing a platform for advanced control strategies and vehicle-infrastructure coordination.
  
  In this context, the <span style="color:green; font-weight: bold;">cell transmission model (CTM)</span> provides an attractive mesoscale modeling tool, as it links both macroscopic and microscopic traffic dynamics. It captures key features such as capacity drop, shockwave propagation, and lane interactions while maintaining a lower computational cost compared to full microscopic simulations. Its lane-level extension allows explicit representation of CAV dedicated lanes and mixed-traffic interactions, making it well suited for systematic evaluation and optimization of CAV DL deployment schemes on freeways.
  
Optimization of Dedicated Lane Configuration for CAVs in Mixed Traffic Environments
------

  This study constructs a <span style="color:blue; font-weight: bold;">fundamental diagram model</span> that reflects both heterogeneous and homogeneous traffic flows by distinguishing between different car-following modes, with considerations for headway and reaction times. The model accurately captures the dynamic characteristics of mixed traffic flows by accounting for the differences between CAVs and HVs.

  To simulate <span style="color:blue; font-weight: bold;">lane-changing behavior</span> for both vehicle types, this study also incorporates <span style="color:blue; font-weight: bold;">a logit model</span>, which takes into account the traffic occupancy rate and other latent factors influencing lane-changing decisions.

  Additionally, the model considers the capacity drop phenomenon, where the flow rate decreases and impacts overall capacity when traffic density exceeds a critical threshold.

  <img src="images/基本图2.png" alt="First Image" style="width: 45%; display:inline-block;">
  <img src="images/接收发送能力.png" alt="Second Image" style="width: 45%; display:inline-block;">

  Through these enhancements, the traditional CTM is modified to better capture the unique dynamics introduced by CAVs and DLs, thereby improving the simulation capability of CAV DL performance in mixed traffic environments.
  
  Well-designed CAV DL configurations such as <span style="color:blue; font-weight: bold;">number</span>, <span style="color:blue; font-weight: bold;">length</span>, and <span style="color:blue; font-weight: bold;">position</span> are therefore crucial for realizing system-level benefits from CAV technologies, ensuring that the substantial investments in automation and connectivity translate into tangible improvements in efficiency, reliability, and safety at the corridor and network levels.

- CAV DL numbers

  <img src="images/有无专用道的流量差.png" alt="First Image" style="width: 45%; display:inline-block;">
  <img src="images/1b.png" alt="Second Image" style="width: 45%; display:inline-block;">
  
  ![]("images/fig1c.png")

- Horizontal position of CAV DLs

  ![]("images/无限速区别时，专用道设置在边缘时与设置在中间时的一小时流量差.png")

  <img src="images/有限速时，专用道位置1-2流量差.png" alt="First Image" style="width: 45%; display:inline-block;">
  <img src="images/有限速时，专用道位置1-3流量差.png" alt="Second Image" style="width: 45%; display:inline-block;">

- 

  *Related research findings have been reported at the 105th Transportation Research Board (TRB) Annual Metting*
  
Reinforcement Learning-Based Dynamic Dedicated Lane Control for CAVs in Mixed Traffic (working paper)
------

  However, in the real world CAV penetration is highly uncertain, traffic demand fluctuates across time and space, and infrastructure budgets are constrained. Under such conditions, naively deploying or statically managing CAV DLs can even waste capacity or worsen congestion if the number, position, or length of DLs is not matched to prevailing traffic states. This creates an urgent need for mesoscale models and intelligent control methods that can further adapt DL allocation in real time as demand and CAV penetration evolve.

  The capacity drop phenomenon is more extended which occurs when traffic density exceeds a critical threshold, leading to a reduction in flow capacity. And apply a simplified approach that captures the essential lane-changing behaviors while reducing computational complexity.

  The control problem is framed as a <span style="color:blue; font-weight: bold;">Markov Decision Process (MDP)</span>, where the <span style="color:blue; font-weight: bold;">state space</span> incorporates key factors such as segment-level traffic density and CAV penetration rate, the <span style="color:blue; font-weight: bold;">action space</span> represents the number of DLs, and the <span style="color:blue; font-weight: bold;">reward function</span> is based on improvements in macroscopic traffic efficiency. To ensure training stability and efficiency, an <span style="color:blue; font-weight: bold;">early-stopping mechanism</span> is introduced, helping to balance the trade-off between training time and convergence.

Awards
======

- Master Student Academic Scholarship, Beijing University of Technology

- Science and Technology Innovation Award, Beijing University of Technology

- Excellent Student, Beijing University of Technology

- Undergraduate Academic Scholarship, Inner Mongolia University

- Excellent Student, Inner Mongolia University
