# ComfyUI + Wan2.2 (I2V) Colab セットアップ

[Zuntan03/EasyWan22](https://github.com/Zuntan03/EasyWan22) の構成を参考に、Google Colab 上で
ComfyUI + Wan2.2（Image-to-Video）をワンクリックで起動できるノートブックです。

## ファイル

- [`ComfyUI_Wan2.2_I2V_Colab.ipynb`](./ComfyUI_Wan2.2_I2V_Colab.ipynb) — Colab用セットアップノートブック

## Google Colabで開く

以下のURLをブラウザで開くと、GitHub上のこのノートブックが直接 Google Colab で開きます
（このリポジトリを GitHub に push した後に有効になります）。

```
https://colab.research.google.com/github/l1istt/neomangaka-site/blob/main/colab/ComfyUI_Wan2.2_I2V_Colab.ipynb
```

## 内容

1. GPUの確認
2. Googleドライブへのインストール（任意・推奨）
3. ComfyUI本体のインストール
4. ComfyUI-Manager / Wan2.2関連カスタムノード（ComfyUI-WanVideoWrapper, ComfyUI-GGUF,
   ComfyUI-KJNodes, ComfyUI-VideoHelperSuite）のインストール
5. Wan2.2 I2Vモデル（fp8スケール版 or GGUF量子化版）、VAE、テキストエンコーダー、
   CLIP Visionモデルのダウンロード（Hugging Faceから）
6. cloudflared（Cloudflare Tunnel）のセットアップ
7. ComfyUIの起動と、外部アクセス用URLの表示

生徒は上から順にセルを実行する（またはメニューの「ランタイム」→「すべてのセルを実行」）だけで、
ComfyUIの外部アクセスURLが最後のセルの出力に表示されます。
