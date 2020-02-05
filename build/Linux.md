# Build

## console

` $ cd m-lang-helper # move to myExtension project `
` $ vsce package # myExtension.vsix generated (package.json 파일의 version 정보를 먼저 수정해 줄것) `
` $ vsce publish # <publisherID>.myExtension published to VS Code MarketPlace `

- 참조: https://code.visualstudio.com/api/working-with-extensions/publishing-extension 

> vsce package 실행시, Publisher관련 에러가 나오면,  
  먼저 publicer를 vsce에서 생성해야되며, 
  Publisher를 생성 후, Publisher ID를 package.json 파일에 추가해주어야 함.


## VS Code 개발 지원 툴 설치

- VS Code에서 Console창을 열고 Util 폴더로 이동 후, 아래 명령어를 입력
> ` $ code --install-extension moca-lang-0.X.X.vsix `

- mac에서 'code: command not found'와 같은 에러가 발생한 경우
  * VS Code에서 Command Palette (⇧⌘P)를 열고, 'shell command'라고 입력
  * Shell Command: Install 'code' command in PATH 명령을 찾아 클릭하여 실행
  * VS Code를 재시작함
