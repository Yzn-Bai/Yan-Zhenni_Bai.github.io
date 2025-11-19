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
  <span style="color:green; font-weight: bold;">Connected and automated vehicles (CAVs)</span> are anticipated to play a central role in future road transport systems, enabling precise car-following, cooperative platoon formation, and vehicle–infrastructure coordination. These capabilities have the potential to enhance the efficiency and stability of mixed traffic streams.

 <div style="text-align: center;">
   <img src="images/3lane.jpg" alt="TRB Conference Poster" style="max-width: 80%;">
   </div>
  
  <span style="color:green; font-weight: bold;">Dedicated lanes (DLs)</span> for CAVs have therefore been proposed as a promising strategy to segregate CAVs from human-driven vehicles (HVs), mitigate traffic shockwaves, and better harness the capabilities of CAV technologies. By facilitating more homogeneous CAV flows with prioritized right-of-way, CAV DLs have the potential to increase effective roadway capacity, dampen traffic oscillations, and improve operational safety, while providing a controlled environment for deploying advanced control strategies and vehicle–infrastructure coordination schemes. The extent of these benefits, however, critically depends on lane management policies, CAV market penetration, and traffic demand.

  <div style="text-align: center;">
    <img src="images/3lane1dl.jpg" alt="TRB Conference Poster" style="max-width: 80%;">
    </div>
  
  In this context, the <span style="color:green; font-weight: bold;">cell transmission model (CTM)</span> provides an attractive mesoscale modeling tool, as it links both macroscopic and microscopic traffic dynamics. It captures key features such as capacity drop, shockwave propagation, and lane interactions while maintaining a lower computational cost. Lane-level extensions of the CTM enable an explicit representation of CAV DLs and mixed-traffic interactions, making it well suited for systematic evaluation and optimization of CAV DL deployment schemes on freeways under varying demand levels and market penetration rates.

Optimization of DL Configuration for CAVs in Mixed Traffic Environments
------

  This study constructs a <span style="color:blue; font-weight: bold;">fundamental diagram model</span> that reflects both heterogeneous and homogeneous traffic flows by distinguishing among different car-following modes, characterized by varying desired headways and reaction times. 
  
  To simulate <span style="color:blue; font-weight: bold;">lane-changing behavior</span> for both vehicle types, the framework further embeds <span style="color:blue; font-weight: bold;">a logit model</span>, which takes into account the traffic occupancy rate and other latent factors influencing lane-changing decisions.

  Additionally, the modeling framework explicitly incorporates the capacity drop phenomenon, where the flow rate decreases and impacts overall capacity when traffic density exceeds a critical threshold.

<div style="text-align: center;">
  <img src="images/基本图2.png" alt="First Image" style="width: 45%; display:inline-block;">
  <img src="images/接收发送能力.png" alt="Second Image" style="width: 45%; display:inline-block;">
  </div>

  Through these extensions, the traditional CTM is modified to better capture the unique dynamics introduced by CAVs and DLs, thereby improving the simulation capability of CAV DL performance in mixed traffic environments.
  
  Within this framework, the CAV DL configurations such as the <span style="color:blue; font-weight: bold;">number</span>, <span style="color:blue; font-weight: bold;">length</span>, and <span style="color:blue; font-weight: bold;">position</span> are examined with respect to improvements in efficiency and utility at the corridor level. Selected numerical results are presented below.

- CAV DL numbers (presence vs absence)

<div style="text-align: center;">
  <img src="images/有无专用道的流量差.png" alt="First Image" style="width: 45%; display:inline-block;">
  <img src="images/1b.png" alt="Second Image" style="width: 45%; display:inline-block;">
  </div>
  
<div style="text-align: center;">
  <img src="images/fig1c.png" alt="Image 1" style="width: 45%; display:inline-block;">
  </div>

- Horizontal position of CAV DLs (with/without speed-limit differences)

<div style="text-align: center;">
  <img src="images/无限速区别时，专用道设置在边缘时与设置在中间时的一小时流量差.png" alt="Image 1" style="width: 45%; display:inline-block;">
</div>

<div style="text-align: center;">
  <img src="images/有限速时，专用道位置1-2流量差.png" alt="First Image" style="width: 45%; display:inline-block;">
  <img src="images/有限速时，专用道位置1-3流量差.png" alt="Second Image" style="width: 45%; display:inline-block;">
  </div>

- CAV DL length effects

<div style="text-align: center;">
  <img src="images/error_line.png" alt="First Image" style="width: 45%; display:inline-block;">
  <img src="images/d=1500&d=2000.png" alt="Second Image" style="width: 45%; display:inline-block;">
  </div>
  
- Longitudinal position of CAV DLs (placement vs incident location)

<div style="text-align: center;">
  <img src="images/d=2000,p=0.3,1.png" alt="First Image" style="width: 45%; display:inline-block;">
  <img src="images/d=2000,p=0.3,2.png" alt="Second Image" style="width: 45%; display:inline-block;">
  </div>

<div style="text-align: center;">
  <img src="images/d=2000,p=0.3,3.png" alt="First Image" style="width: 45%; display:inline-block;">
  <img src="images/d=2000,p=0.3,4.png" alt="Second Image" style="width: 45%; display:inline-block;">
  </div>

*Related findings have been presented as a poster at the 104th Transportation Research Board (TRB) Annual Meeting.*

<img src="images/TRB海报.png" alt="TRB Conference Poster" style="max-width: 100%;">

Reinforcement Learning-Based Dynamic Dedicated Lane Control for CAVs in Mixed Traffic (working paper)
------

  However, in the real world CAV penetration is highly uncertain, traffic demand fluctuates across time and space, and infrastructure budgets are constrained. Under such conditions, naively deploying or statically managing CAV DLs can even waste capacity or worsen congestion if the number, position, or length of DLs is not matched to prevailing traffic states. This creates an urgent need for mesoscale models and intelligent control methods that can further adapt DL allocation in real time as demand and CAV penetration evolve.

  <div style="text-align: center;">
    <img src="images/CTM-RL研究场景(CTS版)(1).png" alt="TRB Conference Poster" style="max-width: 80%;">
    </div>

  The capacity drop phenomenon is more extended which occurs when traffic density exceeds a critical threshold, leading to a reduction in flow capacity. And apply a simplified approach that captures the essential lane-changing behaviors while reducing computational complexity.

  <div style="text-align: center;">
    <img src="images/强化学习.png" alt="First Image" style="width: 45%; display:inline-block;">
    <img src="images/supply_receive_together.png" alt="Second Image" style="width: 45%; display:inline-block;">
  </div>

  The control problem is framed as a <span style="color:blue; font-weight: bold;">Markov Decision Process (MDP)</span>, where the <span style="color:blue; font-weight: bold;">state space</span> incorporates key factors such as segment-level traffic density and CAV penetration rate, the <span style="color:blue; font-weight: bold;">action space</span> represents the number of DLs, and the <span style="color:blue; font-weight: bold;">reward function</span> is based on improvements in macroscopic traffic efficiency. To ensure training stability and efficiency, an <span style="color:blue; font-weight: bold;">early-stopping mechanism</span> is introduced, helping to balance the trade-off between training time and convergence.

  <div style="text-align: center;">
    <img src="images/reward_plot_3D.png" alt="Image 1" style="width: 45%; display:inline-block;">
    </div>

  <div style="text-align: center;">
    <img src="images/line_reward_mean_std_shaded_ok.png" alt="First Image" style="width: 45%; display:inline-block;">
    <img src="images/line_t_end_mean_std_shaded_ok.png" alt="Second Image" style="width: 45%; display:inline-block;">
    </div>
    
  <div style="text-align: center;">
    <img src="images/1.png" alt="TRB Conference Poster" style="max-width: 100%;">

    <img src="images/2.png" alt="TRB Conference Poster" style="max-width: 100%;">

    <img src="images/3.png" alt="TRB Conference Poster" style="max-width: 100%;">
    </div>
  
Awards
======

- Master Student Academic Scholarship, Beijing University of Technology

- Science and Technology Innovation Award, Beijing University of Technology

- Excellent Student, Beijing University of Technology

- Undergraduate Academic Scholarship, Inner Mongolia University

- Excellent Student, Inner Mongolia University
