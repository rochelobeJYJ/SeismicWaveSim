# Web Seismic Wave Simulator (웹 지진파 시뮬레이터)

[![License](https://img.shields.io/badge/License-GPL_3.0-blue.svg)](LICENSE)
[![Play Online](https://img.shields.io/badge/Play-Online-success.svg)](https://rochelobeJYJ.github.io/SeismicWaveSim/)

**👉 [웹에서 바로 실행하기 (Play Online)](https://rochelobeJYJ.github.io/SeismicWaveSim/)**

웹 기반 지진파 시뮬레이터로, 지진파(P파 및 S파)의 전파 과정과 주시곡선 생성 과정을 실시간으로 시각화합니다. 이 프로젝트는 [FFLiK/SeismicWaveSimulator](https://github.com/FFLiK/SeismicWaveSimulator)의 원본 C++ 물리 엔진을 단일 HTML5/JavaScript 파일로 이식(Porting)한 버전으로, 직관적인 UI와 확장된 교육용 기능을 제공합니다.
<img width="1918" height="856" alt="image" src="https://github.com/user-attachments/assets/0921c66a-66dc-4223-95a8-3a0d859baac1" />


## 🌟 주요 기능 (Key Features)

* **지진파 추적 (Ray Tracing):** P파와 S파의 직접파, 반사파, 그리고 임계굴절파(선두파)의 전파 과정을 동시에 시뮬레이션합니다.
* **지층 구조 편집:** 슬라이더 형태의 UI를 통해 다층 구조의 지구 내부 모델(두께, 밀도, Vp, Vs)을 실시간으로 설계하고 조작할 수 있습니다.
* **주시곡선 (Travel-Time Curves):** 이론적 곡선과 관측된 데이터 포인트를 동시에 매칭하여 보여주는 주시곡선 그래프를 실시간으로 렌더링합니다.
* **데이터 엑셀 추출:** 지표면 수신기들에 도달한 지진파의 도달 시간 및 전체 시뮬레이션 변수를 `.xlsx` 엑셀 파일로 손쉽게 다운로드하여 과학적 분석에 활용할 수 있습니다.
* **화면 확대 및 반응형 디자인:** 어두운 테마(Dark Theme)와 글래스모피즘(Glassmorphism) 기반의 수려한 UI를 갖추고 있으며, 단면도와 그래프를 전체 화면으로 확대하여 세밀하게 관찰할 수 있습니다.
* **단일 파일 호환성:** 외부 서버나 복잡한 빌드 과정 없이, 오직 하나의 단일 HTML 파일로 모든 기능이 작동합니다.

## 🚀 실행 방법

1. **[웹 브라우저에서 바로 실행하기 (클릭)](https://rochelobeJYJ.github.io/SeismicWaveSim/)**: 별도의 다운로드나 설치 없이 위 링크를 클릭하여 모바일/PC 환경에서 즉시 시뮬레이터를 사용할 수 있습니다.
2. **로컬 오프라인 실행하기**: 저장소의 `index.html` 파일을 다운로드 받아 웹 브라우저(크롬, 엣지, 사파리 등)에 드래그 앤 드롭하여 오프라인 환경에서도 실행할 수 있습니다.

## 🔧 사용 가이드

* **프리셋 (Presets):** "기본 세팅", "다층 구조", "저속도층", "숨은층(Blind Zone)" 등 교육용으로 구성된 사전 설정 시나리오를 클릭 한 번으로 불러올 수 있습니다.
* **시뮬레이션 조작:** 단면 시뮬레이션 캔버스의 임의의 위치를 클릭하면 해당 위치로 즉시 진원(지진 발생 위치)이 이동하며 재실행됩니다. 사이드 제어판에서 입자 수, 시뮬레이션 속도, 파동 표시 여부를 자유롭게 설정할 수 있습니다.
* **지층 에디터:** 슬라이더를 움직여 각 지층의 밀도와 지진파 속도를 조절하세요. 밀도를 `0`으로 설정하면 '공기층(Air Layer)'으로 자동 인식됩니다. 가장 아래쪽 지층에 `무한대(INF)`를 체크하면 깊이가 무한한 기반암으로 설정됩니다.
* **데이터 내보내기:** 우측 하단의 수신기 테이블 상단에 있는 `📊 엑셀 다운로드` 버튼을 클릭하면 전체 시뮬레이션 환경 변수 및 지진파 도달 기록을 즉시 엑셀로 저장할 수 있습니다.

## 📚 출처 및 참고 (Acknowledgements)

이 프로젝트는 [FFLiK/SeismicWaveSimulator](https://github.com/FFLiK/SeismicWaveSimulator)의 C++ 물리 엔진을 웹 브라우저 환경으로 포팅한 것입니다. 스넬의 법칙(Snell's Law) 근사화 및 반사 계수를 포함한 핵심 광선 추적(Ray-tracing) 알고리즘은 원본의 물리 법칙을 따르며, UI/UX와 교육용 시각화 기능은 자바스크립트를 통해 새롭게 설계되었습니다.

## 📜 라이선스 (License)

이 프로젝트는 GPL-3.0 라이선스 규정을 따릅니다.
