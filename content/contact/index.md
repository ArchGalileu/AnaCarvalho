---
title: "Contact Us"
date: 2025-01-01
type: page

design:
  spacing: "6rem"

sections:
  - block: hero
    content:
      title: "Get in Touch"
      text: "Have questions about our guided tours? Want to book a tour in Soajo and Parque Peneda Gerês? Reach out to our team."
    design:
      css_class: "bg-gradient-to-br from-blue-50 to-indigo-50 dark:from-gray-900 dark:to-gray-800"

  - block: contact
    content:
      # Set the email form provider in `config/_default/params.yaml`:
      #   email_form: ["netlify", "forms", "getform", "formspree", "airtable", "static", "false"]
      #   For advanced usage see https://sourcethemes.com/academic/docs/page-builder/#contact-form
      widget: "contact"
      title: "Send a Message"
      subtitle: "We'll respond to your inquiry as soon as possible."
      text:

      # Contact details
      email: "info@soajotours.com"
      phone: "+351 123 456 789"
      address:
        street: "Rua Principal"
        city: "Soajo"
        region: "Viana do Castelo"
        postcode: "4990"
        country: "Portugal"
      coordinates:
        latitude: 41.8569
        longitude: -8.3806
    design:
      spacing:
        padding: ["4rem", 0, "4rem", 0]

  - block: cta-card
    content:
      title: "Ready for Your Adventure?"
      text: "Don't miss out on experiencing the beautiful nature of Soajo and Parque Peneda Gerês."
      button:
        text: "View Our Tours"
        url: "/"
    design:
      card:
        css_class: "bg-primary-600 text-white"
---