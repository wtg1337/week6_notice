# 6주차 과제: 비동기 공지사항 앱 (`week6_notice`)

본 프로젝트는 Flutter의 비동기 처리(`Future`, `Stream`, `async/await`), `mounted` 검사를 통한 안전한 화면 상태 관리, 그리고 프롬프트 엔지니어링 실습 결과를 담고 있는 과제 제출용 저장소입니다.

---

## 📌 주요 구현 및 학습 내용

* **비동기 공지 처리**: `Future` 및 `async/await`를 활용한 데이터 로딩 및 상태 변화 구현
* **예외 처리 및 상태 안전성**: `await` 실행 후 `mounted` 여부를 확인하여 위젯 수명주기 에러 방지
* **UI 상태 대응**: `idle`, `loading`, `success`, `failure` Enum 상태에 따른 직관적인 UI 제공
* **테스트 및 검증**: `flutter test` 기반 AC(Acceptance Criteria) 통과 검증

---

## 📁 파일 및 폴더 구조

* **`lib/main.dart`**: 과제 주요 로직 및 비동기 화면 구성 코드
* **`PROMPT_COMPARISON.md`**: 프롬프트 A/B 요청 비교, 모델 실행 결과, 선택 이유, `await` 전후 상태 변화 설명
* **`evidence/`**: `flutter test` 결과 및 실행 로그 증거 자료
* **`test/widget_test.dart`**: 과제 요구사항 검증을 위한 위젯 테스트 코드

---

## 🛠️ 실행 및 테스트 방법

```bash
# 1. 패키지 수급
flutter pub get

# 2. 앱 실행
flutter run

# 3. 과제 검증 테스트 실행
flutter test