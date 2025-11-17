---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi! Welcome to my homepage 👋 I’m Yan-Zhenni Bai, an M.Eng. student in Transportation at Beijing University of Technology. My current research focuses on mixed traffic flow with connected and autonomous vehicles, dedicated lane management, and reinforcement learning for dynamic control and optimization. I am passionate about using quantitative methods and simulation to improve the efficiency and safety of highway and urban road networks.

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
  Connected and automated vehicles (CAVs) are expected to become a dominant component of future road traffic, offering precise car-following, platooning, and vehicle–infrastructure cooperation that can significantly enhance capacity, stability, and safety in mixed traffic. Dedicated lanes (DLs) for CAVs have therefore emerged as a key management strategy to segregate CAVs from human-driven vehicles (HVs), mitigate shockwaves, and fully exploit CAV capabilities. By aggregating CAVs into homogeneous streams with exclusive right-of-way, CAV DLs can increase effective roadway capacity, stabilize traffic flow, and provide a safer operating environment with fewer disturbances from imperfect human driving. In addition, CAV DLs create a favorable platform for deploying advanced control strategies and vehicle–infrastructure coordination, because traffic conditions within these lanes are more predictable and easier to model.
  In this context, the cell transmission model (CTM) provides an attractive mesoscale modeling tool, as it links both macroscopic and microscopic traffic dynamics. It captures key features such as capacity drop, shockwave propagation, and lane interactions while maintaining a lower computational cost compared to full microscopic simulations. Its lane-level extension allows explicit representation of CAV dedicated lanes and mixed-traffic interactions, making it well suited for systematic evaluation and optimization of CAV DL deployment schemes on freeways.
- Optimization of Dedicated Lane Configuration for CAVs in Mixed Traffic Environments
  This study constructs a fundamental diagram model that reflects both heterogeneous and homogeneous traffic flows by distinguishing between different car-following modes, with considerations for headway and reaction times. The model accurately captures the dynamic characteristics of mixed traffic flows by accounting for the differences between Connected and Automated Vehicles (CAVs) and Human-Driven Vehicles (HVs). To simulate lane-changing behavior for both vehicle types, this study also incorporates a logit model, which takes into account the traffic occupancy rate and other latent factors influencing lane-changing decisions. Additionally, the model considers the capacity drop phenomenon, where the flow rate decreases and impacts overall capacity when traffic density exceeds a critical threshold. Through these enhancements, the traditional Cell Transmission Model (CTM) is modified to better capture the unique dynamics introduced by CAVs and Dedicated Lanes (DLs), thereby improving the simulation capability of CAV DL performance in mixed traffic environments.
  
  Well-designed CAV DL configurations such as number, length, and position are therefore crucial for realizing system-level benefits from CAV technologies, ensuring that the substantial investments in automation and connectivity translate into tangible improvements in efficiency, reliability, and safety at the corridor and network levels.
  
- Reinforcement Learning-Based Dynamic Dedicated Lane Control for CAVs in Mixed Traffic (working paper)
  However, in the real world CAV penetration is highly uncertain, traffic demand fluctuates across time and space, and infrastructure budgets are constrained. Under such conditions, naively deploying or statically managing CAV DLs can even waste capacity or worsen congestion if the number, position, or length of DLs is not matched to prevailing traffic states. This creates an urgent need for mesoscale models and intelligent control methods that (i) can efficiently evaluate CAV DL configurations under heterogeneous mixed-traffic conditions, and (ii) can further adapt DL allocation in real time as demand and CAV penetration evolve.

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one Markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a Markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each Markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

The repository includes [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual Markdown files that will be properly formatted for the Academic Pages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the Markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and Markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a Markdown file for a talk
![Editing a Markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/), the [growing wiki](https://github.com/academicpages/academicpages.github.io/wiki), and you can always [ask a question on GitHub](https://github.com/academicpages/academicpages.github.io/discussions). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
