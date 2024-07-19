---
# An instance of the Contact widget.
widget: contact

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 130

title: Contact
subtitle:

content:
  # Automatically link email and phone or display as text?
  autolink: false

  # Email form provider
  #form:
  #  provider: netlify
  #  formspree:
  #    id:
  #  netlify:
      # Enable CAPTCHA challenge to reduce spam?
  #    captcha: false

  # Contact details (edit or remove options as required)
  email: d.carvalho@ieee.org
# phone: 888 888 88 88
  address:
    street: Av. Maracanã, 229
    city: Rio de Janeiro
    region: RJ
    postcode: '20271-204'
    country: Brazil
    country_code: BR
  coordinates:
    latitude: '-22.9118'
    longitude: '-43.2241'
  directions: Enter Building E and take the lift to Office 506 on Floor 5
  office_hours:
    - 'Monday 10:00 to 13:00'
    - 'Wednesday 14:00 to 15:00'
# appointment_url: 'https://calendly.com'
  contact_links:
    - icon: twitter
      icon_pack: fab
      name: DM d_carvalho
      link: 'https://twitter.com/Twitter'
    - icon: telegram
      icon_pack: fab
      name: DiegoCarvalho
      link: https://t.me/DiegoCarvalho
design:
  columns: '2'
---
