# KryVenta Image AI Models

Versioned on-device neural models used by KryVenta Enhance Image tools.

## v1.0.0 model pack

| Tool stage | Model | File | Exact bytes | SHA-256 |
| --- | --- | --- | ---: | --- |
| Background removal | BiRefNet General FP16 (1024 px) | `birefnet-general-fp16.onnx` | 489,666,272 | `3654c741eb80bd926ada8fed1713b506ccf8d30eb1f6487e87eb9f234f33df09` |
| Person instances | RF-DETR Seg Preview (432 px) | `rf-detr-seg-preview.onnx` | 134,443,363 | `42e3571cf64d70df6f6acf3c5dcf0fc4ecbf8bab46d819ca8e4e94d4cee4de9b` |
| Background reconstruction | LaMa (512 px) | `lama-inpainting.onnx` | 92,591,623 | `7df918ac3921d3daf0aae1d219776cf0dc4e4935f035af81841b40adcf74fdf2` |

All files are hosted in the v1.0.0 GitHub Release. KryVenta downloads only the model needed by the selected tool, resumes interrupted transfers, and validates exact byte length plus SHA-256 before ONNX Runtime opens it.

## Upstream projects and licenses

- [BiRefNet](https://github.com/ZhengPeng7/BiRefNet) - MIT
- [RF-DETR](https://github.com/roboflow/rf-detr) - Apache-2.0 designated open models
- [LaMa](https://github.com/advimman/lama) and the [OpenCV ONNX conversion](https://huggingface.co/opencv/inpainting_lama)

See each upstream project for its full model and license documentation.