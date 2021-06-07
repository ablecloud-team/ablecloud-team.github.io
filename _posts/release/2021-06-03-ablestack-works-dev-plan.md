---
layout: page-fullwidth
title:  "ABLESTACK Works 개발 계획"
subheadline:  "제품 및 기능 릴리즈"
teaser: "<br/>ABLESTACK은 HCI를 기반으로 조직의 사용자에게 가상의 데스크톱 서비스를 제공할 수 있도록 Mold를 통해 관련 구성요소를 자동으로 배포하고, 가상 데스크톱 관리자가 직접 가상머신을 생성, 사용자에게 할당할 수 있도록 하는 기능을 가진 Works를 2021년 9월 중으로 개발 완료하여 릴리즈할 예정입니다."

categories:
    - Release
tags:
  - ablestack
  - release
  - roadmap

header:
   title: ''
   image_fullwidth: corona-virus-illustration.jpeg

image:
   thumb: corona-virus-illustration-thumb.png
   homepage: corona-virus-illustration.jpeg
---

<div class="row">
<div class="medium-4 medium-push-8 columns" markdown="1">
  <div class="panel radius" markdown="1">
  **Table of Contents**
  {: #toc }
  *  TOC
  {:toc}
  </div>
</div><!-- /.medium-4.columns -->

<div class="medium-8 medium-pull-4 columns" markdown="1">

### 제품 개발 배경
<br/>
<div class="row">
   <div class="medium-12 columns">
      <p>
        가상화 환경을 기업에 도입한 후 최종 사용자에게 제공할 수 있는 서비스에 대한 고민이 생기게 됩니다. 이러한 고민의 가장 빠른 해결 방법은 바로 최종 사용자 컴퓨팅입니다. 최종 사용자 컴퓨팅은 Virtual Desktop 또는 Virtual Workspace라는 용어로 표현되기도 합니다. 
      </p>
      <p>
        또한 최근 코로나19로 인해 비대면 업무 환경에 대한 관심이 높아지고, 실제 재택근무 환경을 도입하는 기업이 늘고 있습니다. 이러한 흐름에서 빠르게 비대면 또는 재택근무 환경을 도입하면서, 안전하게 기업의 데이터를 보호할 수 있는 환경으로 최종 사용자 컴퓨팅이 주목 받고 있습니다. 
      </p>
  </div>
</div>

</div>
</div>

<div class="row">
   <div class="medium-12 columns">
      <p>
        우리는 이러한 인프라 환경의 흐름, 최종 사용자의 요구 등을 반영할 수 있도록 하기 위해 원클릭으로 최소화된 자원 만으로 최종 사용자 컴퓨팅을 제공할 수 있는 기능인 Works를 개발하기로 결정하였습니다. 
      </p>
   </div>
</div>
<br/>


### Works 주요 특징
<br/>
ABLESTACK Works는 다음과 같은 특징을 가집니다.

<div class="row">
  <div class="medium-4 column" style="padding:40px 15px">
    <img src="/images/last-mile-delivery-cost-main.png">
  </div>
  <div class="medium-8 column">
    <p>
      <ul>
        <li><b>다양한 하이퍼바이저 지원</b> : ABLESTACK 뿐 아니라 KVM, VMWare, Citrix Hypervisor 등의 지원</li>
        <li><b>최소 자원 구성</b> : 워크스페이스를 제공할 때 Windows License를 최소화 합니다. Active Directory 서버 등을 오픈소스로 구성하여 필수 자원을 줄입니다.</li>
        <li><b>원클릭 배포</b> : 구성요소를 자동으로 프로비저닝하여 구성을 단순화 합니다. 게이트웨이, 워크스페이스 관리, Active Directory, 포털 등을 별도로 설치할 필요가 없습니다.</li>
        <li><b>Clientless 접속</b> : 전용 클라이언트 없이 바로 업무 환경에 접속할 수 있도록 합니다. 웹 브라우저를 이용해 모든 워크스페이스에 접속 가능합니다.</li>
        <li><b>Desktop 및 App 가상화 지원</b> : 사용자에게 데스크탑 뿐만 아니라 특정한 앱만 사용 가능하도록 자원을 유연하게 할당할 수 있습니다. </li>
        <li><b>다양한 Guest OS 지원</b> : Windows 뿐 아니라 리눅스, 국산 OS 등을 모두 지원합니다.</li>
      </ul>
    </p>
  </div>
</div>

<br/>

### Works 아키텍처
<br/>
ABLESTACK Works의 사용자 및 소프트웨어 구성요소 간의 아키텍처는 다음과 같습니다 

<div class="row">
  <div class="medium-12 column" style="padding:0 30px; text-align: center;">
    <img src="/images/ablestack-works-architecture.png">
  </div>
</div>

#### Mold를 통한 배포 통합
<br/>
모든 Mold 사용자는 자신만의 Works 구성요소를 배포할 수 있습니다. 즉, Mold가 제공하는 클라우드 환경을 통해, 사용자가 속한 도메인별로, 또는 사용자가 생성한 도메인별로 가상 데스크톱 환경을 생성할 수 있습니다. 

인프라 관리자는 ABLESTACK Mold를 통해 기업에 단일의 워크스페이스를 만들 수도 있으며, 전문가 커뮤니티 내에 다수의 조직별로 필요한 워크스페이스를 만들어 제공할 수 있기 때문에 높은 유연성을 가진 DaaS 서비스를 제공할 수 있습니다. 

#### 단순화된 구성요소
<br/>
가상 데스크톱 및 가상 앱을 조직 또는 사용자에게 제공하기 위해서는 Active Directory 및 DB 서버, 관리자/사용자 포털 등이 제공되어야 합니다. 

Works는 이러한 모든 구성요소가 **Works Proxy** 라는 가상머신에 내장되어 제공됩니다. 따라서 별도의 관리용 Windows 운영체제 라이선스가 필요 없습니다. 또한 해당 프록시 서버가 연결용 게이트웨이 역할도 제공하기 때문에 내부 접속 및 내부 접속을 위한 구조가 매우 단순해 집니다. 

#### 웹 기반 Works 포털
<br/>
Works는 웹 기반의 관리자 및 사용자 포털을 제공합니다. 

웹 기반 포털을 통해 관리자는 빠르게 사용자용 가상머신 및 애플리케이션을 배포할 수 있고, 사용자에게 할당할 수 있으며, 정책 및 권한, 공지사항 등을 관리할 수 있습니다. 또한 Works 포털을 기업의 환경에 맞게 커스터마이징 할 수 있어, 기업 내부 시스템과 Look & Feel을 일관성 있게 유지하여 사용자에게 제공할 수 있습니다. 

사용자는 웹 페이지를 통해 별도의 클라이언트 없이 자신만의 업무용 데스크톱에 접속하거나, 사용자에게 할당된 애플리케이션을 실행할 수 있습니다. 

#### 데스크톱/앱 가상화 지원
<br/>
Works는 사용자에게 전용으로 할당된 데스크톱을 제공하거나, 관리자에 의해 지정된 특정한 앱만을 제공할 수 있습니다. 

데스크톱은 사용자가 사용할 수 있는 애플리케이션이 미리 설치되어 있고, 사용자가 원하는 애플리케이션을 설치할 수 있는 일반적인 Windows 데스크톱입니다. 

애플리케이션 가상화를 이용하게 되면 사용자에게 데스크톱을 제공하는 대신, 사용자가 업무 중 사용하는 특정 애플리케이션만 사용하도록 제한할 수 있습니다. 예를 들어 전문가용 애플리케이션, 또는 오피스 애플리케이션 만 제한하여 사용할 수 있도록 함으로써 자원을 더 효율적이고 안전하게 사용하도록 할 수 있습니다. 
<br/><br/>

### Mommoss 전문가용 Works
<br/>
ABLESTACK Works는 에이블스토어의 전문가 커뮤니티 플랫폼인 Mommoss와 연계하여, 전문가(세무사, 변리사, 법무사, 변호사 등의 전문가 그룹)에게 필요한 가상 데스크톱 환경 또는 애플리케이션을 제공하도록 통합 개발됩니다. 

<div class="row">
  <div class="medium-12 column" style="padding:0 30px; text-align: center;">
    <img src="/images/ablestack-works-mommoss.png">
  </div>
</div>

전문가 커뮤니티 플랫폼인 Mommoss에 가입한 사용자가 워크스페이스 서비스에 가입하면 해당 사용자를 위한 도메인이 생성되고, 워크스페이스가 만들어집니다. 

이러한 워크스페이스를 통해 편의성 및 접근성이 높아지고, 업무용 데스크톱의 유지보수가 간편해 지며, 전문가의 중요한 데이터를 보호할 수 있게 되어 언제 어디서나 안전하고 편리한 업무환경을 사용할 수 있습니다. 

<br/>
<div class="row" style="text-align: center;">
  <a class="button center r15 small radius" href="/assets/files/ablestack-works-mommoss.pdf" target="_blank">더 자세한 Mommoss & ABLESTACK Works 자료보기 &gt;</a>
</div>

<br/><br/>
{% include next-previous-post-in-category %}

<br/><br/>
<h3>제품 및 기능 릴리즈 카테고리의 다른 문서</h3>
<br/>
{% include list-posts entries='3' offset='0' category='Release' %}