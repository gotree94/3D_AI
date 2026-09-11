# 게임 개발자 & 크리에이터를 위한 3D AI 도구 가이드

> 게임 개발자, 애니메이션 작가, 콘텐츠 크리에이터, 그래픽 아트 창작자의 작업 효율과 속도를 높여주는 3가지 도구

---

## 1. Luma Labs Genie — Text-to-3D AI

### 개요

Luma Labs에서 개발한 **Genie**는 텍스트 프롬프트만으로 3D 모델을 생성하는 AI 도구입니다. ChatGPT처럼 텍스트를 입력하면 약 **10초 이내**에 완성된 3D 오브젝트가 생성됩니다.

### 주요 특징

| 항목 | 내용 |
|------|------|
| **입력 방식** | 텍스트 프롬프트 (최대 400자) |
| **생성 시간** | 약 10초 (기본), HD 업스케일 시 추가 시간 |
| **출력 포맷** | GLB, FBX, OBJ, USDZ |
| **호환 소프트웨어** | Blender, Unity, Unreal Engine 등 |
| **대상 사용자** | 게임 개발자, 프로덕트 디자이너, 건축가, 3D 아티스트 |

### 사용 방법

1. **Luma 웹 플랫폼** 접속: https://app.lumalabs.ai (Genie 기능이 통합됨)
2. 또는 **Discord 서버**에서 봇 명령어로 사용 가능
3. 텍스트 프롬프트 입력 (예: "a medieval castle with torches")
4. 약 10초 후 4개의 초기 3D 모델 생성
5. 마음에 드는 모델 선택 후 HD 업스케일 또는 다운로드
6. GLB, FBX, OBJ 등 원하는 포맷으로 내보내기

### 추가 기능 (최신)

- **시드(Seed) 번호 & 네거티브 프롬프트** 지원
- **API 제공**: Luma API에서 `genie-3d` 모델로 텍스트 기반 3D 이미지 생성 (6개 직교 + 2개 자유 뷰)
- 최대 400자 프롬프트 입력

> [!WARNING]
> `https://lumalabs.ai/genie` 독립 페이지는 더 이상 제공되지 않으며, 기능은 **Luma 앱/웹 플랫폼 (Dream Machine)** 및 **API**로 통합되었습니다.

### 가격 정책 (2026년 기준)

| 플랜 | 가격 | 크레딧 | 특징 |
|------|------|--------|------|
| **Free** | $0 | 제한적 | 기본 생성, 표준 품질 |
| **Plus** | $30/월 | 10,000 | 상용 사용 가능, 고품질 |
| **Pro** | $90/월 | 40,000 | 4배 사용량 |
| **Ultra** | $300/월 | 150,000 | 15배 사용량 |

> **무료 사용 가능**: 예, 기본 생성 기능은 무료로 이용 가능합니다.

---

## 2. Luma AI Interactive Scenes (NeRF)

### 개요

Luma AI의 **Interactive Scenes**는 **Neural Radiance Fields (NeRF)** 및 **Gaussian Splatting** 기술을 활용하여 일반 스마트폰 영상이나 사진을 고품질 3D 장면으로 변환하는 AI 모델입니다.

### 주요 특징

| 항목 | 내용 |
|------|------|
| **기술 기반** | NeRF + Gaussian Splatting |
| **입력 방식** | 스마트폰 영상 또는 드론 영상 |
| **출력 포맷** | GLTF, OBJ, USDZ, PLY |
| **WebGL 지원** | 30FPS 브라우저 렌더링 |
| **파일 크기** | 오브젝트 8MB, 씬 20MB |
| **플랫폼** | iOS, Android, Web |
| **상용 라이선스** | 무료 (별도 라이선스 불필요) |

### 사용 방법

1. **앱 다운로드**
   - iOS: App Store에서 "Luma" 검색
   - Android: Google Play Store에서 "Luma" 검색
   - 또는 웹: https://lumalabs.ai 접속

2. **촬영**
   - 스마트폰으로 대상 오브젝트 또는 장면을 둘러보며 영상 촬영
   - 약 30초~1분 분량의 영상 권장
   - 반사되는 표면이나 투명한 오브젝트는 피하는 것이 좋음

3. **업로드 및 처리**
   - 앱 내에서 촬영한 영상 업로드
   - 클라우드에서 AI가 자동으로 3D 재구성 (수분 소요)
   - 웹 뷰어에서 즉시 인터랙티브 탐색 가능

4. **내보내기 및 활용**
   - GLTF, OBJ, USDZ 등으로 다운로드
   - Unity, Unreal Engine, Blender 등에서 활용
   - 웹사이트에 임베딩 가능 (WebGL)
   - AR/VR 호환 출력 지원

### 추가 업데이트 정보

- **Interactive Scenes V1.2**: 부동 소수점 아티팩트(floater) 감소, 실외 씬의 하늘/배경 품질 대폭 개선
- **Magic Reveal**: 씬을 열 때 생성되는 페이드인 효과를 앱에서 직접 비디오로 내보내기 가능
- **Gaussian Splatting 지원**: NeRF 외에 3D Gaussian Splatting 파이프라인 통합
- **WebGL 라이브러리**: 웹사이트에 임베딩 가능한 인터랙티브 3D 라이브러리 제공
- **Unbounded Captures**: 대규모 장면(건물, 거리 등) 캡처 지원

### 가격 정책 (2026년 기준)

| 플랜 | 가격 | 특징 |
|------|------|------|
| **Free** | $0 | 월 다수 캡처, 표준 품질, GLTF 내보내기 |
| **Pro** | $15/월 | 무제한 캡처, 고해상도 처리, 모든 내보내기 포맷, 상용 라이선스 |

> **무료 사용 가능**: 예, 기본 캡처 및 뷰어 기능은 무료입니다.

### 활용 분야

- **부동산**: 매물의 3D 인터랙티브 뷰 생성
- **여행 관광**: 명소의 몰입형 3D 투어 제작
- **게임 개발**: 실사 3D 에셋 프로토타이핑
- **제품 쇼케이스**: 제품의 360도 인터랙티브 뷰

---

## 3. Luma Scenes — 스토리보드 기반 AI 비디오 워크플로우 (신규)

### 개요

2026년 8월 출시된 **Luma Scenes**는 기존 Luma 생태계의 새로운 워크플로우로, AI 비디오 제작 시 전체 렌더링 비용이 낭비되는 문제를 해결합니다. 텍스트나 이미지에서 시작해 **스토리보드의 모든 키프레임을 먼저 검토하고 승인한 뒤에만 렌더링**하는 방식입니다.

### 주요 특징

| 항목 | 내용 |
|------|------|
| **기획 모델** | Uni-1 (브랜드/자산 일관성 유지) |
| **렌더링 모델** | Ray 3.2 또는 Seedance 2 |
| **비율 지원** | 9:16 (수직), 16:9 (수평) |
| **핵심 기능** | 씬별 개별 수정/재생성/타이밍 조정 |
| **대상** | 상업 광고, 소셜 비디오, 제품 영상 |

### 핵심 워크플로우

1. 한 줄 브리프 또는 브랜드 자산 입력
2. Uni-1이 완성된 시퀀스 스토리보드 생성 (컷 전환 없이 일관적 룩 유지)
3. 개별 키프레임 확인/의견 반영/교체 가능
4. 승인된 씬만 렌더링 → 한 씬이 어긋나도 전체가 아닌 해당 씬 1개만 수정
5. 무제한 반복 사용: 같은 승인 시퀀스를 재사용해 새로운 변형 제작

> **무료 사용 가능**: 유료 플랜(Plus $30/월~)에 포함됩니다.

---

## 4. Google Earth Studio

### 개요

**Google Earth Studio**는 Google Earth의 위성 및 3D 이미지를 활용하여 전문 수준의 지리 공간 애니메이션을 제작하는 **웹 기반 애니메이션 도구**입니다. 드론 촬영 없이도 항공 촬영 효과를 연출할 수 있습니다.

### 주요 특징

| 항목 | 내용 |
|------|------|
| **유형** | 웹 기반 애니메이션 도구 |
| **브라우저** | Google Chrome 전용 |
| **지원 OS** | Mac, Windows |
| **필수 기술** | WebGL, WebAssembly, 하드웨어 가속 |
| **데이터 소스** | Google Earth 위성/3D 이미지 |
| **출력** | JPEG 시퀀스, MP4 영상, 360° 스페리컬 영상 |
| **After Effects 연동** | 카메라 데이터 + 트래킹 포인트 내보내기 |

### 최신 업데이트 (Earth Studio 1.6~)

- **360° 스페리컬 내보내기**: VR 헤드셋(YouTube VR 등)용 파노라마 영상 렌더링 지원
- **로컬 렌더링**: Chrome 86+에서 하드디스크로 직접 렌더링 (메모리 절약, 장시간 시퀀스 지원)
- **클라우드 렌더링**: H.264/MPEG-4 동영상 렌더링 기능 (일일 18,000 프레임 한도 - 30fps 기준 10분)
- **KML 지원 개선**: Network Links, ScreenOverlays 등 확장 지원
- **Google Drive 통합**: KML/KMZ 파일을 Drive에서 직접 가져오기
- **텍스처 팝핑 완화**: 렌더 시 텍스처 깜빡임(popping) 블렌딩 기능
- **구름 저장**: 프로젝트 생성 시점의 구름 상태 저장으로 일관성 유지
- **3D 카메라 내보내기**: After Effects에서 2D/3D 요소 합성용 트래킹 데이터

### 시스템 요구사항

- **브라우저**: 최신 버전 Google Chrome
- **OS**: macOS 또는 Windows (최신 업데이트 권장)
- **WebGL**: 지원 필수 (확인: Chrome에서 WebGL 테스트 페이지 방문)
- **하드웨어 가속**: Chrome 설정 > 고급 설정 > 시스템 > "사용 가능한 경우 하드웨어 가속 사용" 활성화
- **인터넷**: 안정적인 고속 인터넷 연결 권장

### 사용 방법

1. **접속 및 승인**
   - https://earth.google.com/studio 접속
   - Google 계정으로 로그인
   - 액세스 요청 양식 제출 (뉴스, 연구, 교육, 비영리 목적으로 무료 승인)

2. **프로젝트 생성**
   - 빈 프로젝트(Blank Project) 또는 Quick Start 템플릿 선택
   - 프로젝트 이름, 해상도, 재생 시간, 프레임 레이트 설정

3. **Quick Start 템플릿 (5종)**
   - **Point-to-Point**: 최대 6개 지점 간 부드러운 카메라 이동
   - **Orbit**: 특정 대상 주변 원형 궤도 애니메이션
   - **Spiral**: 점점 작아지는 나선형 궤도
   - **Fly-To and Orbit**: 원거리에서 접근 후 궤도 전환
   - **Zoom-To**: 고도에서 지점으로 간단한 줌

4. **애니메이션 편집**
   - 키프레임 추가/편집으로 카메라 경로 조정
   - 커브 에디터로 이징(Easing) 효과 적용
   - 시간대 변경으로 일출/일몰 효과 연출
   - 필드 오브뷰 조정으로 줌 인/아웃 효과

5. **렌더링 및 내보내기**
   - 온라인 렌더링 (해상도에 따라 시간 소요)
   - JPEG 시퀀스 또는 MP4로 내보내기
   - After Effects용 카메라 데이터 내보내기 가능

### 가격 정책

> **무료**: 뉴스, 연구, 교육, 비영리 목적으로 **완전 무료** 사용 가능

- 상용 사용 시 Google Maps/Google Earth 추가 약관 준수 필요
- 콘텐츠에 "Google Earth" 및 제3자 이미지 제공자 표시 필요

### 활용 분야

- **콘텐츠 크리에이터**: 드론 없이 항공 촬영 효과 영상 제작
- **뉴스 미디어**: 지리적 사건 시각화
- **교육**: 지구과학, 지리학 교육 자료 제작
- **부동산/관광**: 지역 소개 영상, 매물 주변 환경 시각화
- **영화/방송**: 지리적 위치 시퀀스 제작

---

## 무료 사용 가능 여부 비교 요약

| 도구 | 무료 플랜 | 상용 플랜 시작가 | 비고 |
|------|-----------|-----------------|------|
| **Luma Genie** | 예 (기본 생성) | $30/월 | 기본 3D 생성은 무료 |
| **Luma Interactive Scenes** | 예 (캡처 + 뷰어) | $15/월 | 캡처, 뷰어, 기본 내보내기 무료 |
| **Luma Scenes (신규)** | 아니요 | $30/월 | 유료 플랜에 포함 |
| **Google Earth Studio** | 예 (전체 기능) | 무료 | 교육/연구/뉴스/비영리 무료, 상용은 별도 문의 |

---

## 추천 사용 시나리오

### 게임 개발자
1. **Luma Genie**로 프로토타입 3D 에셋 신속 생성
2. **Luma Interactive Scenes**로 실사 환경 스캔 후 게임에 통합
3. **Google Earth Studio**로 게임 배경 레퍼런스 영상 제작

### 애니메이션 작가
1. **Luma Interactive Scenes**로 실사 캐릭터/배경 3D 캡처
2. **Google Earth Studio**로 애니메이션 배경 지리 시퀀스 제작
3. 생성된 3D 모델을 Blender/Unreal Engine에서 애니메이션 적용

### 콘텐츠 크리에이터
1. **Google Earth Studio**로 여행/지리 콘텐츠 항공 영상 제작
2. **Luma Genie**로 영상에 들어갈 3D 그래픽 요소 생성
3. **Luma Interactive Scenes**로 인터랙티브 3D 콘텐츠 제작

### 그래픽 아트 창작자
1. **Luma Genie**로 텍스트 기반 3D 아트 프로토타이핑
2. **Luma Interactive Scenes**로 실물 스캔 후 디지털 아트 통합
3. 웹사이트에 임베딩 가능한 인터랙티브 3D 갤러리 제작

---

## 참고 링크

| 도구 | URL |
|------|-----|
| Luma 앱/웹 (Genie 포함) | https://app.lumalabs.ai |
| Luma Interactive Scenes | https://lumalabs.ai/interactive-scenes |
| Luma Scenes (신규) | https://lumalabs.ai/news/introducing-luma-scenes |
| Luma API 문서 | https://docs.lumalabs.ai |
| Luma 앱 (iOS) | App Store 검색 "Luma Dream Machine" |
| Luma 앱 (Android) | Google Play Store 검색 "Luma" |
| Google Earth Studio | https://earth.google.com/studio |
| Earth Studio 문서 | https://earth.google.com/studio/docs |
| Earth Studio 튜토리얼 | https://earth.google.com/studio/docs/tutorials |
| Google Earth 업데이트 내역 | https://developers.google.com/maps/documentation/earth/release-notes |

---

*생성일: 2026년 9월 11일*
