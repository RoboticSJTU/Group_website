---
title: Tour
date: 2022-10-24

type: landing

sections:
  - block: slider
    content:
      slides:
        - title: 👋 Welcome to the Robot Planning and Learning group
          content: Take a look at what we're working on...
          align: center
          background:
            image:
              filename: ropl.jpg
              filters:
                brightness: 0.7
            position: right
            color: "#747474ff"
        - title: "PO-PDDL"
          content: "Learning Symbolic POMDPs from Visual Demonstrations for Robot Planning Under Uncertainty"
          align: top
          background:
            image:
              filename: popddl.png
              filters:
                brightness: 0.7
            position: center
            color: "#747474ff"
          link:
            url: "https://roboticsjtu.github.io/PO-PDDL/"
            text: Project Page
        - title: "TGPO"
          content: "Trace-Guided Policy Optimization for Robot Task Planning via Verifiable Subgoal Generation"
          align: top
          background:
            image:
              filename: tgpo.png
              filters:
                brightness: 0.7
            position: center
            color: "#747474ff"
          link:
            url: "https://tgpo2026.github.io/TGPO/"
            text: Project Page
        - title: "I-Perceive"
          content: "A Foundation Model for Vision-Language Active Perception"
          align: top
          background:
            image:
              filename: iperceive.jpg
              filters:
                brightness: 0.7
            position: center
            color: "#747474ff"
          link:
            url: "https://roboticsjtu.github.io/I-Perceive-Page/"
            text: Project Page

        - title: "Hi-Drive"
          content: "Hierarchical POMDP Planning for Safe Autonomous Driving in Diverse Urban Environments"
          align: top
          background:
            image:
              filename: hidrive.jpg
              filters:
                brightness: 0.7
            position: center
            color: "#747474ff"
        
        - title: "Vec-QMDP"
          content: "Vec-QMDP: Vectorized POMDP Planning on CPUs for Real-Time Autonomous Driving"
          align: top
          background:
            image:
              filename: vecqmdp.png
              filters:
                brightness: 0.7
            position: center
            color: "#747474ff"
          link:
            url: "https://sii-boluomonster.github.io/VecQMDP-website/"
            text: Project Page
    design:
      # Slide height is automatic unless you force a specific height (e.g. '400px')
      slide_height: ""
      is_fullscreen: true
      # Automatically transition through slides?
      loop: true
      # Duration of transition between slides (in ms)
      interval: 2000
---
