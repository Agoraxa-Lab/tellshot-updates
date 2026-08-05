# Tellshot Updates

Tellshot のソフトウェア更新配信専用リポジトリです(旧: mendaco-updates)。

- Tellshot のソースコードは置きません。
- EdDSA 秘密鍵、GitHub token、Apple の署名・公証資格情報は置きません。
- GitHub Releases には署名・公証済みの更新 ZIP だけを配置します。
- `appcast.xml` は GitHub Pages から配信します。

## 公開順序

1. GitHub Release asset を公開する。
2. asset の HTTPS 取得、サイズ、SHA-256 を検証する。
3. 検証成功後に限り、`appcast.xml` を最後に更新する。

参照中の asset を先に削除せず、失敗時は直前の正常な `appcast.xml` を維持します。

問い合わせ先: [Agoraxa-Lab](https://github.com/Agoraxa-Lab)
