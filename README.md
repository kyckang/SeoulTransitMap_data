# 서울 교통맵 공개 데이터

"서울 교통맵" 앱이 받아 쓰는 정류소·노선·지하철역 데이터입니다. 앱 저장소의 GitHub Actions가 매일 새로 만들어, 바뀐 것이 있을 때만 올립니다. **이 저장소의 파일은 직접 고치지 마세요.** 다음 갱신 때 덮어씌워집니다.

| 파일 | 내용 |
|---|---|
| `v1/seoul_bus_stops.csv` | 버스 정류소 (서울 + 서울 노선이 지나는 경기·인천) — 정류소 ID, ARS 번호, 이름, 좌표, 방면 |
| `v1/seoul_bus_routes.csv` | 서울 면허 버스 노선 — 번호, 유형, 기점·종점, 첫차·막차, 배차 |
| `v1/seoul_subway_stations.csv` | 수도권 지하철역 — 노선, 역 번호, 역명(한·영·중·일), 좌표 |
| `v1/data_manifest.json` | 생성 시각, 건수, 파일별 sha256(앞 16자리), 형식 버전 |

`v1` 은 형식 버전입니다. 열 구성이 바뀌면 `v2` 폴더를 새로 만들어, 옛 앱은 계속 `v1` 을 받게 합니다.

## 출처

- 서울특별시 교통정보시스템(TOPIS), 서울열린데이터광장 — 공공누리 제1유형
- 공공데이터포털(data.go.kr) 서울특별시 버스 정보 API
- 서울교통공사 등 운영기관 역 정보 (서울열린데이터광장 제공)

This repository holds public transit data (bus stops, routes, subway stations in Seoul) generated automatically from Seoul Metropolitan Government open data (KOGL Type 1) for the Seoul Transit Map app.
