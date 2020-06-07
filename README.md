# golang_basic

golang 설치하기 

0. 
bin: 바이너리 파일, 실행파일
pkg : 패키지 오브젝트 파일
     소스가 컴파일된 후 코드들. 실행가능한 파일은 아님
     라이브러리가 들어감
src: 소스코드가 들어감 

1. go get golang.org/x/tools/cmd 
- 필요한 명령 도구들 설치 (위치 : GOPAHT/bin ) 
- 해당 명령어를 실행하면 GOPATH 에 bin, pkg,src 디렉터리가 생성됨. 
cf. 필요한 도구만 설치하기
ex) go get golang.org/x/tools/cmd/goimports
: 모든 도구를 설치하지 않고, goimports만 설치하기 



2. 기본명령어 
1) gofmt -w helloworld.go
2) goimports -w helloworld.go
3) go run helloworld.go 
   : go 파일 실행하기 
     굳이 작업 공간 디렉터리 사용 ㄴx
4) go install github.com/dev-hy-joy/helloworld
  : 파일 설치하기 
    제대로 된 디렉터리가 들어가야 함 
    가정 : github.com/dev-hy-joy/helloworld/helloworld.go
    bin 폴더에 helloworld.exe 실행파일이 생김 
    
3. 패키지 & 라이브러리 
디렉터리 하나가 한 패키지
한 패키지는 메인패키지 or 라이브러리패키지 
그러나 메인패키지와 라이브러리패키지를 같은 위치에 둘 수 없음. 
메인패키지를 설치하면 (go imports명령어) --> 관련 라이브러리도 컴파일 됨 




reference : 디스커버리 Go 언어 (염재현 저)
