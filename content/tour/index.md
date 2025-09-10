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
          color: '#747474ff'
      - title: 'AHAT: Any House, Any Task Planning!'
        content: Long horizon embodied decision making using common sense.
        align: top
        background:
          image:
            filename: ahat.png
            filters:
              brightness: 0.7
          position: center
          color: '#747474ff'
      - title: 'Unidomain'
        content: 'Pretraining a Unified PDDL Domain from Real-World Demonstrations for Generalizable Robot Task Planning'
        align: top
        background:
          image:
            filename: unidomain.png
            filters:
              brightness: 0.7
          position: center
          color: '#747474ff'
        link:
          url: "https://unidomain.github.io/"
          text: Project Page

      - title: 'Tru-POMDP'
        content: 'Task Planning Under Uncertainty via Tree of Hypotheses and Open-Ended POMDPs'
        align: top
        background:
          image:
            filename: trupomdp.png
            filters:
              brightness: 0.7
          position: center
          color: '#747474ff'
        link:
          url: "https://tru-pomdp.github.io/"
          text: Project Page
      - title: 'Hi-Drive'
        content: 'Hierarchical POMDP Planning for Safe Autonomous Driving in Diverse Urban Environments'
        align: top
        background:
          image:
            filename: hidrive.jpg
            filters:
              brightness: 0.7
          position: center
          color: '#747474ff'
      - title: RoPL
        content: 'We are hiring!'
        align: right
        background:
          image:
            filename: welcome.png
            filters:
              brightness: 0.7
          position: center
          color: '#747474ff'
        link:
          icon: graduation-cap
          icon_pack: fas
          text: Join Us
          url: ../contact/
    design:
      # Slide height is automatic unless you force a specific height (e.g. '400px')
      slide_height: ''
      is_fullscreen: true
      # Automatically transition through slides?
      loop: true
      # Duration of transition between slides (in ms)
      interval: 2000
---
