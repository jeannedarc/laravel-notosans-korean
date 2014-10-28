# Noto Sans Korean Font Bundle for Laravel

Google의 Noto Sans폰트에 대한 한국 폰트 웹폰트로 변환하여 Laravel용으로 패키지화 한것 입니다.
Noto Sans폰트는 [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0.html)을 따르고 있습니다.
폰트에대한 자세한 사항은 [Google Noto Fonts](https://www.google.com/get/noto/)에서 확인하세요.

## 설치 및 사용법

개발프로젝트의 composer.json 파일에 다음을 추가합니다.
require가 이미 있다면 그안의 내용만 넣어주세요.

    "require": {
        "jeannedarc/laravel-notosans-korean": "~0.1"
    }

이제 다음 명령어로 패키지를 설치합니다.

    composer update

실제로 사용하기 위해선, 이폰트를 사용하고자하는 페이지의 헤더에 다음과 같이 넣으세요.

    <link href='<?php echo asset("packages/jeannedarc/laravel-notosans-korean/css/fonts.css")?>' rel='stylesheet' type='text/css'>

혹은, css import를 활용하여, css파일에

    @import url("../packages/jeannedarc/laravel-notosans-korean/css/fonts.css");

와 같이 넣어 주셔도 됩니다.