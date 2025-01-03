## 실습 환경 세팅
    1. Repository 환경설정
        1. 팀 리드가 실습용 리파지토리 생성
        2. Github Repository 페이지 → Setting (우측 상단)
        3. Manage Access (or Collaborators)
        4. invite a collaborator 버튼 클릭
        5. 팀원의 Github 이메일 입력 → 초대
        6. 팀원 각자 수락 →  collaborator 권한 부여
        7. gitignore 파일 한 번 세팅해 보기
        8. README.md 파일 세팅해 보기
    2. Branch Protection 설정으로 PR 강제하기 
        1.  dev 브랜치 생성하여 dev에 즉각 커밋이 불가능하도록 설정
        2. Setting → Branches → Add branch protection rule 클릭
        3. Branch name pattern = dev, main
            1. 실제 브랜치 이름과 맞게 설정해야 함. main 혹은 master
        4. Rule 옵션
            1. Protect matching branches → 활성화
            2. Require pull request reviews before merging → 체크
            3. Require approvals → 전체 팀원 -1 명 이상 review 필요
            4. save
        5. 각자 작업해 보기
            1. 각자 컨셉을 정해 feature를 하나씩 만들어 보세요
                1. 금융 앱, 음식 배달앱 등등
                2. 컨셉을 정했다면 어떤 기능이 필요할지 생각해 보세요
                    1. 생각한 기능에 이름을 붙여 보세요
                    2. 학습한 규칙에 맞게 각자 브랜치를 생성하세요
                3. git clone 진행한 뒤, 자신의 브랜치에서 작업하세요
                    1. 본인이 맡은 기능의 로직을 고민해 보세요
                        1. 예) 로그인이라고 하면, 사용자 정보를 데이터베이스에서 가져오고, 데이터베이스에 저장된 비밀번호와 사용자가 입력한 비밀번호를 대조할 수 있겠죠.
                            1. 이 때 비밀번호 암호화는…?
                    2. 자유 포맷/확장자로 파일에 작성하세요.
                    3. 완성되었다면 다음으로…
        6. PR
            1. 각자 작업 후 PR 요청
            2. PR 페이지 접근 → 코드 리뷰
            3. File changed 탭 확인 → Review changes 클릭
        7. (optional) 충돌 해결 실습
            1. 여러분들은 이제 어떻게 작업해야 충돌이 생기는지 학습했습니다.
            2. 고의로 동료의 브랜치에 conflict를 발생시켜 보세요.
