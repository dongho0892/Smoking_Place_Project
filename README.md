## 멋사 프로젝트 회의록 & 진행상황

### 날짜 : 18.07.10

##### 참여자 : 				파티장 : 동규   		파티원 : 동호

##### 팀           명  : 스무브(Smoking Move (이동)

##### 아이디어명 : 흡연 구역 알리미

##### 회의 내용 :

```ruby
프로젝트 전체 흐름 구상
```

![18.07.10 - routes](D:/%EB%A9%8B%EC%82%AC%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/%EC%A0%9C%EC%9E%91%20%EA%B3%BC%EC%A0%95/18.07.10%20-%20routes.jpg)

![18.07.10 - 모델링, DB 구조](D:/%EB%A9%8B%EC%82%AC%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/%EC%A0%9C%EC%9E%91%20%EA%B3%BC%EC%A0%95/18.07.10%20-%20%EB%AA%A8%EB%8D%B8%EB%A7%81,%20DB%20%EA%B5%AC%EC%A1%B0.jpg)

![18.07.10 - 유저용 view 흐름](D:/%EB%A9%8B%EC%82%AC%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/%EC%A0%9C%EC%9E%91%20%EA%B3%BC%EC%A0%95/18.07.10%20-%20%EC%9C%A0%EC%A0%80%EC%9A%A9%20view%20%ED%9D%90%EB%A6%84.jpg)

![18.07.10 - 관리자용 view 흐름](D:/%EB%A9%8B%EC%82%AC%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/%EC%A0%9C%EC%9E%91%20%EA%B3%BC%EC%A0%95/18.07.10%20-%20%EA%B4%80%EB%A6%AC%EC%9E%90%EC%9A%A9%20view%20%ED%9D%90%EB%A6%84.jpg)





해야할 일

```ruby
1. 페이지 만들어야할 것 목록 정리


1. 챗봇 기본 기능 구현하기			( 카톡 플친 + 버튼 구현 완료)
	- 메인 인사말 / 기능 1,2,3 구현하기 / 링크 연결시켜 주기 


********************

   
1. 카톡 플러스친구 헤로쿠에다가 작업 내용 서버 업로드
2. (위도, 경도) 자료 반복문 형식으로 넣기 (.each / all)
3. 메인 웹페이지 만들기
4. 등록(흡연 / 단속) 웹페이지 만들기

1. 페이지 만들어야할 것 목록 정리




[ 프로젝트 마무리 시점에 세부 조정 사항]
1. csv 자료 위도 경도 안맞는 문제 (해결함)
 - 주소 정확한 것 => 위도 경도 추출 (구 지번 주소로 검색)
				: https://brunch.co.kr/@yeowoonbae/4 (구글 스프레드 시트 이용)
 - 지하철 출구 정보 => 공공 데이터 포털 (철도공사 쪽 이용 예정)
 - 어린이집 : APT에 있는 곳 => 동까지 위치 조정해줘야함.
```





















##### 완료 한 일

```ruby
0. https://dongho0892.github.io/ 상에 화면 띄워주기
1. 발표용 웹사이트 구현 완료
(동호)
	- 첫 화면 / Services / About / Team / Contact
2. Geolocation을 이용한 위도 경도 받아오기 + 지도 상 보여주기 구현 성공.
(동규)

3.(06/21)
Portpolio 사진 6개 만들기
(동규)
	- 1.챗봇 : 메시지 형식으로 인사 + 우리가 제공하는 3가지 기능을 버튼으로 보여주기
			: 버튼이나 채팅으로 응답!
			( 3가지 기능 : 지도 관련 / 흡연 장소 등록 / 단속 장소 등록)
			( 지도 관련 : 내위치 -> 가까운 지도 -> 길찾기 순서로 대화 설정 할 예정)
	- 2. 챗봇 : 지도 띄워주기 ( 채팅창에서 )
			( 채팅창 상에서 지도를 움직 일 수 있게끔 (다른 링크 가는 것 없이) )
			( => else 웹페이지로 링크 연결하기)
	- 3. 모바일용 웹  : 카톡 로그인 화면 (썸네일) 
			+  웹 페이지 첫번째 화면 (본화면) 
			( 4가지 항목 : 지도보기 / 카톡 로그인하기 /  흡연 장소 등록 / 단속 구역 등록 )
(동호)
	- 4. 모바일용 웹 : 흡연 / 단속구역 등록 페이지 
				( 지도찍기 / 검색하기 / 지역명 / 위도 경도 / 사진 업로드 )
	- 5. 모바일용 웹 : 지도 기본창 화면
	- 6. 모바일용 웹 : 지도 길찾기 기능 구현 이미지

------------------------------------------------------------------------------------------------
    
3. (06/21) 팀명 정하기 : 스무브(Smoking Move (이동))
4. (06/21) 아이디어명 : 흡연 구역 알리미
5. (06/21) 밴드에 팀명 / 아이디어명 올리기 
6. (06/21) 밴드에 있는 PPT 파일 정리해서 메일로 보내기.
    (동규) : PPT 초안 작성
    (동호) : PPT 초안 수정 및 전송

2-1. (06/21) 발표 페이지 수정하기
(동호)
	- 1. Portfolio 위치 수정 :  1  2 3 3 4 5 6 
    	 1. 챗봇 첫화면 -> 2. 챗봇 지도 띄워주는 화면 -> 3. 웹 로그인 화면 (썸네일) + 웹 첫화면
		 4. 장소 등록 화면 -> 5. 웹 지도 첫 화면 -> 6. 웹 지도 길찾기
(동규)
	- 2. 맨 위 start bootstrap 문구 수정하기
	- 3. Portfolio 위의 배너 생성해서 유저 이해도 높히기.  (취소)
	- 4. Service 3개의 이모티콘 변경

------------------------------------------------------------------------------------------------
3. 발표 준비
4. 발표 준비 완료
------------------------------------------------------------------------------------------------

챗봇으로 구현 가능한지 확인해보기 -> 지도 뿌려주는 것 등 어려울 것으로 예상됨. = 방화벽 문제 확인(동규)

카카오톡 플러스 친구 개설
다음지도 API 사용해서 C9 에서 지도 만들어보기

------------------------------------------------------------------------------------------------

금연구역 자료가 위도, 경도가 안맞음. => 강남구 전체에서 일부구역으로 축소 XX (기존안 대로함)
		=> 위도 경도 : 기존 지번주소로 하니까 조정됨. 
( 어린이집, 택시승차장, 지하철 출구 등만 프로젝트 마무리 때 조정해주기)

------------------------------------------------------------------------------------------------
4. 다음지도 API로 금연구역 표시해보기. => 위도 경도 자료 넣어서 원 / 사각형 구현 완료.
2. 전체 구조 모델링 하기
------------------------------------------------------------------------------------------------
전체 흐름 파악 완료
routes 파악 완료
```



##### 과거 회의 내용

```
1. 팀명 / 아이디어명 정하기
2. 발표 자료 마무리 짓기

------------------------------------------------------------------------------------------------


```



##### 특이사항

```기타
모든 지도는 챗봇에서 바로 이용할 수 있도록 할 것
우리의 주 포커스는 챗봇으로 구현 하는 것
	- 웹을 만드는 것은 등록 기능만 하되,
	- 챗봇으로 지도를 보여주는 것이 어려울 경우에 웹페이지로 만들어서 링크를 걸어줄 것.
	
	
JSON, Node.js, JavaScript 공부가 필요함... : 왓슨 챗봇, 카톡, 루비연결.. 	
```



##### 느낀점

```동호
 - 
```



##### 시행착오

```
의견 충돌 (06.20)
- 구현하고자 하는 예시 이미지 선정 과정 
- 각자의 구현하고자 하는 방향이 조금 달랐음 
		: 동규는 챗봇을 100%로 생각 / 나는 챗봇 50% 웹 50% 생각했는데, 그것 때문에 웹페이지 용도에 대한 이해가 달랐음. -> 동규는 웹페이지는 등록 용도로만 / 동호는 웹페이지는 등록, 지도보기 등 모든 것을 구현 되게끔 하려고 함 (+ 챗봇으로 구현 안 됬을 경우를 위해 만드려는 목적도 있음)

=> 둘의 이해를 합치고, 내 웹페이지 구현은 챗봇으로 구현이 안되는 경우에 한해서 차선책으로 만들기로 합의

------------------------------------------------------------------------------------------------

챗봇 구현의 어려움 (06.25)
 - 카카오톡 플러스친구를 개설했으나, 챗봇과 연결하는 것이 어려움. 
 - 대화 하는 것도 자유롭지 않고 제한이 많음. 이 것을 어떻게 해결해 나갈 것인가...?


--------------------------------------------------------------------------------
공공데이터 포털 상에 위도, 경도 데이터가 안맞음
 => 구글 스프레드시트의 geocode 이용 => 위도 경도 안맞는 문제 = 도로명 주소 때문으로 파악됨. 2시간 내내 데이터 가공 함.... 좌절.. 코드를 짜서 뭔가 할 수 없는 이 현실..
 슬프도다... 그래도 다행히 데이터는 그대로 쓸 수 있을 것 같다
 
```

