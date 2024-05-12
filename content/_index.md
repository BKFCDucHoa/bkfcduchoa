---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: hero
    id: hero
    content:
      title: BKFC THPT Đức Hoà
      image:
        filename: logo.png
      cta:
        label: 'Facebook'
        url: https://www.facebook.com/bkfcduchoalongan/
      cta_alt:
        label: Messenger
        url: https://www.messenger.com/t/bkfcduchoalongan/
      cta_note:
        label: >-
          Online trong khoảng 6:00am đến 10:10pm
      text: |-
        -> *Những người bạn đồng hành cùng học sinh trường THPT Đức Hòa*

        Cập nhật những thông tin mới nhất về:
        
          - Kỳ thi THPT Quốc gia
          - Kỳ thi Đánh giá năng lực của ĐHQG Tp.HCM
        
          Cùng ôn lại, giải thêm những bài tập [_Toán_](/tag/toan/), [_Lý_](/tag/ly/), [_Hóa_](/tag/hoa/),...

    design:
          background:
            gradient_end: '#1976d2'
            gradient_start: '#004ba0'
            text_color_light: true
  - block: about.biography
    id: about
    content:
      title: Giới thiệu
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: slider
    content:
      slides:
        - title: 👋 Xin chào!
          content: Rất vui vì bạn đã đến với site của chúng mình
          align: center
          background:
            image:
              # Specify an image from `assets/media/`
              # or delete the image section to remove it
              filename:
              filters:
                brightness: 0.7
            position: right
            color: '#666'
          link:
            icon: facebook
            icon_pack: fab
            text: Liên hệ chúng mình tại đây nhé!
            url: 'https://www.facebook.com/bkfcduchoalongan/'
        - title: Bạn là học sinh cấp 3?
          content: 'Xem hướng dẫn tại link sau nhé!'
          align: left
          background:
            image:
              # Specify an image from `assets/media/`
              # or delete the image section to remove it
              filename:
              filters:
                brightness: 0.7
            position: center
            color: '#555'
          link:
            icon: link
            icon_pack: fas
            text: Hướng dẫn tại đây
            url: /post/2020-05-30-huong-dan-hoc-sinh/
        - title: Bạn là thành viên nhóm?
          content: 'Xem hướng dẫn tại link sau nhé!'
          align: right
          background:
            image:
              # Specify an image from `assets/media/`
              # or delete the image section to remove it
              filename:
              filters:
                brightness: 0.5
            position: center
            color: '#333'
          link:
            icon: link
            icon_pack: fas
            text: Hướng dẫn tại đây
            url: /courses/huong-dan-thanh-vien
    design:
      # Slide height is automatic unless you force a specific height (e.g. '400px')
      slide_height: '400px'
      # Make the slides full screen within the browser window?
      is_fullscreen: false
      # Automatically transition through slides?
      loop: false
      # Duration of transition between slides (in ms)
      interval: 2000
  - block: collection
    id: posts
    content:
      title: Bài viết gần đây
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
  - block: collection
    id: events
    content:
      title: Sự kiện
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - event
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
  - block: markdown
    id: gallery
    content:
      title: Thư viện ảnh
      subtitle: ''
      text: |-
        {{< gallery album="gallery" >}}
    design:
      columns: '1'
  - block: tag_cloud
    id: tags
    content:
      title: Từ khoá phổ biến
      text: "[_Xem tất cả từ khoá_](/tags)"
    design:
      columns: '2'
  - block: people
    id: people
    content:
      title: Các thành viên
      # Choose which groups/teams of users to display.
      #   Edit `user_groups` in each user's profile to add them to one or more of these groups.
      user_groups:
        - Members
      sort_by: Params.last_name
      sort_ascending: true
    design:
      # Show user's social networking links? (true/false)
      show_social: true
      # Show user's interests? (true/false)
      show_interests: true
      # Show user's role?
      show_role: true
      # Show user's organizations/affiliations?
      show_organizations: true
  - block: contact
    id: contact
    content:
      title: Liên hệ
      subtitle:
      text: |-
        Nếu bạn có bất kỳ câu hỏi nào, hãy liên hệ với chúng tôi qua một trong những cách sau:
      # Contact (add or remove contact options as necessary)
      email: ''
      phone: ''
      appointment_url: ''
      address:
        street: 268 Lý Thường Kiệt, Phường 14, Quận 10
        city: Tp.Hồ Chí Minh
        region: ''
        postcode: '700000'
        country: Việt Nam
        country_code: VN
      directions: ''
      office_hours:
        - '8:00 đến 18:00 các ngày trong tuần'
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      coordinates:
        latitude: '10.77331'
        longitude: '106.65938'  
      contact_links:
        - icon: facebook
          icon_pack: fab
          name: Facebook
          link: 'https://www.facebook.com/bkfcduchoalongan/'
        - icon: facebook-messenger
          icon_pack: fab
          name: Messenger
          link: 'https://www.messenger.com/t/bkfcduchoalongan/'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: ''
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
