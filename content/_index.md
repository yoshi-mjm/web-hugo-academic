---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: features
    content:
      title: Skills
      items:
        - name: R
          description: 30%
          icon: r-project
          icon_pack: fab
        - name: Statistics
          description: 50%
          icon: chart-line
          icon_pack: fas
        - name: Apple
          description: 50%
          icon: apple
          icon_pack: fab
        - name: Linux
          description: 30%
          icon: linux
          icon_pack: fab
        - name: Network
          description: 15%
          icon: wifi
          icon_pack: fas
        - name: Coffee
          description: 100%
          icon: coffee
          icon_pack: fas
        - name: Photography
          description: 10%
          icon: camera
          icon_pack: fas
        - name: Aircraft
          description: 30%
          icon: fighter-jet
          icon_pack: fas
        - name: Car
          description: 30%
          icon: car
          icon_pack: fas
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
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
      view: list
      columns: '2'
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
---
