# AWSKRUG 홈페이지
본 페이지는 AWSKRUG의 Single Page Application으로 awskr.org의 첫화면입니다. 필요한 정보가 있으시면 업데이트 하시기 바랍니다.
- 홈페이지: https://www.awskr.org
- 관리자: contact@awskr.org
- 배포 상태: ![Deploy Website](https://github.com/awskrug/awskrug.github.io/actions/workflows/deploy.yml/badge.svg)

## 자동 배포 (Automatic Deployment)
이 저장소는 GitHub Actions를 통해 자동 배포가 설정되어 있습니다. `main` 또는 `master` 브랜치에 변경사항이 푸시되면 자동으로 웹사이트가 빌드되고 GitHub Pages를 통해 배포됩니다.

### 배포 과정
1. 코드 변경사항을 커밋합니다.
2. `main` 또는 `master` 브랜치에 푸시합니다.
3. GitHub Actions가 자동으로 실행되어 웹사이트를 `gh-pages` 브랜치에 배포합니다.
4. 배포 상태는 저장소의 Actions 탭에서 확인할 수 있습니다.

### 수동 배포
필요한 경우 GitHub 저장소의 Actions 탭에서 "Deploy Website" 워크플로우를 수동으로 실행할 수 있습니다.

## 웹 사이트 자동 배포 기능 (GitHub Actions)
소스 코드가 커밋되면 자동으로 배포하는 GitHub Actions 워크플로우가 `.github/workflows/deploy.yml` 파일에 구성되어 있습니다. 이 워크플로우는 다음과 같은 기능을 제공합니다:

- `main` 또는 `master` 브랜치에 푸시될 때 자동 배포
- 수동 트리거 옵션 (`workflow_dispatch`)
- 동시 실행 방지 및 진행 중인 작업 취소 기능
- 배포 상태 알림

자세한 내용은 [배포 가이드](.github/DEPLOYMENT.md)를 참조하세요.
