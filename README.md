##  목차
1. [프로젝트 개요](#1-프로젝트-개요)
2. [프로젝트 범위](#2-프로젝트-범위) 
3. [기술 스택](#3-기술-스택)
4. [프로젝트 설치/실행](#4-프로젝트-설치-실행)
5. [핵심 기능 설명](#5-핵심-기능-설명)
6. [기타](#6-기타)

## 1. 프로젝트 개요
![nursedeu-highlight](https://github.com/seunghoonKang/nurseedu-frontend/assets/59612529/6e05d605-a0a5-441d-9a79-faba82b4be3c)


본 프로젝트는 널스에듀의 온라인 강의 수강을 위해 개발되었습니다.백오피스로 업로드한 동영상을 수강신청, 결제를 통해 수강할 수 있는 환경을 제공합니다.
* 외부 문제로 구현 사이트 기능 사용에 제한이 있습니다. 양해부탁드립니다.

<br>

## 2. 프로젝트 범위
1. **회원가입, 로그인**
    - AccessToken을 이용한 로그인 기능
    - 동시접속 제한 기능
    - 정규식 이용한 회원가입 유효성 검증

|   회원가입    |   로그인,로그아웃     |  
| :-------------------------: |  :-------------------------: | 
|![nurseedu_signIn](https://github.com/seunghoonKang/nurseedu-frontend/assets/59612529/c592c95a-ddc3-48fd-873a-57e8188be0fd)|![nurseedu_login_logout](https://github.com/seunghoonKang/nurseedu-frontend/assets/59612529/e292b00a-1638-4da5-ba93-df7e03ac609e) | 




2. **메인페이지**
    - 전체 강의 목록 조회
    - 검색 및 카테고리별 강의 목록 조회 

|  메인 카테고리, 검색    |  동시 접속 제한 |
| :-------------------------: |  :-------------------------: | 
|![nurseedu_search_category](https://github.com/seunghoonKang/nurseedu-frontend/assets/59612529/9b7c8566-d422-4f17-bff4-303ce8c3a647)| ![nurseedu_duplicate_access](https://github.com/seunghoonKang/nurseedu-frontend/assets/59612529/57fadc00-17db-4bab-af97-7bea8960b959)|






3. **강의 상세 페이지**
    - 강의 소개, 강의 목록 토글 형식 조회
    - 사용자 별 구매 이력에 따른 버튼, 동영상 보기 UI/UX



| 상세페이지 (탭 전환, 탭 유지) |  상세페이지 (강의 구매전) |
| :-------------------------: |  :-------------------------: |
|![nurseedu_detailpage_maintain_tap](https://github.com/seunghoonKang/nurseedu-frontend/assets/59612529/efcf0e5d-312b-494a-9e4c-87e67c3526d7)| ![nurseedu_detailpage_before_buy_lecture](https://github.com/seunghoonKang/nurseedu-frontend/assets/59612529/15ccaaf3-f8c3-4697-b240-c2661d75fe82) | 








| 상세페이지 (구매 - 결제) |  상세페이지 (강의 구매후) |
| :-------------------------: |  :-------------------------: |
|![nurseedu_from_detail_to_mypage](https://github.com/seunghoonKang/nurseedu-frontend/assets/59612529/4486bbee-d1d2-4797-a332-6e3e6d647be7)| ![nurseedu_detailpage_after_buy_lecture](https://github.com/seunghoonKang/nurseedu-frontend/assets/59612529/eb2eb317-97ef-4c60-ac92-199405dbea78) | 

4. **수강 신청 & 결제 페이지**
    - 상황에 맞는 API 호출로 마이페이지 UI 구현  
5. **마이 페이지**
    1. 내 강의 보기
        - 결제 완료된 강의 목록 조회
        - 진도율, 남은기간에 따른 수강 상태 변경
    2. 수강 신청 내역 
        - 수강 신청 후 결제 전 강의 목록 조회
6. **강의 시청 페이지**
    - 강의 목차 조회
    - 현재 수강중인 강의가 먼저 보이도록 구현
    - 강의 시청 기록 저장
        - 현재 수강중인 강의 완료 10초 전 시청 완료 처리 
    - 강의 시청 제한 
        - 강의 당 시청 시간 2배 시청 시 해당 강의 수강 불가 
    - 백오피스에서 설정된 위치의 워터마크 구현 

| 수강신청 - 결제 |  강의  |
| :-------------------------: |  :-------------------------: |
|![nurseedu_from_apply_lecture_to_buy_lecture](https://github.com/seunghoonKang/nurseedu-frontend/assets/59612529/393f97ac-fb3b-4b34-b646-a5a2decfa84b)| ![nurseedu_video_check_10sec](https://github.com/seunghoonKang/nurseedu-frontend/assets/59612529/b5470409-f122-4004-a770-67e31432eed3) | 




## 3. 기술 스택  
<div>
   <img src="https://img.shields.io/badge/NextJs-000000?style=for-the-badge&logo=nextdotjs&logoColor=white">
<img src="https://img.shields.io/badge/reactquery-FF4154?style=for-the-badge&logo=reactquery&logoColor=white">
  <img src="https://img.shields.io/badge/Typescript-3178C6?style=for-the-badge&logo=Typescript&logoColor=white">
  <img src="https://img.shields.io/badge/videojs-000000?style=for-the-badge">        
</div>

<div style='margin-top:10px;'>
<img src="https://img.shields.io/badge/antdesign-0170FE?style=for-the-badge&logo=antdesign&logoColor=white">
        <img src="https://img.shields.io/badge/axios-5A29E4?style=for-the-badge&logo=axios&logoColor=white">
  <img src="https://img.shields.io/badge/recoil-3578e5?style=for-the-badge&logo=recoil&logoColor=white">
    <img src="https://img.shields.io/badge/styledcomponents-DB7093?style=for-the-badge&logo=styledcomponents&logoColor=white"> 
</div>
<br>

  
  |   언어   |  버전   |   
  |:-------:|:------:|
  |  Typescript |   5.0.4  |
  
  |   프레임워크   |  버전   |   
  |:-------:|:------:|
  |  NextJs |   13.3.0  |
  
  |   라이브러리   |  버전   |   
  |:-------:|:------:|
  |  react |   18.2.0  |
  |  react-query |   3.39.3  |
  |  recoil |   0.7.7  |
  |  video.js |   7.17.0  |
  |  styled-components |   5.3.9  |
  |  axios |   1.3.6  |
  |  ant-design |   5.4.4  |
 
## 4. 프로젝트 설치-실행

```
$ git clone https://github.com/DevCamp-TeamSparta/nurseedu-frontend.git
$ cd nurseedu-frontend
$ yarn install && yarn run dev
```

## 5. 핵심 기능 설명

<details>
<summary><strong>✅ 워터마크 위치 지정</strong></summary>
    
<div markdown="1">

- 백오피스에서 강의별로 설정한 좌측상단 ~ 우측하단 9군데 위치 중 한 곳에 워터마크 표기.
- video div를 `position: relative` 로 두고, video가 생성됐을 때 설정된 위치에 `position: absolute`로 워터마크 위치 지정 (default: 우측 상단)
    
```tsx
const WatermarkLocationName = {
  TOP_LEFT: "TOP_LEFT",
  TOP_CENTER: "TOP_CENTER",
  TOP_RIGHT: "TOP_RIGHT",
  MID_LEFT: "MID_LEFT",
  MID_CENTER: "MID_CENTER",
  MID_RIGHT: "MID_RIGHT",
  BOTTOM_LEFT: "BOTTOM_LEFT",
  BOTTOM_CENTER: "BOTTOM_CENTER",
  BOTTOM_RIGHT: "BOTTOM_RIGHT",
};    
```
### 백오피스 워터마크 위치 설정
![backoffice_watermark_setting_1](https://github.com/DevCamp-TeamSparta/nurseedu-frontend/assets/59612529/3d528cf0-1a2f-42f3-874c-da08dce53fd6)
![backoffice_watermark_setting_2](https://github.com/DevCamp-TeamSparta/nurseedu-frontend/assets/59612529/11ac854d-0d5d-4d8a-b1ac-c1e265469f87)

### 프론트 워터마크 위치 확인
![front_watermark_setting_1](https://github.com/DevCamp-TeamSparta/nurseedu-frontend/assets/59612529/54c1522b-66ab-4b71-ae4c-22ccdc03fe47)


</div>
</details>


<details>
<summary><strong>🙅 로그인 유지</strong></summary>
    
<div markdown="1">
    
- accessToken, useQuery, Recoil을 이용하여 로그인 상태 유지
- hook으로 작성하여, 로그인 상태가 필요한 부분에만 사용 가능
    

    
```tsx
import { useQuery } from "react-query";
import { useResetRecoilState, useSetRecoilState } from "recoil";
import { userInformation } from "../../shared/atoms";
import { getUserInformation } from "@/_helpers/axiosapi";
import { getCookie } from "@/_helpers/getcookie";

export const useUser = () => {
  const setUserInfor = useSetRecoilState(userInformation);
  const resetUerState = useResetRecoilState(userInformation);
  const accessToken = getCookie("accessToken");

  if (!accessToken) {
    resetUerState();
  }

  return useQuery(
    ["userInfo"],
    async () => {
      const response = await getUserInformation();
      setUserInfor(response);
    },
    {
      enabled: !!accessToken,
    }
  );
};
```
</div>
</details>

## 6. 기타
<details>
<summary><strong>useQuery select를 통한 필터링</strong></summary>
    
<div markdown="1">
- 메인 페이지의 전체 목록이 1개 이상의 카테고리를 가져 중복된 데이터를 불러오기에 처음 useQuery에서 select를 통해 필터링.

```tsx
const useGetFilteredCourses = () => {
  const { data, isLoading } = useQuery(
    ["getFilteredCoursesDatas"],
    getCourses,
    {
      select: (items) => {
        const uniqueCourses = new Set();
        const deduplicatedItems = items.reduce((result: any, item: any) => {
          const { id, name, courseCategories } = item;
          const uniqueCategories: any = [];

          courseCategories.forEach((category: any) => {
            const { id: categoryId, course } = category;
            if (!uniqueCourses.has(course.id)) {
              uniqueCourses.add(course.id);
              uniqueCategories.push({ id: categoryId, course });
            }
          });

          result.push({ id, name, courseCategories: uniqueCategories });
          return result;
        }, []);

        return deduplicatedItems;
      },
    }
  );
  return { data, isLoading };
};
```

### 중복제거된 목록
- 카테고리에는 한 강의가 2개 이상의 카테고리를 가질 수 있기에 2, 1, 2, 1 로 표기됨
![nurseedu_main](https://github.com/DevCamp-TeamSparta/nurseedu-frontend/assets/59612529/4ba87842-e9ba-450f-bfa3-ad75588c6487)

</div>
</details>
