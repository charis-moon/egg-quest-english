# Egg Quest 🐣

4–7세를 위한 독립 영어 학습 플랫폼 게임. Reading Eggs나 Nintendo의 공식 제품이 아니며, 해당 서비스의 코드·캐릭터를 사용하지 않습니다.

## 실행

`python3 -m http.server 8080 --directory dist` 후 http://localhost:8080 방문. 설치·빌드 없이 실행됩니다.

## 조작 및 학습

방향키 / 화면 버튼으로 이동, 스페이스 / ↑ 버튼으로 점프. 들려주는 단어의 그림에 닿으면 수집합니다. 과일·동물·색깔 3개 월드, 9개 기초 단어를 지원합니다. 오답 감점이나 게임 오버가 없고 다시 듣기, 일시정지, 월드 선택을 제공합니다.

영어 발음은 Web Speech API이며 지원 여부와 발음은 브라우저에 따라 달라집니다. 기기 내 localStorage에 완료한 월드만 저장합니다. 서버나 개인정보 수집 기능은 없습니다. Google Fonts를 사용하며 오프라인에서는 시스템 글꼴로 대체됩니다.

## 배포

운영 주소: https://egg-quest-taupe.vercel.app

GitHub `main` 브랜치에 푸시하면 연결된 Vercel 프로젝트 `egg-quest`가 자동으로 운영 배포합니다. Vercel 설정은 `vercel.json`에 있으며 출력 디렉터리는 `dist`입니다.

`dist/`를 정적 호스팅에 배포합니다. GitHub Pages는 저장소 Settings → Pages → GitHub Actions에서 활성화하면 포함된 워크플로로 배포할 수 있습니다. Sites 배포 설정은 `.openai/hosting.json`에 있습니다.
