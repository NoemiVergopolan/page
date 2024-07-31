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
  autolink: true

  # Email form provider
  form:
    provider: 
    formspree:
      id:
    netlify:
      # Enable CAPTCHA challenge to reduce spam?
      captcha: false

  # Contact details (edit or remove options as required)
  #email: noemi@princeton.edu
  # phone: 888 888 88 88
  # address:
  #   street: 450 Serra Mall
  #   city: Stanford
  #   region: CA
  #   postcode: '94305'
  #   country: United States
  #   country_code: US
  # coordinates:
  #   latitude: '37.4275'
  #   longitude: '-122.1697'
  # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
  # office_hours:
  #   - 'Monday 10:00 to 13:00'
  #   - 'Wednesday 09:00 to 10:00'
  # appointment_url: 'https://calendly.com'
  contact_links:
  #  - icon: envelope
  #    icon_pack: fas
  #    name: 'Noemi.Vergopolan@noaa.gov'
  #    link: 'malito:Noemi.Vergopolan@noaa.gov'
    - icon: envelope
      icon_pack: fas
      name: 'Noemi.Vergopolan@rice.edu'
      link: 'malito:Noemi.Vergopolan@rice.edu'
  #  - icon: envelope
  #    icon_pack: fas
  #    name: 'Noemi@princeton.edu'
  #    link: 'malito:noemi@princeton.edu'
    - icon: twitter
      icon_pack: fab
      name: '@NVergopolan'
      link: 'https://twitter.com/NVergopolan'
    - icon: linkedin
      name: LinkedIn
      icon_pack: fab
      link: https://www.linkedin.com/in/vergopolan/
    
    
    # - icon: video
    #   icon_pack: fas
    #   name: Zoom Me
    #   link: 'https://zoom.com'

design:
  columns: '2'

  spacing:
    # Customize the section spacing. Order is top, right, bottom, left.
    padding: ["80px", "20px", "80px", "20px"]

---

