# 보글 (Bogle)

그림을 캐릭터 친구로 만드는 iPad 가로 화면용 Flutter 데모입니다. 스케치북에 그림을 그리거나 사진을 선택해 친구를 만들고, 이름·성격·말투를 정한 뒤 보관함과 친구의 집에서 다시 만날 수 있습니다.

## 실행

Flutter 3.41.5와 Dart 3.11.3, iPadOS 15 이상을 기준으로 합니다. iOS 실기기는 Xcode에서 개발 팀과 서명을 설정해 주세요.

```sh
flutter pub get
flutter devices
flutter run -d <DEVICE_ID>
```

친구 생성, 대화, 보관함과 캐릭터 모션은 기기에서 동작합니다. 그림이나 사진은 캐릭터의 이미지로 사용되고, 대화에는 기기 내 시연용 응답이 나옵니다. 인형 주문과 결제 화면은 시연용입니다. 주소 검색을 열면 카카오 우편번호 서비스에 연결됩니다.

## 코드와 검증

- `lib/src/drawing/`에 스케치북 도구가 있습니다.
- `lib/src/screens/`에 그림·사진 입력, 캐릭터 설정과 보관함 화면이 있습니다.
- `lib/src/data/`에 기기 저장소와 서비스 인터페이스가 있습니다.
- [캐릭터 리그 규약](docs/CHARACTER_RIG.md)에 이미지와 SVG 캐릭터의 모션 구조를 정리했습니다.

```sh
flutter analyze
flutter test
```

이 공개본은 프론트엔드 데모입니다. 서버 연동이 필요한 운영 기능은 별도 프로젝트에서 관리합니다. 기본 캐릭터·로고·예시 스케치에는 데모 그래픽을 사용합니다.

## 기여 및 에셋

[jjukummee](https://github.com/jjukummee)가 공개본을 관리합니다.

- [Pretendard · SIL Open Font License](assets/fonts/Pretendard-OFL.txt)
- [양진체 · SIL Open Font License](assets/fonts/Yangjin-OFL.txt)
- [Lucide 사진 편집 아이콘 · ISC License](assets/icons/photo/LICENSE)
