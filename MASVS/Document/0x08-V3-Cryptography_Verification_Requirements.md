# V3: 暗号要件

## 制御目標

暗号はモバイルデバイスに保存されたデータを守ることに関して不可欠な要因である。特に標準の慣習が守られていないとき、それは物事がひどく間違っている可能性のあるカテゴリでもある。本章における制御の目的は、検証されたアプリケーションが以下のような業界のベストプラクティスに従って暗号を使用することを確保することである。

- 実績のある暗号ライブラリの使用
- 暗号プリミティブの適切な選択と設定
- ランダム性が必要な場合は、適切な乱数生成機を使用

## セキュリティ検証要件

| # | 説明 | L1 | L2 |
| --- | --- | --- | --- |
| **3.1** | 唯一の暗号方式として、アプリがハードコードされたキーを用いた対称暗号(秘密鍵暗号)に頼らない | ✓ | ✓ |
| **3.2** | アプリが実績のある暗号プリミティブの実装を使用している | ✓ | ✓ |
| **3.3** | アプリが業界のベストプラクティスに準拠したパラメータで構成された特定のユースケースに適切な暗号プリミティブを使用している | ✓ | ✓ |
| **3.4** | セキュリティの目的で脆弱であると広く考えられている暗号プロトコルやアルゴリズムをアプリが使用していない | ✓ | ✓ |
| **3.5** | アプリが複数の目的で同じ暗号鍵を再利用しない | ✓ | ✓ |
| **3.6** | すべての乱数が十分にセキュアな乱数生成機を用いて生成されている | ✓ | ✓ |

## 参考文献

OWASP モバイルセキュリティテストガイドは、本セクションに記載されている要件を検証するための詳細な指示を提供する。

- Android - https://github.com/OWASP/owasp-mstg/blob/master/Document/0x05e-Testing-Cryptography.md
- iOS - https://github.com/OWASP/owasp-mstg/blob/master/Document/0x06e-Testing-Cryptography.md

詳細は以下参照：

- OWASP Mobile Top 10: [M5 - Insufficient Cryptography(不十分な暗号化)](https://www.owasp.org/index.php/Mobile_Top_10_2016-M5-Insufficient_Cryptography)
- CWE: https://cwe.mitre.org/data/definitions/310.html
