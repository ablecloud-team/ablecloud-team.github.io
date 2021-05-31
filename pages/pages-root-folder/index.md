---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth: header_unsplash_12.jpg
widget1:
  title: "제품"
  url: 'http://phlow.github.io/feeling-responsive/blog/'
  image: https://via.placeholder.com/302x182
  text: '<br/>ABLESTACK은 기업의 데이터센터에 설치하여 엔터프라이즈 클라우드 환경을 구축하는 HCI 플랫폼으로 ABLECLOUD의 제품 전체를 상징합니다. 단 하나의 플랫폼으로 어떤 가상머신이든, 어떠한 앱이든, 어떠한 가상화/클라우드 환경이든 사용하고 관리할 수 있습니다. 상용 x86 서버에 10G Network에 연결하고 ABLESTACK을 설치하여 지금 바로 핵심 인프라를 포함하여 모든 애플리케이션을 시작하십시오.'
widget2:
  title: "솔루션"
  url: 'http://phlow.github.io/feeling-responsive/info/'
  text: '<br/>ABLESTACK을 활용하면 기업은 어떠한 애플리케이션이든 모두 단일 인프라를 이용해 실행할 수 있기 때문에 전총적인 사일로 인프라를 제고하고 새로운 형태의 기업 데이터센터를 운영할 수 있는 유연성과 확장성, 안정성을 제공합니다. 기업은 지금 바로 모든 IT인프라에 대해 단일 플랫폼으로 인프라를 단순화하고 민첩성을 높일 수 있습니다. ABLESTACK이 제공하는 클라우드 환경에서 다양한 솔루션을 만나 보십시오. '
  image: https://via.placeholder.com/302x182
widget3:
  title: "파트너"
  url: 'https://github.com/Phlow/feeling-responsive'
  image: https://via.placeholder.com/302x182
  text: '<br/>우리는 ABLESTACK을 기반으로 고객에게 끊임없이 변화하는 IT 기술 환경에 적응할 수 있는 인프라를 제공하고, 자동화하며, 모니터링하기 위한 토탈 플랫폼을 제공합니다. 지금 바로 사용 가능하고, 빠르게 배포하며, 어떠한 워크로드에도 적용할 수 있는 ABLESTACK의 파트너로 함께 할 수 있습니다. 유연한 개방형 기술 플랫폼으로써 지속적으로 전문가 지원을 제공할 준비가 되다면 에이블클라우드와 함께 해주십시오.'
#
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
callforaction:
  url: https://tinyletter.com/feeling-responsive
  text: 보다 더 자세한 자료와 컨설팅이 필요하십니까? ›
  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---

<div id="videoModal" class="reveal-modal large" data-reveal="">
  <div class="flex-video widescreen vimeo" style="display: block;">
    <iframe width="1280" height="720" src="https://www.youtube.com/embed/3b5zCFSmVvU" frameborder="0" allowfullscreen></iframe>
  </div>
  <a class="close-reveal-modal">&#215;</a>
</div>
