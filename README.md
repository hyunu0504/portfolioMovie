
  ## PC
</br>
<table>
  <tr> 
    <td width = "50%" valign="top"><b>메인페이지</b><img src="https://user-images.githubusercontent.com/105877042/216832762-dd63d876-422c-49e3-b64b-7e638ddb0785.JPG"/></td>
    <td width = "50%" valign="top"><b>상세페이지</b><img src="https://user-images.githubusercontent.com/105877042/216832772-ba50f448-76fe-4ef7-9558-de14ae29ebcf.JPG"/></td>
  </tr>
</table>
</br>
</br>
</br>

  ## 모바일
</br>
<table>
  <tr> 
    <td width = "50%" valign="top"><b>메인페이지</b><img src="https://user-images.githubusercontent.com/105877042/216832776-4d415af9-f319-4214-bd8d-b94918d631c2.JPG"/></td>
    <td width = "50%" valign="top"><b>상세페이지</b><img src="https://user-images.githubusercontent.com/105877042/216832780-4fc608f1-cf3c-4176-bfaa-6ec2cf3be8e7.JPG"/></td>
  </tr>
</table>
</br>
</br>
</br>


## 프로젝트 과정

TMDB에서 제공하는 API를 사용하였습니다.

제공하는 API의 정보를 보고 현재 상영 중, 상영 예정작, 인기 영화를 보여주고 검색할 수도 있고

영화를 클릭했을 때 해당 영화의 상세정보를 보여주는 사이트를 만들고자 했습니다.

useEffect를 사용해서 불필요한 렌더링이 안생기도록 했습니다.

useContext로 데이터를 관리했습니다.

영화 상세 페이지에서 새로고침할 때  클릭한 영화의 ID값이 초기화 되는것을

local storage에 담아서 새로고침해도 보이도록 했습니다.

깃헙은 SPA를 지원하지 않는다는 것을 모르고 새로고침을 했더니 404에러가 떠서

react-route-dom의 Browserrouter를 Hashrouter로 변경해서 해결했습니다.

## 검색창
<ul>
<li>검색을 클릭할때 useRef로 검색창에 focus를 설정했습니다.</li>
<li>영화 검색은 최대 18개의 영화가 검색되도록 그리고 이미지가 없는 영화는 검색되지 않도록 했습니다.</li>
</ul>

## 현재 상영중, 상영 예정작, 인기 영화
<ul>
<li>component를 재활용 했습니다.</li>
<li>제목, 줄거리가 일정칸을 넘을시 ...처리 했습니다.</li>
</ul>

## 상세페이지
<ul>
<li>현재 영화의 주요정보 ( 줄거리, 감독, 장르, 영화 시간, 개봉일, 평점을 볼 수 있습니다) </li>
<li>스틸컷에서 포스터를 클릭하면 이미지를 보여주고 배경을 다시 클릭하면 이미지를 숨깁니다.</li>
<li>출연진의 프로필을 보여주고 이미지가 없는 경우에는 기본 프로필을 보여줍니다.</li>
<li>일정 스크롤을 내리면 header와 제목 탭을 보여주고 더 내리면 주요정보, 스틸컷, 출연진 탭을 보여줍니다. </li>
</ul>

## 디자인
<ul>
<li>가로 1023px, 600px 이하에서 반응형 디자인을 구현하고, styled-components를 사용했습니다.</li>
</ul>

## 라이브러리
<ul>
<li>추천 영화 이미지 슬라이더는 리액트 라이브러리 Swiper를 사용했습니다.</li>
<li>
react-spinners 라이브러리를 사용해서 현재 상영중, 상영 예정작, 인기 영화, 추천 영화에 로딩화면을 구현 했습니다. </li>
</ul>


