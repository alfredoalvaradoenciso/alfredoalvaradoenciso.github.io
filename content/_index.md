---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/CV_AlfredoAlvarado.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: collection
    id: papers
    content:
      title: Recent Publications
      text: ""
      count: 3
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: markdown
    id: media
    content:
      title: Recent Media
      text: <ul><li><a href='https://larazon.pe/una-reforma-tributaria-para-que-los-que-tienen-mayores-rentas-paguen-mas-impuestos/'> Una reforma tributaria para que los que tienen mayores rentas paguen mas impuestos</a>.</li>
        <li><a href='https://andina.pe/agencia/noticia-sunafil-estrategia-disminuye-incumplimiento-los-los-derechos-laborales-915898.aspx'> Sunafil estrategia disminuye el incumplimiento de los derechos laborales</a>.</li>
        <li><a href='http://blog.pucp.edu.pe/blog/idhal/2021/02/09/el-rompecabezas-de-la-informalidad/'> El rompecabezas de la informalidad</a>.</li></ul> <div class="mt-10 flex justify-center"><a class="relative inline-flex items-center gap-1 rounded-md border border-gray-300 bg-white px-3 py-2 pl-4 text-sm font-medium text-gray-500 hover:bg-gray-50 focus:z-20 dark:border-gray-500 dark:bg-gray-800 dark:text-gray-300" href="/media/"><span>See all media appearances</span></a></div>
      filters:
        folders:
          - media
  - block: markdown
    id: contact
    content:
      title: Contact Me
      text:
      {{< icon name="hero/envelope" >}} alvaradoencisoa@gmail.com
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
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
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
---
