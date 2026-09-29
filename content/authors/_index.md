---
cms_exclude: true

# To publish author profile pages, remove all of the `_build` and `cascade` settings below.
# Team members opt back in individually with `_build: {render: always}` in their
# own _index.md, so only people with a profile folder get a page, not every
# co-author in the publication list.
_build:
  render: never
cascade:
  _build:
    render: never
    list: always
---
