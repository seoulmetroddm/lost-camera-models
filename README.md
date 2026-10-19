# lost-camera-models

유실물 촬영 웹앱 모델 파일 보관 (Releases)

모델 파일은 이 저장소에 커밋하지 않고 **Releases 첨부 파일**로 둔다. 앱 저장소의 빌드 스크립트가 아래 주소에서 받아 SHA-256을 확인한 뒤 배포에 넣는다.

## 모델 목록

| 태그 | 파일 | 크기 | SHA-256 | 출처 | 라이선스 |
|---|---|---|---|---|---|
| `u2netp-v1` | `u2netp.onnx` | 4,574,861 B | `309c8469258dda742793dce0ebea8e6dd393174f89934733ecc8b14c76f4ddd8` | [danielgatis/rembg v0.0.0](https://github.com/danielgatis/rembg/releases/tag/v0.0.0) (ONNX 변환본), 원 모델 [xuebinqin/U-2-Net](https://github.com/xuebinqin/U-2-Net) | 원 모델 Apache-2.0 ([전문](LICENSES/U-2-Net-Apache-2.0.txt)), 변환·배포 rembg MIT ([전문](LICENSES/rembg-MIT.txt)) |

내려받기 주소: `https://github.com/seoulmetroddm/lost-camera-models/releases/download/<태그>/<파일>`

## 규칙

- 올린 파일은 바꾸지 않는다. 모델이 바뀌면 새 태그(예: `u2netp-v2`)로 올린다.
- 업무(상업적) 이용이 허용된 라이선스만 올리고, 라이선스 전문을 `LICENSES/`에 둔다.
- 올리지 않는 것: BRIA RMBG(비상업 전용), `@imgly/background-removal`(AGPL).

## 라이선스 메모

- U²-Net 저장소는 Apache-2.0이며, README에 가중치만 따로 다르게 정한 조건은 없다 (2026-10-20 확인).
- `u2netp.onnx`는 원 저자가 배포한 `u2netp.pth`를 rembg가 ONNX로 변환해 배포한 것을 수정 없이 다시 배포한다.
