유닉스 팀프로젝트 사물함 시스템 (학교 유닉스프로그래밍 프로젝트)
--------------------------------------

1)팀원

-박범진

º 서버의 전체적인 부분 담당

º 서버 부분 기본기능 구현

º 비밀번호 변경 기능 구현

-김태연

º 클라이언트의 전체적인 부분 담당

º 클라이언트 부분 기본기능 구현

º 비밀번호 2차확인 기능 구현


2)구현기능

º 사용자에게 사물함에 대한 정보를 제공

º 패스워드 지정 및 패스워드 확인

º 원하는 사물함에 접근

º 해당 사물함의 비밀번호 설정

º 서버 시작 시 사물함 개수 설정

º 서버 시작 시 비밀번호 길이 설정

º 비밀번호 설정 시 비밀번호 2차확인

º 잠근 된 사물함 접근 시 언락, 비밀번호 변경, 나가기 중 선택




3)전체흐름

![1](https://user-images.githubusercontent.com/87348209/146746868-122a61cd-8a45-46a9-8269-0d7ba38d090d.PNG)

서버 시작 시 사물함의 수와 비밀번호의 자릿수를 설정.

![2](https://user-images.githubusercontent.com/87348209/146746937-813ed4aa-948e-475e-a49a-b43d8fd9fd7b.PNG)

서버와 클라이언트가 연결되면 서버에서 사물함 구조체 배열에 저장된 is_available에 있는 문자열
을 클라이언트에게 넘겨주고 출력.

![4](https://user-images.githubusercontent.com/87348209/146747015-e0331484-d694-481a-ad60-3719b43e9157.PNG)

비어 있는 사물함에 접근하게 되면 비밀번호를 입력 받게 되고, 비밀번호 자리수가 맞는지, 재입
력 받은 비밀번호와 일치 하는지 검사 후 비밀번호를 설정하게 되고 사물함의 상태를 사용 중으
로 바뀜.

![5](https://user-images.githubusercontent.com/87348209/146747111-965d6730-6774-432a-8773-eb509885e5bb.PNG)

사용중인 사물함에 접근 시 설정된 비밀번호를 확인하게 되고, 설정된 비밀번호와 같으면 잠금
해제, 비밀번호 변경, 나가기 중에 선택을 할 수 있고, 1번 선택 시 사물함을 비우게 되고 2번 선
택 시 새로운 비밀번호를 입력 받아 저장하게 됨.
