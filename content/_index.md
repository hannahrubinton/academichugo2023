---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: About Me
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: collection
    id: publications
    content:
      title: Publications
      filters:
        publication_type: "2"
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: workingpapers
    content:
      title: Working Papers
      filters: 
        publication_type: "3"
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: blogposts
    content:
      title: Blog Posts 
      filters: 
        publication_type: ""
        folders:
          - blogs
        exclude_featured: true
    design:
      columns: '2'
      view: list

---
