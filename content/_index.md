---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: markdown
    content:
      subtitle: ''
      text: |-
        {{< gallery album="gallery_alpini" >}}
    design:
      columns: '2'
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
  - block: collection
    id: posts
    content:
      title: Eventi
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 8
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
  - block: portfolio
    id: projects
    content:
      title: IL GRUPPO
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false 
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Per contattare gli amici del Gruppo Alpini Valdarno Superiore scrivi qui:
      # Contact (add or remove contact options as necessary)
      email: gruppoalpini.valdarno@gmail.com
      phone: 3332616399
      address:
        street: Strada provinciale Penna 11
        city: Terranuova Bracciolin
        region: AR
        postcode: 52028
        country: Italia
        country_code: IT
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
