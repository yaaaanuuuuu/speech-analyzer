# 🗣️ 한국어 발화 분석기 (Kiwi v09)

언어치료·언어학 연구를 위한 한국어 구어 발화 분석 웹앱입니다.

## 산출 지표
| 지표 | 설명 |
|------|------|
| Token / Type | 전체·고유 형태소 수 |
| MLU / MLU-w | 평균발화길이 (형태소 / 어절) |
| TTR_전체 / TTR_내용어 | 어휘 다양도 |
| NDW / NDW-50 | 다른 단어 수 |
| 내용어수 / 기능어수 | 품사 분류별 집계 |

---

## 로컬 실행

```bash
pip install -r requirements.txt
streamlit run app.py
```

브라우저에서 `http://localhost:8501` 접속

---

## Streamlit Community Cloud 무료 배포

1. 이 폴더를 **GitHub 저장소**에 push
   ```
   git init
   git add .
   git commit -m "init"
   git remote add origin https://github.com/사용자명/저장소명.git
   git push -u origin main
   ```

2. [share.streamlit.io](https://share.streamlit.io) 접속 → Google/GitHub 로그인

3. **New app** → 저장소·브랜치·`app.py` 선택 → **Deploy**

4. 배포 완료 후 URL 공유  
   예: `https://사용자명-저장소명-app-xxxx.streamlit.app`

---

## 파일 구조

```
speech_analyzer/
├── app.py            ← Streamlit 메인
├── requirements.txt  ← 패키지 목록
└── README.md
```
