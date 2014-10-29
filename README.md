# Laravel용 Noto Sans Korean 폰트

Google의 Noto Sans폰트에 대한 한국 폰트 웹폰트로 변환하여 Laravel용으로 패키지화 한것 입니다.

Noto Sans폰트는 [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0.html)을 따르고 있습니다.

폰트에대한 자세한 사항은 [Google Noto Fonts](https://www.google.com/get/noto/)에서 확인하세요.

## 설치법

개발프로젝트의 composer.json 파일의 require안에 다음을 추가합니다.

    "jeannedarc/laravel-notosans-korean": "1.0.*"

이제 프로젝트 디렉토리에서 다음 명령어를 실행하여, 패키지를 설치합니다.

    composer update

(폰트 용량이 큰 관계로 오래걸릴 수 있습니다.)

이제 이 패키지에 구성되어있는 asset들을  프로젝트로 가져올 차례입니다.

    php artisan asset:publish

## 사용법

실제로 사용하기 위해선, 이폰트를 사용하고자하는 페이지의 헤더에 다음과 같이 넣으세요.

    <link href='<?php echo asset("packages/jeannedarc/laravel-notosans-korean/css/fonts.css")?>' rel='stylesheet' type='text/css'>

혹은, import를 활용하여, css파일이나, style태그안에 다음을 넣어주셔도됩니다.

    @import url("packages/jeannedarc/laravel-notosans-korean/css/fonts.css");

그러고 나서, CSS의 font-family를 다음과 같이 변경하시면 폰트를 사용할 수 있습니다.

    body{
      font-family: "Noto Sans Korean", sans-serif;
    }

## 문의

기타 문의 사항은 jeannedarc0330@gmail.com으로 해주세요.
홈페이지는 제작하고 있습니다.
