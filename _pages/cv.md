---
layout: none
permalink: /cv/
title: cv
nav: true
nav_order: 5
# 메뉴의 'cv' 를 눌렀을 때 바로 열릴 PDF 경로.
# 본인 CV 파일로 바꾸세요. (예: /assets/pdf/cv.pdf)
nav_url: /assets/pdf/example_pdf.pdf
---
{% assign cv_pdf_url = page.nav_url | relative_url %}
<!-- /cv/ 로 직접 들어오거나 검색으로 와도 PDF 로 바로 이동 -->
<!DOCTYPE html>
<html lang="{{ site.lang | default: 'en' }}">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="refresh" content="0; url={{ cv_pdf_url }}">
    <link rel="canonical" href="{{ cv_pdf_url }}">
    <title>CV</title>
  </head>
  <body>
    <p>Redirecting to <a href="{{ cv_pdf_url }}">CV (PDF)</a>…</p>
  </body>
</html>