# filteringdev-noti
이 문서는 [webhook-noti](https://github.com/FilteringDev/webhook-noti)를 기반으로 동작하는 filteringdev-noti bot 봇에 대한 설명입니다.

## Repo
봇은 GitHub App이 설치된 저장소를 대상으로 합니다. 설치된 저장소 목록은 10분마다 갱신하고, 릴리스는 60초마다 확인합니다. 최초 기준 상태를 기록한 뒤 새로 게시된 초안이 아닌 각 릴리스에 대해 내부 검증 후 알림을 전송합니다. 모니터링을 시작할 때 기존에 게시된 릴리스는 전송하지 않습니다.

## 설치 방법
설치하시라면 아래 방법으로 진행하시면 됩니다.

- Discord: https://discord.com/oauth2/authorize?client_id=1543001264776814723 를 오픈하시고 진행
- Telegram: `@filteringdev_noti_bot`

## 법적 문서
- [이용약관](TERMS_OF_SERVICE-ko.md)
- [개인정보 처리방침](PRIVACY_POLICY-ko.md)

영문 문서는 [README.md](README.md)를 참조하세요.