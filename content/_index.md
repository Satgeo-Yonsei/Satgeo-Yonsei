---
# 홈페이지 설정
title: "YESAT"
subtitle: "Satellite Geosciences Lab"
date: 2025-03-31

# 홈페이지 레이아웃 설정
type: landing

# 홈페이지 섹션/위젯 활성화
sections:
  - block: hero
    design:
      background:
        image:
          filename: public/background.png  # 배경 이미지 파일명
        text_color_light: true
    content:
      title: YESAT
      text: |
        <br>
        
        # Satellite Geosciences Lab
        
        Yonsei University, Earth System Sciences Department

  - block: markdown
    content:
      title: Who We Are
      text: |
        This is the webpage of the Satellite Geosciences Research Group at the Department of Earth System Sciences, Yonsei University.
        The group is led by Hahn Chul Jung, and the research that we do focuses on radar remote sensing, 
        land information system, natural disaster monitoring, 
        and the study of large-schale hydrology.
        
        What we do in our lab is as follows : 
        satellite data processing and develop algorithms for earth observation, 
        modeling implementation using satellite-based input data,
        analysis & understanding of natural phenomena using satellite data and modeling.
    design:
      columns: "2"
      css_style: |
        .section-title::after {
          content: '';
          position: absolute;
          left: 0;
          bottom: -10px;
          width: 80px;
          height: 3px;
          background-color: #0056b3;
        }
      css_class: "intro-section"

  - block: collection
    id: research
    content:
      title: What We Do
      subtitle: Our research areas
      text: ""
      count: 7  # 표시할 연구 영역 수
      filters:
        folders:
          - research
      sort_by: "weight"
    design:
      columns: "1"
      view: card
      flip_alt_rows: true
      background:
        color: "#f0f0f0"

  - block: collection
    id: people
    content:
      title: Our Team
      subtitle: Meet the researchers
      text: ""
      count: 10  # 표시할 사람 수
      filters:
        folders:
          - people
      sort_by: "weight"
    design:
      columns: "2"
      view: compact

  - block: contact
    id: contact
    content:
      title: Contact Us
      subtitle: Get in touch
      text: ""
      email: hcjung@yonsei.ac.kr
      address:
        street: Science Hall, 50 Yonsei-ro, Seodaemun-gu
        city: Seoul
        region: ""
        postcode: "03722"
        country: South Korea
        country_code: KR
      coordinates:
        latitude: "37.565"
        longitude: "126.938"
      directions: Enter Science Hall and take the stairs to the 5th floor
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: Follow us on Twitter
          link: "https://twitter.com/SatGeoLab"
    design:
      columns: "1"
---
