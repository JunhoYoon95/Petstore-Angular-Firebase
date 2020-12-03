# Junmannn's 개발 노트
### Angular 프로젝트 생성
* terminal : ng new petstore
-> SCSS로 선택
***
### Angular material 다운로드 - 많은 material들을 가져오는 것임.
* termnial : ng add @angular/material

angular material 페이지 -> https://material.angular.io/components/categories  
***

### Angular material - slider 을 import 하기.  
https://material.angular.io/guide/getting-started
***

### Angular module이 많아서 app.modules.ts에 하나하나 가져오기 너무 비요율적이다. 모듈 폴더를 만들어 한 번에 관리하고 import 하자
* terminal : ng generate module modules/angular-material

모듈을 만드는데 modules 라는 곳에 angular-material 이라는 폴더를 만든거지.
***

### material 폴더를 만들고 안의 내용을 이것으로 대체
https://www.creapple.com/
그 폴더 자체를 가져오는걸로 app.module.ts, angular-material.module.ts 고치고 

app.component.html로 이동해서 추가해
usage : https://material.angular.io/components/checkbox/examples

[(ngModel)]="checked" 부분은 빼라
***

### Angular schematics
https://material.angular.io/guide/schematics
이 중에서도 navigation을 설치할거야
* terminal : ng generate @angular/material:navigation <component-name>
  usage : ng generate @angular/material:navigation --name=nav
이름을 nav라고 지은 것 뿐이고, 저 이름은 아무거나 바꿔도 상관은 없겠지
* 생성된 nav 폴더 안에 nav.component.ts 파일을 보면 @component에 selector: 'app-nav'라고 쓰여있다. 이 이름이 다른 곳에서 이 navigation을 불러오는 이름이다.
이걸 대표 화면인 app.component.html 에서 불러봐야지
* 얘 하면 친철하게 app.module.ts에 또 더 가져오는데 나는 이걸 wrapper 로 묶어놨기때문에 지워줘도 된다.

***
## Firebase
https://firebase.google.com/

noSQL기반 으로 사용을 할 거다.

JSON(Javascript Object Notation)형태로 저장이 된다.

structure : noSQL기반의 JSON데이터 형태. + Realtime Database(하나의 커다란 JSON tree형태), key를 생성해줌



***




***






# AngularPetstore

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 11.0.2.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.


