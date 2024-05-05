---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
  - block: features
    content:
      title: Навыки
      items:
        - name: Программирование
          description: 10%
          icon: laptop-code
          icon_pack: fas
        - name: Скорость печати
          description: 80%
          icon: keyboard
          icon_pack: fas
        - name: Английский язык
          description: 90%
          icon: language
          icon_pack: fas
        - name: Французский язык
          description: 40%
          icon: language
          icon_pack: fas
  - block: experience
    content:
      title: Опыт работы
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Студент
          company: РУДН
          company_url: 'https://www.rudn.ru/'
          company_logo: 
          location: Москва
          date_start: '2022-09-01'
          date_end: ''
          description: |2-
           
             Компьютерные и информационные науки
    design:
      columns: '2'
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Достижения'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: https://stepik.org/cert/1936266
          date_end: '2023-02-03'
          date_start: '2023-01-25'
          description: 'Пройдено 100%'
          organization: Stepik
          organization_url: https://www.stepik.org
          title: Математика в кибербезопасности
          url: 'https://stepik.org/course/62247/info'
        - certificate_url: https://stepik.org/cert/1895974
          date_end: '2022-12-30'
          date_start: '2022-12-29'
          description: 'Пройдено 100%'
          organization: Stepik
          organization_url: https://www.stepik.org
          title: Безопасность в интернете
          url: https://stepik.org/course/191/info
        - certificate_url: https://stepik.org/cert/2146127
          date_end: '2023-08-09'
          date_start: '2023-06-24'
          description: 'Пройдено 100%'
          organization: Stepik
          organization_url: https://www.stepik.org
          title: Основы программирования на C. Задачи.
          url: https://stepik.org/course/3078/info
        - certificate_url: https://stepik.org/cert/2090380
          date_end: '2023-06-03'
          date_start: '2023-04-29'
          description: 'Пройдено 100%'
          organization: Stepik
          organization_url: https://www.stepik.org
          title: Введение в Linux
          url: https://stepik.org/course/3078/info
        - certificate_url: https://drive.google.com/file/d/1KiTFhsJWny2uMpCCZNSCLo1vcaww_Ocg/view?usp=sharing
          date_end: '2024-05-05'
          date_start: '2024-02-17'
          description: 'Пройдено 100%'
          organization: Stepik
          organization_url: https://www.stepik.org
          title: Основы кибербезопасности
          url: https://stepik.org/course/111512/info
          
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: Последние публикации
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
      view: compact
      columns: '2'
  - block: portfolio
    id: projects
    content:
      title: Проекты
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
      buttons:
        - name: All
          tag: '*'

    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  
  - block: collection
    id: featured
    content:
      title: Рекомендуемые публикации
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  
  - block: collection
    id: talks
    content:
      title: Прошедшие и предстоящие выступления
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: tag_cloud
    content:
      title: Популярные темы
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Контакты
      subtitle:
      text: |-
      # Contact (add or remove contact options as necessary)
      email: По обращению
      phone: По обращению
      appointment_url: 'https://calendly.com'
      address:
        street: 
        city: Москва
        region:
        postcode:
        country: Россия
        country_code: РУ
      directions: Напротив РУДН
      office_hours: Всегда
      contact_links:
        - icon: skype
          icon_pack: fab
          name: Доступен в Скайпе
          link: 'skype:echo123?call'
        - icon: video
          icon_pack: fas
          name: Доступен в Зуме
          link: 'https://zoom.com'
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
