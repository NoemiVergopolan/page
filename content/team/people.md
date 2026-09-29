---
# People widget: current members as photo cards. Lists every page in
# content/authors/ whose `user_groups` matches one of the groups below. A group
# heading only appears once the group has at least one member. Alumni are
# listed separately, as text, by content/team/alumni.md.
#
# To add a member, copy content/authors/example-member/ to
# content/authors/<firstname-lastname>/ (the name as spelled in paper author
# lists) and follow the instructions at the top of that file.
widget: people
headless: true
weight: 10
active: true

title: Team
subtitle: ''

content:
  user_groups:
    - Principal Investigator
    - Postdoctoral Researchers
    - Graduate Students
    - Undergraduate Researchers

design:
  show_interests: false
  show_role: true
  show_social: true
  show_organizations: false
  spacing:
    # Customize the section spacing. Order is top, right, bottom, left.
    padding: ["80px", "20px", "40px", "20px"]
---
