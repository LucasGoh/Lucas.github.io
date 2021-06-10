---
title: 컴터 브라우저 광고 차단 && 키워드 search &&고급 검색 &&버전관리
tag: tech
toc: true
---

# 광고 차단

크롬을 사용하면 [여기](https://chrome.google.com/webstore/category/extensions?hl=en-US) 들어가서 ublock origin  다운하면 끝(대부분 광고 막을수 있다.)

Safari, firefox 유저는 extension / 扩展应用 / 확장프로그램 검색해서 찾아보고 다운한다.

# 키워드 search

브라우저 설정에 들어가서 검색을 누른다. 

키워드는 자기가 설정하고 싶은 대로 하고(가능하면 :영문 ), Query URL 은 구글, 네이버에 검색한다.

구글을 예를 들면 키워드는 :g 로 설정. Query URL 은 검색해서 찾아내고 http://*search*.*naver*.com/*search*.*naver*?*query*=%s 로 설정한다.

다음부터 구글 검색하려면 검색창에 :g 타자하고 space 누르면 바로 검색가능. 

자주 쓰는 사이트를 이렇게 해 놓으면 좋다. 나는 구글, 네이버, 바이두 등등 설정해 놓고 검색할 일이 있으면 쉽게 검색할수 있다.

# 고급검색

search operator / 상세검색 /고급검색 /연산자 / 高级搜索操作符

보다 정확하게 검색하기 위하여.  Google  baidu 많고 네이버는 적다.

기본 연산자

1. "":정확한 문구 찾기(nikola tesla)
2. |: 혹은
3. ():그룹 만들기 (tesla OR edision) alternating current
4. *: 아무 문자나 매치하기 (Tesla "rock * roll")
5. in: 100 dollar in krw



고급 연산자

1. intitle: Search only in the page's title for a word or phrase. Use exact-match (quotes) for phrases.
2. allintitle: 
3. inurl:
4. allinurl:
5. intext:
6. allintext:
7. filetype:
8. movie:



불안정 한 연산자

1. +:더하기 문자로 검색 결과 범위 좁히기(풍경사진 +유럽)
2. -:검색 결과에서 제외시키기 (풍경사진 +유럽 -스페인)



사용하는 예: 

영화를 찾고 싶은데 facebook youtube 영상들이 나온다.  movie:name -allinurl:facebook youtube



# mac 어플 버전관리

앱 스토어에서 응용을 다운하면 업데이트 하기 쉬운데, 그기 아닌 직접 다운한 경우 업데이트하기 쉽지 않다. 코드를 치는 터미널에 조금 익숙하다면 https://brew.sh/ 에 들어가서 프로그램 다운하고 버전관리 하면 된다. 응용 다운할때는 검색해서 다운하고 업데이트 할땐  brew update && brew doctor 하면 된다. 