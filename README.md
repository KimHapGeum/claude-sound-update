# claude-sound 설치와 업데이트

claude-sound는 마이크로 Claude Code를 조작하는 Windows 앱이에요. 말하면 Claude 창에 입력되고, 답은 소리로 읽어 줘요. 작업 표시줄 위에는 캐릭터가 살면서 Claude가 하는 일에 맞춰 움직여요.

이 저장소에는 설치 파일과 업데이트 정보만 있어요. 앱의 코드 저장소는 비공개예요.

## 설치

1. [최신 릴리스](https://github.com/KimHapGeum/claude-sound-update/releases/latest)에서 `claude-sound-setup.zip`을 받아 압축을 풀어요.
2. 폴더 안의 `설치하기.bat`을 두 번 눌러요.
3. 바탕화면의 `claude-sound` 바로 가기로 켜요.

처음 설치할 때는 라이브러리 2~3GB를, 처음 켤 때는 음성 인식 모델 약 3GB를 받아요.

### 필요한 것

- Windows
- [Claude Code](https://claude.com/claude-code)
- 마이크
- NVIDIA GPU 권장 (없으면 CPU로 받아써서 느려요. 그럴 때는 설정에서 `small` 모델을 고르세요)

## 사용법

F9를 누르고 말한 뒤 떼면 돼요. 자세한 사용법은 설정 창의 "사용 방법" 탭에 있어요. 설정 창은 작업 표시줄 오른쪽의 트레이 아이콘에서 열어요.

## 업데이트

앱을 켤 때 새 버전을 찾아 설치할지 물어보고, 네를 누르면 받아서 깔고 다시 켜져요. 설정 창의 업데이트 확인 버튼으로도 찾을 수 있어요.

새 버전을 직접 받아 `설치하기.bat`을 다시 실행해도 돼요. 설정과 시청자 기록은 그대로예요.

## 이 저장소의 파일

| 파일 | 하는 일 |
|---|---|
| `version.json` | 앱이 새 버전을 확인할 때 읽는 정보 (버전, 받을 주소, 바뀐 내용, 파일 지문) |
| [Releases](https://github.com/KimHapGeum/claude-sound-update/releases) | 버전별 설치 파일과 바뀐 내용 |

앱은 받은 파일의 지문이 `version.json`의 `sha256`과 같을 때만 설치해요.
