# nuxt-firebase

firebase hosting 과 firebase functions 에 배포하는 universal nuxt project

## Pre requirements
- [firebase tools][firebase-tools] 를 설치합니다.
  > npm i -g firebase-tools
- [파이어베이스 콘솔][[firebase-console]] 에서 firebase 프로젝트를 생성하고 project id를 `.firebaserc` 의 projects 항목 아래 적어넣습니다.

  ```json
  {
    "projects": {
      "default": "your-firebase-project-id"
    }
  }
  ```
- 콘솔에서 firebase 에 로그인합니다.
  > firebase login

## Development

nuxt 페이지를 개발할 때는 `src/` 디렉토리 아래서 `npm run dev` 명령을 실행하여 빠르게 개발합니다.  
> npm run dev

배포 전에 firebase functions가 잘 동작하는지 확인하기 위해서는 프로젝트 루트 디렉토리에서 `firebase serve` 명령을 통해 functions를 에뮬레이션합니다.
> firebase serve --only functions

개발이 끝나고 배포할때는 `firebase deploy` 명령으로 배포합니다
> firebase deploy -m"첫번째 릴리즈"

[firebase-tools]: https://firebase.google.com/docs/cli/
[firebase-console]: https://console.firebase.google.com/u/0/
