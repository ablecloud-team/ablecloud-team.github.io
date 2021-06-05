---
layout: page-fullwidth
title:  "ABLESTACK 1.0 Allo 릴리즈"
subheadline:  "제품 및 기능 릴리즈"
teaser: "<br/>우리는 기업의 새로운 클라우드 데이터센터 구축을 위한 최고의 소프트웨어스택인 ABLESTACK의 첫번째 버전을 릴리즈 하고 자신있게 제품을 선보입니다. 지금 바로 ABLESTACK을 기업에서 설치하여 프라이빗 클라우드 환경을 구성할 수 있습니다."

categories:
    - Release
tags:
  - ablestack
  - release
  - allo

header:
   title: ''
   image_fullwidth: ablestack-allo-background.png

image:
   thumb: home_product_thumb.png
   homepage: ablestack-allo-background.png
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

### Codename : Allo
<br/>
<div class="row">
   <div class="small-4 columns">
      <img src="/images/allosaurus-img.jpeg">
   </div>
   <div class="small-8 columns">
      <p>
        ABLESTACK은 소프트웨어 정의 클라우드 데이터센터를 구축하기 위한 최적의 솔루션으로써의 미션을 달성하고, HCI 시장의 공룡이 되겠다는 다짐을 담아 버전 코드명을 공룡의 이름으로 정하기로 결정했습니다. 영어로 된 공룡의 이름 중 Saurus를 뺀 나머지 이름을 코드명으로 합니다. 
      </p>
   </div>
</div>
<br/>


금번 버전 1.0의 버전 코드명은 **"알로"** 입니다. 위키백과에서 알로사우르스에 대한 내용을 살펴보면 다음과 같습니다. 

</div>
</div>

{% include alert text='알로사우루스는 후기 쥐라기를 대표하는 큰 육식공룡이다. 알로사우루스라는 학명의 어원은 고대 그리스어 인데, 이 말은 "특이한 도마뱀"이라는 뜻으로, 한자표기 이특룡은 여기서 비롯되었다. 미국의 고생물학자 오스니얼 찰스 마시가 알로사우루스속 화석을 처음으로 기재했다.' %}

우리는 ABLESTACK이 HCI 시장에서 특별하고, 선도적인 제품이 되기를 소망합니다. 그러한 제품이 되기 위해서 첫 버전인 Allo 부터 이러한 생각을 담고 제품을 개발했으며, 앞으로도 이러한 선도적이며, 사용자에게 특별한 제품이 될 수 있도록 하기 위해 최선을 다해 제품을 개발할 것입니다. 

<br/>

### 릴리즈에 포함된 구성요소
<br/>
ABLESTACK 1.0 Allo는 기업에 소프트웨어로 정의된 클라우드 데이터센터를 구성하여 프라이빗 클라우드를 제공하고, 단순한 구조로 고가용성을 제공하는 가상화 인프라를 제공하기 위해 다음의 구성요소를 포함합니다. 

#### 핵심 인프라 구성요소

<div class="row">
  <div class="medium-12 column" style="padding:0 30px;">
    <p>
      <ul>
        <li>Cube : 호스트에 설치하는 운영체제로 하이퍼바이저와 ABLESTACK을 위한 패키지가 포함되어 있습니다. </li>
        <li>Cell : 가상화를 처리하는 하이퍼바이저로 Cube를 서버에 설치하면 자동으로 설치됩니다. </li>
        <li>Glue : 대용량 분산 데이터 처리를 지원하는 분산 스토리지로 가상머신 등에 블록, 파일시스템, 오브젝트 스토리지 등을 제공합니다. </li>
        <li>Mold : 프라이빗 클라우드를 제공하기 위한 웹 기반 클라우드 플랫폼으로 셀프서비스를 통해 가상자원을 프로비저닝 합니다.</li>
        <li>Koral : Mold를 이용해 쿠버네테스 클러스터를 배포하여, 컨테이너를 통한 애플리케이션 프로비저닝을 지원합니다. </li>
      </ul>
    </p>
  </div>
</div>

#### 스토리지 구성요소

<div class="row">
  <div class="medium-12 column" style="padding:0 30px;">
    <p>
      <ul>
        <li>Volume : 가상머신에 블록 스토리지를 제공하고, 블록스토리지를 기반으로 멀티패스 iSCSI 스토리지를 제공합니다. </li>
        <li>Files : 멀티 세션을 지원하는 POSIX 표준을 따르는 파일 시스템을 제공합니다.</li>
        <li>Objects : 다수의 게이트웨이를 제공하는 페타 바이트 급의 비정형 저장공간을 제공 합니다.</li>
      </ul>
    </p>
  </div>
</div>

#### 네트워크 구성요소

<div class="row">
  <div class="medium-12 column" style="padding:0 30px;">
    <p>
      <ul>
        <li>Track : L3, L2, Load Balancer, Firewall, VPN 등의 네트워크 기능을 제공합니다. </li>
        <li>Atom : 보안그룹 정책을 통해 가상머신 간, 가상머신과 호스트 간의 모든 세부 트래픽을 제어합니다. </li>
      </ul>
    </p>
  </div>
</div>
<br/>

### 릴리즈 주요 내용
<br/>
ABLESTACK 1.0 Allo는 소프트웨어로 정의된 클라우드 데이터센터 구축을 위한 필수적인 구성요소를 제공하고, 특정 벤더에 대한 의존성을 최대한 제거하여 선택의 자유를 제공합니다. 이번 릴리즈는 다음과 같은 내용을 포함합니다.

<div class="row">
  <div class="medium-12 column" style="padding:0 30px;">
    <p>
      <ul>
        <li>모든 x86 서버에 운영체제 설치 미디어를 통해 쉽게 설치할 수 있도록 해 서버 제품 선택을 자유롭게 할 수 있습니다.</li>
        <li>운영체제 설치 미디어를 자유롭게 선택할 수 있습니다. 별도의 OS 전용 미디어를 사용할 수도 있고, 별도의 OS 파티션을 사용할 수도 있습니다. </li>
        <li>스토리지 전용으로 10G NIC 2개 포트 이상만 연결되어 있다면 바로 클라우드 환경을 구성할 수 있습니다. </li>
        <li>호스트별로 ABLESTACK 가상어플라이언스를 배포할 수 있는 배포 마법사를 제공하며, 배포 마법사를 통해 수분 내에 모든 구성요소의 배포가 가능합니다. </li>
        <li>호스트별로 ABLESTACK 랜딩 페이지를 통해 모든 어플라이언스 및 클러스터 상태를 모니터링할 수 있으며, 관리 플랫폼에 대한 바로가기를 제공합니다. </li>
        <li>호스트 및 클러스터, 클라우드, 스토리지 등의 모든 관리 기능을 웹 관리 플랫폼을 통해 관리할 수 있습니다. </li>
      </ul>
    </p>
  </div>
</div>

### 최소 실행 환경
<br/>
ABLESTACK을 이용해 기업에 클라우드 환경을 구성하기 위한 최소 실행 환경은 다음과 같습니다. 

#### 최소 호스트 수
<br/>
ABLESTACK은 고가용성을 제공하기 위해 **최소 3대**의 x86 CPU 기반의 랙 타입 서버가 필요합니다. 

#### 호스트 사양
<br/>
ABLESTACK 클러스터를 구성하는 x86 서버는 다음과 같은 사양을 만족해야 합니다. 

<table style="width: 100%">
  <caption>ABLESTACK 호스트 사양</caption>
  <colgroup>
    <col span="1" style="width: 20%;">
    <col span="1" style="width: 40%;">
    <col span="1" style="width: 40%;">
  </colgroup>
  <thead>
    <tr>
      <th>항목</th>
      <th>최소사양</th>
      <th>권장사양</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>CPU</td>
      <td>Intel Xeon Scalable CPU, <br/>2.0GHz이상 10Core 이상 1 Socket</td>
      <td>Intel Xeon Scalable CPU, <br/>2.0GHz이상 10Core 이상 2 Socket</td>
    </tr>
    <tr>
      <td>Memory</td>
      <td>96GB</td>
      <td>256GB</td>
    </tr>
    <tr>
      <td>ROOT Disk</td>
      <td>RAID5 Usable 300GB 이상</td>
      <td>M.2 RAID1 Usable 200GB 이상</td>
    </tr>
    <tr>
      <td>Local Cache Disk</td>
      <td>ROOT Disk를 공유하여 사용</td>
      <td>전용 SAS Type MU SSD 500GB 이상<br/>Persistent Memory 512GB 이상</td>
    </tr>
    <tr>
      <td>Glue Storage용 Disk</td>
      <td>SATA SSD 500GB 이상 1EA<br/>10K RPM SAS HDD 2TB 2EA</td>
      <td>SAS SSD MU 3.84TB 6EA</td>
    </tr>
    <tr>
      <td>관리용 NIC</td>
      <td>1GbE Mgmt 전용 NIC, IPMI 지원</td>
      <td>1GbE Mgmt 전용 NIC, IPMI 지원</td>
    </tr>
    <tr>
      <td>Guest NIC(이중화)</td>
      <td>1GbE 이상 2Port 이상</td>
      <td>외부 서비스용 1GbE 이상 2Port 이상<br/>가상머신간 통신용 10Gb SFP+ 2Port 이상</td>
    </tr>
    <tr>
      <td>Glue Storage NIC(이중화)</td>
      <td>10GbE 2Port</td>
      <td>스토리지 서비스용 10Gb SFP+ 2Port<br/>데이터 복제/복구용 10Gb SFP+ 2Port</td>
    </tr>
  </tbody>
</table>

<br/><br/>
{% include next-previous-post-in-category %}

<br/><br/>
<h3>제품 및 기능 릴리즈 카테고리의 다른 문서</h3>
<br/>
{% include list-posts entries='3' offset='0' category='Release' %}