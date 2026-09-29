---
# ============================================================================
#  TEAM MEMBER PROFILE TEMPLATE
# ============================================================================
#
#  1. Fill in the fields below. Only the REQUIRED fields must be filled in.
#     Every OPTIONAL section can be left as it is: anything left blank or
#     commented out (lines starting with #) is simply not shown, so the page
#     stays short.
#
#  2. Write one to three sentences about the person's research below the
#     closing `---` at the bottom of this file.
#
#
#  WHEN SOMEONE GRADUATES OR LEAVES: change `user_groups` to Alumni and update
#  `role` to their degree and where they went (e.g. "PhD 2028, now Research
#  Scientist at NOAA"). They move from the photo cards to the text-only Alumni
#  list below the current members on the Team page, where each line is their name and
#  `role`. To order that list, add `weight: 1`, `weight: 2`, ... (lower first);
#  without weights it is alphabetical. Keep the folder: their profile page and
#  publication links keep working.
# ============================================================================

# true = hidden everywhere, false = published.
draft: false


# --- REQUIRED ---------------------------------------------------------------

# Full name, as shown on the Team page and profile.
title: Caroline Hashimoto
first_name: Caroline
last_name: Hashimoto

# One short line shown under the name, e.g. "PhD Student", "Postdoctoral
# Research Associate", "Undergraduate Researcher", "PhD 2028, now at NOAA".
role: Undergrad 2025, now PhD at Caltech.

# Which heading this person appears under on the Team page. Use exactly ONE of
# these, spelled exactly as shown:
#   Postdoctoral Researchers     \
#   Graduate Students             > current members: shown as photo cards
#   Undergraduate Researchers    /
#   Alumni                       -> former members: shown as a text list below
#                                   the photo cards (name + role), no photo needed
user_groups:
  - Alumni

# Year graduated or left; sorts the Alumni list newest first.
graduation_year: 2025


# --- OPTIONAL: affiliation --------------------------------------------------
# Shown under the role on the profile page. Delete the `name:` text to hide it.
organizations:
  - name: Rice University
    url: https://eeps.rice.edu/


# --- OPTIONAL: contact and social icons -------------------------------------
# Icons shown under the photo. To show one, remove the `#` at the start of its
# three lines and put in the link. Icons left commented out are not shown.
social:
#  - icon: envelope
#    icon_pack: fas
#    link: mailto:first.last@rice.edu
#  - icon: google-scholar
#    icon_pack: ai
#    link: https://scholar.google.com/citations?user=XXXXXXXX
#  - icon: linkedin
#    icon_pack: fab
#    link: https://www.linkedin.com/in/XXXXXXXX/
#  - icon: github
#    icon_pack: fab
#    link: https://github.com/XXXXXXXX
#  - icon: orcid
#    icon_pack: ai
#    link: https://orcid.org/0000-0000-0000-0000
#  - icon: globe
#    icon_pack: fas
#    link: https://personal-website.example


# --- OPTIONAL: research interests -------------------------------------------
# Shown as a short list on the profile page. Keep each item to a few words.
# Leave the list empty ([]) to hide the Interests section.
interests: []
#  - Soil Moisture
#  - Remote Sensing
#  - Machine Learning


# --- OPTIONAL: education ----------------------------------------------------
# Shown on the profile page, most recent first. Include the degree in progress
# (e.g. "PhD in Earth, Environmental and Planetary Sciences (in progress)")
# and previous degrees. Entries with an empty `course` are not shown, and the
# whole Education section is hidden when none are filled in.
#
#   course:          degree or certificate name (REQUIRED for the entry to show)
#   institution:     university and year, e.g. "Rice University, 2024"
#   institution_url: optional link for the degree name
#   certificate_url: use instead of institution_url for a certificate; it shows
#                    a certificate icon instead of a graduation cap
education:
  courses:
    - course: ''
      institution: ''
      institution_url: ''
    - course: ''
      institution: ''
      institution_url: ''
    - course: ''
      institution: ''
      institution_url: ''


# --- Do not change ----------------------------------------------------------
avatar_filename: avatar.jpg
superuser: false
highlight_name: false
---

