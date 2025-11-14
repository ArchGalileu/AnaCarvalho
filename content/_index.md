---
title: "Guided Tours in Soajo & Parque Peneda Gerês"
date: 2025-01-01
type: landing

design:
  spacing: "6rem"

sections:
  - block: hero
    content:
      title: "Discover Our Guided Tours"
      text: "Experience the breathtaking landscapes of Soajo and Parque Nacional Peneda Gerês with our expertly guided tours. Our experienced local guides will lead you through the most spectacular natural attractions."
      primary_action:
        text: "Book a Tour"
        url: "/tour"
      secondary_action:
        text: "Learn More"
        url: "/about"
    design:
#      css_class: "bg-gradient-to-br from-green-50 to-blue-50 dark:from-gray-900 dark:to-gray-800"
      background:
        video:
          # Name of video in `assets/media/`.
          filename: background-video.mp4
          # Post-processing: flip the video horizontally?
          flip: false
  - block: collection
    content:
      title: "Available Tours"
      text: "Explore our curated selection of guided tours in Soajo and Parque Peneda Gerês."
      # Filter tour content
      filters:
        folders:
          - tour
        exclude_drafts: true
      # Choose how many cards to display
      count: 10
    design:
      view: card
      spacing:
        padding: ["4rem", 0, "4rem", 0]

  - block: cta-card
    content:
      title: "Ready for Adventure?"
      text: "Book your guided tour today and immerse yourself in the natural beauty of Soajo and Parque Peneda Gerês."
      button:
        text: "Contact Us"
        url: "/contact/"
    design:
      card:
        css_class: "bg-primary-600 text-white"
---
