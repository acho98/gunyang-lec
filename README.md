# 초급 데이터 분석 과정 (5교시 · 5시간)

---

## 🗂 커리큘럼 (5교시)

| 교시 | 슬라이드(이론, `slides/*.pdf`) | 실습(`labs/*.ipynb`) | 핵심 |
|---|---|---|---|
| **1교시** | `1교시_데이터분석개론` + `1교시_사례편` | `01_demo` (강사 시연) | 왜 분석하나 · 기초 통계(평균의 함정) · 데이터 보는 법 · AI 시대 · 실전 사례 |
| **2교시** | `2교시_데이터와친해지기` | `02_lab` — 타이타닉 생존 분석 | 첫인상(EDA) · 결측 점검 · 그룹별 비교(groupby) |
| **3교시** | `3교시_지저분한데이터` | `03_lab` — 부동산·금융 | 타입 변환 · 결측치 처리 5가지 방법 |
| **4교시** | `4교시_그림으로말하기` | `04_lab` — 펭귄·세계행복·팁 | 5대 차트 · 차트 선택 · 결과 해석 |
| **5교시** | `5교시_분석가의길` | `05_capstone` (월드컵) **또는** `05_project_spotify` (음악) 중 **택1** | 분석 전 과정 · 분석가의 진짜 일 · AI 시대 · 의료 데이터 · 셀프스터디 로드맵 |

> 슬라이드는 **PDF**로 제공됩니다(`slides/`). 실습은 **Jupyter 노트북**으로 제공됩니다(`labs/`).
>
> **5교시 프로젝트는 둘 중 하나만** 수업에서 진행합니다(시간상). 두 프로젝트 모두 독립 완결형이라, **나머지 하나는 셀프스터디용**으로 집에서 그대로 완주할 수 있습니다.

---

## 💻 환경 — 구글 코랩이면 설치 없이 바로

처음이라면 **구글 코랩(Google Colab)** 을 추천합니다. 브라우저만 있으면 됩니다.

- **코랩**: <https://colab.research.google.com> → 새 노트 → `labs/`의 `.ipynb` 업로드 → 위에서부터 실행.
- **내 컴퓨터(아나콘다)**: [Anaconda](https://www.anaconda.com/download) 설치 → Jupyter 실행.

> **🚀 데이터·폰트가 자동으로 따라옵니다 (업로드 불필요)**
> 노트북은 로컬에 `data/`가 있으면 그걸 쓰고, **없으면(코랩 등) 공개 저장소에서 인터넷으로 바로 내려받습니다.** 그래서 코랩에선 `.ipynb`만 열어 실행하면 끝 — 파일 업로드도, 드라이브 마운트도 필요 없습니다.
> - 데이터 저장소: **<https://github.com/acho98/gunyang-data>** (노트북이 `data_path()` 헬퍼로 raw URL 자동 로드)
> - seaborn 내장 데이터(`titanic`·`tips`·`penguins`)도 업로드 없이 바로 로드
> - 한글 폰트도 자동: 로컬에 없으면 저장소에서 내려받아 적용(실패해도 영문 차트는 정상)

---

## 📊 사용 데이터셋 & 출처

**검증된 고전 (seaborn 내장 — 다운로드 불필요)**: `titanic` · `tips` · `penguins`

**실제·공개 데이터 (저장소 [gunyang-data](https://github.com/acho98/gunyang-data)에서 자동 로드)**

| 파일 | 내용 | 출처 |
|---|---|---|
| `world_happiness_owid.csv` | 세계 행복 점수 2011–2025, 158개국 | Our World in Data (무인증 공개) |
| `apt_realprice_202105.csv` | 국토부 아파트 실거래가 (2021-05) | 국토교통부 실거래가 공개시스템 |
| `worldcup_results.csv` | 국제 축구 A매치 1872–2026 (49,477경기) | martj42/international_results (스냅샷) |
| `spotify_tracks.csv` | Spotify 트랙 114,000곡 × 오디오 피처 | maharshipandya/spotify-tracks-dataset (BSD) |
| `btc_usd_daily.csv` · `gold_5y.csv` | 비트코인·금 시세 | CryptoDataDownload · 강사 수집본 |
| `BMDOHYEON.ttf` | 한글 폰트 (차트 한글 깨짐 방지) | 배민 도현체 (상업적 이용 무료) |

> 자세한 출처·라이선스는 gunyang-data의 `DATA_SOURCES.md` 참고.
