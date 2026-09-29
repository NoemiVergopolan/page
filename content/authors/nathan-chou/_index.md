---
# ============================================================================
#  TEAM MEMBER PROFILE TEMPLATE
# ============================================================================
#
#  On the Team page each member is a photo card; clicking it opens a detail
#  card in place (no separate page) with their photo, role, links, research
#  areas and education.
#
#  1. Copy this folder to content/authors/<firstname-lastname>/ and put their
#     photo next to this file as avatar.jpg (square, at most 900 px).
#
#  2. Fill in the fields below. Only the REQUIRED fields must be filled in.
#     Every OPTIONAL section can be left as it is: anything left blank or
#     commented out (lines starting with #) is simply not shown, so the card
#     stays short.
#
#  WHEN SOMEONE GRADUATES OR LEAVES: change `user_groups` to Alumni and update
#  `role` to their degree and where they went (e.g. "PhD 2028, now Research
#  Scientist at NOAA"). They move from the photo cards to the text-only Alumni
#  list below the current members on the Team page, where each line is their name and
#  `role`. Also set `graduation_year` (below): the list is sorted newest year
#  first. Their name in that list still opens their detail card.
# ============================================================================

# true = hidden everywhere, false = published.
draft: false


# --- REQUIRED ---------------------------------------------------------------

# Full name, as shown on the Team page and detail card.
title: Nathan Chou
first_name: Nathan
last_name: Chou

# One short line shown under the name, e.g. "PhD Student", "Postdoctoral
# Research Associate", "Undergraduate Researcher", "PhD 2028, now at NOAA".
role: M.S. Student

# Which heading this person appears under on the Team page. Use exactly ONE of
# these, spelled exactly as shown:
#   Postdoctoral Researchers     \
#   Graduate Students             > current members: shown as photo cards
#   Undergraduate Researchers    /
#   Alumni                       -> former members: shown as a text list below
#                                   the photo cards (name + role), no photo needed
user_groups:
  - Graduate Students

# ALUMNI ONLY: the year they graduated (or, for postdocs and staff, the year
# they left), e.g. 2028. Sorts the Alumni list newest first; people in the same
# year are alphabetical, and alumni without a year are listed last. Not shown
# on the page itself, so also mention the year in `role`. Leave blank for
# current members.
graduation_year:


# --- OPTIONAL: affiliation --------------------------------------------------
# Shown under the role on the detail card. Delete the `name:` text to hide it.
organizations:
  - name: Rice University
    url: https://eeps.rice.edu/


# --- OPTIONAL: contact and social icons -------------------------------------
# Shown as labelled buttons on the detail card (email shows the address). To
# show one, remove the `#` at the start of its three lines and put in the
# link. Entries left commented out are not shown.
social:
  - icon: envelope
    icon_pack: fas
    link: mailto:nwc1@rice.edu


# --- OPTIONAL: research areas ------------------------------------------------
# Shown as "Research areas" on the detail card. Keep each item to a few words.
# Leave the list empty ([]) to hide it.
interests: []


# --- OPTIONAL: education ----------------------------------------------------
# Shown on the detail card, most recent first. Include the degree in progress
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
    - course: "M.S. in Earth, Environmental and Planetary Sciences (in progress)"
      institution: "Rice University"
    - course: "B.S. in Computer Science, minor in Earth, Environmental and Planetary Sciences"
      institution: "Rice University, 2025"


# --- Do not change ----------------------------------------------------------
avatar_filename: avatar.jpg
superuser: false
highlight_name: false
---
