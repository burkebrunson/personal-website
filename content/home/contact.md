---
# An instance of the Contact widget.
widget: contact

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 60

title: Contact
subtitle:

content:
  # Automatically link email and phone or display as text?
  autolink: true

  # Email form provider
  form:
    provider: netlify
    formspree:
      id:
    netlify:
      # Enable CAPTCHA challenge to reduce spam?
      captcha: true

  # Contact details (edit or remove options as required)
  email: ""
  phone: ""
  address:
    street: 81 Cornell St. Stop 8358
    city: Grand Forks
    region: ND
    postcode: "58202"
    country: United States
    country_code: US
  coordinates:
    latitude: "47.919851"
    longitude: "-97.068496"
  directions: Enter Leonard Hall and take the stairs or elevator to the 2nd floor (2) and go to Rm. 206 (Planetary Geology) or to the Basement (B) and go to Rm. 11 (Geothermal Lab), depending on meeting location.
  office_hours:
    - Meetings by appointment are preferred, but I maintain an open door policy.
  appointment_url: "https://outlook.office365.com/owa/calendar/DanielBBrunson@ad.ndus.edu/bookings/"
  contact_links:
    - icon: twitter
      icon_pack: fab
      name: DM Me
      link: "https://twitter.com/BurkeBrunson"
    - icon: video
      icon_pack: fas
      name: Zoom Me
      link: "https://und.zoom.us/my/burke.brunson"

design:
  columns: "2"
---
