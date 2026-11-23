# 📚 리드픽 (ReadPick) - 스마트 모바일 독서 추천 PWA

> **"왓챠피디아의 까다로운 별점과 교보문고의 실구매 독자 평점을 한곳에서!"**  
> 전자책(eBook)과 독서를 사랑하는 독서가를 위해 스마트폰 최적화 UI로 설계된 스마트 도서 큐레이션 웹/PWA 애플리케이션입니다.

**공식 배포 주소**: [https://kig0402.github.io/readpick](https://kig0402.github.io/readpick)

---

## 📱 PWA (Progressive Web App) 앱 설치 방법

이 웹사이트는 **PWA 표준**을 완벽하게 준수하여 제작되었으므로, 별도의 앱스토어 설치 과정 없이 스마트폰과 PC의 크롬 브라우저에서 바로 앱으로 설치하여 사용할 수 있습니다.

### 1. 모바일 크롬 (Android / iOS)
- `https://kig0402.github.io/readpick` 접속
- 화면 상단에 자동으로 나타나는 **[리드픽 앱 설치하기]** 배너에서 **[설치]** 클릭
- 또는 브라우저 상단 우측 메뉴(⋮)에서 **[앱 설치]** 또는 **[홈 화면에 추가]** 터치
- 스마트폰 홈 화면에 리드픽 아이콘이 생성되며, 브라우저 주소창 없이 **순수 네이티브 앱**처럼 전체 화면으로 구동됩니다.

### 2. PC / Mac 크롬 (Chrome / Edge)
- 주소창 우측 상단의 **[설치 아이콘(💻↓)]** 클릭 또는 상단 헤더의 **[앱 설치]** 버튼 클릭
- 독립된 데스크톱 앱 창으로 실행됩니다.

---

## 🌟 핵심 기능 요약

1. **왓챠피디아 × 교보문고 평점 교차 검증 (더블 체크)**
   - **왓챠피디아**: 5.0점 만점 기준 별점, 평가자 수, 감성 키워드 및 리뷰 태그.
   - **교보문고**: 10.0점 만점 실구매 독자 평점, 리뷰 개수, 구매 만족도 지수(%).
   - 두 플랫폼의 정규화 평점 비교 게이지 및 "더블 골든 추천(만장일치 명작)" 배지 제공.

2. **도서 상세 정보 & 교보문고 원클릭 링크**
   - 3D 책등 효과 북커버, 출판사, 쪽수, 핵심 인용구, 줄거리 요약.
   - 각 도서마다 교보문고 검색/상세 페이지로 연결되는 직접 링크 탑재.
   - 전자책(eBook) 지원 여부 배지 표기.

3. **다양한 큐레이션 & 랭킹 시스템**
   - **요즘 화제의 베스트셀러 순위**: 실시간 베스트셀러 1위~12위, 순위 변동 추이(NEW, ▲1, -) 표시.
   - **스테디셀러 컬렉션**: 오랜 세월 검증받은 불멸의 명작 모음.
   - **장르별 평점 TOP 추천**: 소설, 인문/철학, 자연과학, 에세이/심리, 경제/경영 등 장르별 필터 및 정렬 기능.
   - **빠른 평점 필터링**: 왓챠 4.2★ 이상, 교보 9.7★ 이상, 전자책 지원 도서만 골라보기.

4. **오프라인 지원 및 캐싱 (Service Worker)**
   - 네트워크 연결이 불안정하거나 오프라인 상태에서도 핵심 기능과 캐시된 도서 정보를 안전하게 조회할 수 있습니다.

5. **내 서재 & 독서 관리 (LocalStorage 연동)**
   - 읽고 싶은 책 (찜하기), 읽는 중인 책, 완독한 책 분류 저장.
   - 독서 통계 대시보드 (상태별 권수 실시간 반영).

---

## 🚀 GitHub 저장소 및 GitHub Pages 배포 가이드

### 1. 로컬 저장소 커밋
```bash
cd "C:\Users\user\.gemini\antigravity\scratch\book-recommend-app"
git init
git add .
git commit -m "feat: ReadPick PWA v1.0 initial release"
```

### 2. GitHub 원격 저장소 연결 및 푸시
```bash
git branch -M main
git remote add origin https://github.com/kig0402/readpick.git
git push -u origin main
```

### 3. GitHub Pages 활성화
1. GitHub에서 [https://github.com/kig0402/readpick](https://github.com/kig0402/readpick) 저장소로 이동합니다.
2. **Settings** 탭 -> 좌측 메뉴의 **Pages** 클릭.
3. **Build and deployment** 섹션의 **Branch**를 `main`, 폴더를 `/ (root)`로 선택하고 **Save** 클릭.
4. 약 1~2분 후 [https://kig0402.github.io/readpick](https://kig0402.github.io/readpick) 주소로 웹과 PWA가 실시간 배포됩니다.
