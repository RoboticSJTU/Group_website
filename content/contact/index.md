---
title: Contact
date: 2025-05-06

type: landing

sections:
  - block: contact
    content:
      title: Contact
      text: |-
        The research group is currently recruiting undergraduate interns and Master's program applicants for 2025 enrollment. Please send your CV to: cai_panpan@sjtu.edu.cn
      email: cai_panpan@sjtu.edu.cn
      address:
        street: 730 Jianchuan Road
        city: Shanghai
        region: Shanghai
        postcode: '200000'
        country: China
        country_code: CN
      coordinates:
        latitude: '31.02780868667594'
        longitude: '121.42237926755062'
      directions: Enter Building A and take the elevator to Office 314 on Floor 3
      #contact_links:
      #  - icon: comments
      #    icon_pack: fas
      #    name: Discuss on Forum
      #    link: 'https://discourse.gohugo.io'
    
      # Automatically link email and phone or display as text?
      autolink: true
    
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '1'

  - block: markdown
    content:
      title:
      subtitle: ''
      text:
    design:
      columns: '1'
      background:
        image: 
          filename: contact.jpg
          filters:
            brightness: 1
          parallax: false
          position: center
          size: cover
          text_color_light: true
      spacing:
        padding: ['20px', '0', '20px', '0']
      css_class: fullscreen
---
