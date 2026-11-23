# 홈페이지 수정 및 배포 안내

배포 주소: https://dhwi96.github.io/

## 자주 수정할 파일

| 변경 내용                                 | 파일                       |
| ----------------------------------------- | -------------------------- |
| 자기소개, 학력, 연구 관심사               | `_pages/about.md`          |
| 국제 논문, 저자, 연도, 코드·프로젝트 링크 | `_bibliography/papers.bib` |
| 국내 논문                                 | `_pages/publications.md`   |
| 연구과제, 경력, 수상                      | `_pages/cv.md`             |
| 강의 경험                                 | `_pages/teaching.md`       |
| 이메일, Scholar, GitHub, LinkedIn         | `_data/socials.yml`        |
| 사이트 이름, 설명, 주소                   | `_config.yml`              |
| 프로필 및 연구·수상 사진                  | `assets/img/research/`     |

GitHub에서 파일을 열고 연필(Edit) → 수정 → Commit changes를 하면 자동 배포됩니다.
Actions의 Deploy site가 성공한 뒤 사이트에 반영됩니다.
논문을 홈페이지에도 표시하려면 BibTeX 항목에 `selected = {true}`를 추가합니다.
썸네일은 `preview = {research/파일명.png}`로 지정합니다.

## 주소와 배포 설정

- 저장소 이름은 계정명과 같은 `dhwi96.github.io`여야 루트 주소를 사용할 수 있습니다.
- `_config.yml`: `url: https://dhwi96.github.io`, `baseurl: ""` 유지.
- 저장소 Settings → Pages의 Source는 GitHub Actions로 설정합니다.
- `.github/workflows/deploy.yml`에서 Jekyll을 빌드하고 공식 Pages Actions로 배포합니다.
- 템플릿 예시 페이지와 컬렉션은 `_config.yml`의 `exclude`로 배포에서 제외했습니다.
- 원본 Google Sites는 별도 서비스이므로 자동 리디렉션되지 않습니다. 이전 안내와 새 주소를 원본 홈 상단에 넣으면 됩니다.
- Google Sites의 공개 내용과 이미지 8장을 이전했습니다. 논문 원제와 저자·연도는 원본을 기준으로 보존했습니다.
