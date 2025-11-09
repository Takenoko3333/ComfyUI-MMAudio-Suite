[English](#English) | [日本語](#日本語)

---
# English

# ComfyUI nodes to use [MMAudio](https://github.com/hkchengrex/MMAudio)

## WIP WIP WIP

https://github.com/user-attachments/assets/9515c0f6-cc5d-4dfe-a642-f841a1a2dba5

## About this custom node

This is a custom node that applies the pull request (pr52) fixing bugs in ComfyUI-MMAudio and adds pitch adjustment functionality.<br>
The pitch adjustment feature integrates [comfyui-audio-pitch](https://github.com/Takenoko3333/comfyui-audio-pitch).<br>
This makes MMAudio easier to implement and is expected to improve performance.<br>
We plan to add features like Bass/Treble adjustment in the future.

## Installation
Navigate to ComfyUI\custom_nodes
```
git clone https://github.com/Takenoko3333/ComfyUI-MMAudio-Suite.git
```
Please restart ComfyUI.

## Models

Models are loaded from `ComfyUI/models/mmaudio`

Download the fp16 safetensors model from the following link:
Safetensors available here:

[https://huggingface.co/Kijai/MMAudio_safetensors/tree/main](https://huggingface.co/Kijai/MMAudio_safetensors/tree/main)

Nvidia bigvganv2 (used with 44k mode)

[https://huggingface.co/nvidia/bigvgan_v2_44khz_128band_512x](https://huggingface.co/nvidia/bigvgan_v2_44khz_128band_512x)

is autodownloaded to `ComfyUI/models/mmaudio/nvidia/bigvgan_v2_44khz_128band_512x`

The first time you run it, downloading Nvidia-related files may take some time.

---
# 日本語

# ComfyUI nodes to use [MMAudio](https://github.com/hkchengrex/MMAudio)

## WIP WIP WIP

https://github.com/user-attachments/assets/9515c0f6-cc5d-4dfe-a642-f841a1a2dba5

## このカスタムノードについて

ComfyUI-MMAudioのバグを修正のプルリクエスト（pr52）を適用し、ピッチ調整機能を加えたカスタムノードです。<br>
ピッチ調整機能は[comfyui-audio-pitch](https://github.com/Takenoko3333/comfyui-audio-pitch)を統合しました。<br>
これによりMMAudioの導入がし易くなり、性能向上も期待できます。<br>
今後、Bass/Treble調整等の機能を追加していく予定です。

## インストール

ComfyUI\custom_nodes に移動
```
git clone https://github.com/Takenoko3333/ComfyUI-MMAudio-Suite.git
```
ComfyUI を再起動してください。

ポータブル版で依存ファイルがインストールされていない場合：ComfyUI_windows_portableフォルダ内で以下を実行してください：
```
python_embeded\python.exe -m pip install -r ComfyUI\custom_nodes\ComfyUI-MMAudio-Suite\requirements.txt
```

## Models

モデルは以下に配置します `ComfyUI/models/mmaudio`

Safetensorsは以下よりfp16をダウンロードしてください:

[https://huggingface.co/Kijai/MMAudio_safetensors/tree/main](https://huggingface.co/Kijai/MMAudio_safetensors/tree/main)

Nvidia bigvganv2 (used with 44k mode)

[https://huggingface.co/nvidia/bigvgan_v2_44khz_128band_512x](https://huggingface.co/nvidia/bigvgan_v2_44khz_128band_512x)

自動的にダウンロードされます `ComfyUI/models/mmaudio/nvidia/bigvgan_v2_44khz_128band_512x`

初回実行時ははNvidia関連ファイルのダウントードに時間がかかります。
