---
layout: page-fullwidth
show_meta: false

title: "지원 문의"

teaser: "<br/>ABLESTACK 전체 제품에 대한 기술지원 및 데모지원 서비스를 제공합니다. 다음의 양식에 기술지원 요청 내용을 작성하신 후 이메일을 보내면 담당자 확인 후 회신하여 드립니다. "
permalink: "/contact_mail/"
---


<form name="sentMessage" id="contactForm" novalidate action="https://formspree.io/f/mzbygdrk" method="post">
    <input type="hidden" name="_subject" value="새로운 기술지원 요청이 있습니다." />
    <input type="text" name="_gotcha" style="display:none" />
    <div class="control-group">
        <div class="form-group floating-label-form-group controls">
        <label>이름 : </label>
        <input type="text" class="form-control" placeholder="이름을 입력하세요." id="name" name="name" required data-validation-required-message="">
        <div class="help-block text-danger"></div>
        </div>
        <div class="form-group floating-label-form-group controls">
        <label>이메일 : </label>
        <input type="email" class="form-control" placeholder="이메일 주소를 입력하세요." id="email" name="email" required data-validation-validemail-message="" data-validation-required-message="">
        <div class="help-block text-danger"></div>
        </div>
        <div class="form-group floating-label-form-group controls">
        <label>기술지원요청 내용</label>
        <textarea rows="5" class="form-control" placeholder="기술지원을 요청할 내용을 입력하세요. 요청 구분(제품소개, 데모요청, 기술지원), 회사, 담당자, 기술지원요청 목적 등을 명확하게 알 수 있도록 작성해 주십시오. 내용 확인 후 바로 회신 드리겠습니다." id="message" name="message" required data-validation-required-message=""></textarea>
        <div class="help-block text-danger"></div>
        </div>
    </div>
    <br>
    <div id="success"></div>
    <div class="form-group">
        <button type="submit" class="btn btn-primary" id="sendMessageButton">기술지원요청 이메일 보내기</button>
    </div>
</form>