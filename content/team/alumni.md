---
# Alumni list (layouts/partials/blocks/alumni.html): a compact text list of
# every author page with `user_groups: [Alumni]`, shown below the current
# members on the Team page. Each line is the name (linked to their profile) and their `role`.
# Sorted by `graduation_year` in each alumni _index.md, newest first (same
# year, or no year: alphabetical). Shows nothing while there are no alumni.
widget: alumni
headless: true
weight: 20
active: true

title: Alumni
subtitle: ''

content:
  user_groups:
    - Alumni

design:
  spacing:
    # Customize the section spacing. Order is top, right, bottom, left.
    padding: ["20px", "20px", "60px", "20px"]
---
