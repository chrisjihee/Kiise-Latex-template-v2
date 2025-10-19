# 한국정보과학회 학술대회 논문작성 양식 (LaTeX)

한국정보과학회(KIISE) 학술대회 논문 작성을 위한 LaTeX 템플릿입니다.

## 소개

이 템플릿은 한국정보과학회(Korea Information Science Society, KIISE) 학술대회에 제출할 논문을 LaTeX으로 작성할 수 있도록 구조화된 양식입니다.

## 파일 구조

```
.
├── paper.tex              # 메인 LaTeX 파일
├── kcc.cls                # 한국정보과학회 문서 클래스
├── packages.tex           # 사용할 LaTeX 패키지 목록
├── definitions.tex        # 사용자 정의 명령어 및 정의
├── references.bib         # 참고문헌 BibTeX 파일
├── 00abstract.tex         # 초록
├── 01introduction.tex     # 서론
├── 02related.tex          # 관련 연구
├── 03preliminaries.tex    # 배경 지식
├── 04proposed.tex         # 제안 방법
├── 05experiments.tex      # 실험
├── 06conclusion.tex       # 결론
├── 07appendix.tex         # 부록
└── figures/               # 그림 파일 디렉토리
    └── features.pdf
```

## 사용 방법

### 1. 기본 정보 설정

`paper.tex` 파일을 열어 다음 정보를 수정하세요:

```latex
\title{국문 제목}
\author{
저자1 국문이름$^{\circ}$, 저자2 국문이름\\
저자 소속 국문명 \\
\{author1email, author2email\}@domain.kr
}
\engtitle{English Title}
\engauthor{
First Author Name, Second Author Name\\
Author Affiliation\\
}
```

### 2. 논문 작성

각 섹션별로 분리된 `.tex` 파일을 편집하세요:

- `00abstract.tex`: 논문 초록 작성
- `01introduction.tex`: 서론 작성
- `02related.tex`: 관련 연구 작성
- `03preliminaries.tex`: 배경 지식 작성
- `04proposed.tex`: 제안 방법 작성
- `05experiments.tex`: 실험 및 결과 작성
- `06conclusion.tex`: 결론 작성
- `07appendix.tex`: 부록 작성 (필요한 경우)

### 3. 참고문헌 추가

`references.bib` 파일에 BibTeX 형식으로 참고문헌을 추가하세요.

### 4. 그림 추가

`figures/` 디렉토리에 그림 파일을 저장하고, 논문에서 참조하세요.

## 컴파일 방법

### 명령줄에서 컴파일

```bash
# LaTeX 컴파일
pdflatex paper.tex

# BibTeX으로 참고문헌 처리
bibtex paper

# LaTeX 재컴파일 (참고문헌 반영)
pdflatex paper.tex
pdflatex paper.tex
```

### Overleaf에서 사용

1. [Overleaf](https://www.overleaf.com/)에 로그인
2. 새 프로젝트 생성 후 모든 파일 업로드
3. 메인 문서를 `paper.tex`로 설정
4. 자동으로 컴파일됩니다

## 문서 모드

`paper.tex`의 첫 줄에서 문서 모드를 선택할 수 있습니다:

```latex
\documentclass[preprint]{kcc}  % 리뷰용 (줄 번호 표시)
%\documentclass{kcc}            % 출판용 (최종 제출)
```

- **리뷰용 (preprint)**: 논문 검토를 위해 줄 번호가 표시됩니다
- **출판용**: 최종 제출 시 사용하는 깔끔한 버전입니다

## 필요한 LaTeX 패키지

이 템플릿은 다음과 같은 주요 패키지를 사용합니다:

- `graphicx`, `subfigure`: 그림 삽입
- `amsmath`, `amssymb`, `amsthm`: 수식 작성
- `algorithm`, `algorithmic`: 알고리즘 표현
- `booktabs`, `multirow`: 표 작성
- `appendix`: 부록 추가

전체 패키지 목록은 `packages.tex` 파일을 참조하세요.

## 참고 자료

이 템플릿은 다음 자료를 참고하여 편집되었습니다:

- [한국정보과학회 공식 양식](http://m.kiise.or.kr/conference/board/referenceview.do?CC=kcc&CS=2016&PARENT%5FID=530300&&no=15)
- [서울대학교 IDS Lab LaTeX Template](http://ids.snu.ac.kr/wiki/LaTeX%5Ftemplate%5Ffor%5FKCC)
- [leejaymin/Kiise-Latex-template](https://github.com/leejaymin/Kiise-Latex-template)
- [Overleaf 템플릿](https://www.overleaf.com/latex/templates/hangugjeongbogwahaghoe-hagsuldaehoe-nonmunjagseong-yangsig/nhgcmdbskkrv)

## 기여자

- **원저자**: Jinhong Jung (Soongsil University, DMLAB)

## 라이선스

이 템플릿은 [Creative Commons Attribution 4.0 International License (CC BY 4.0)](LICENSE) 하에 배포됩니다.

## 문의사항

논문 작성 중 문제가 발생하거나 궁금한 점이 있으시면 한국정보과학회 학술대회 담당자에게 문의하시기 바랍니다.

---

**Happy Writing! 📝**

