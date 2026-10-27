# studio-ai-t2i — model cho "Tạo Ảnh bằng Prompt" (bản Nhanh)

Kho này chỉ chứa **trọng số model** (chia mảnh < 50 MB) để ứng dụng https://yosimura99.github.io/studio-ai/ tải về và chạy **ngay trong trình duyệt** (WebGPU / WASM), không cần máy chủ, không cần API key.

- Model: **SDXS-512-DreamShaper** (IDKiro) — sinh ảnh 1 bước. Giấy phép: **OpenRAIL++** (cấm dùng sai mục đích theo điều khoản của giấy phép).
- Chuyển đổi: PyTorch → ONNX, lưu trọng số fp16 (`w.NNN`), đồ thị `g16.onnx` (WebGPU fp16) và `g32.onnx` (WASM/fp32; trình duyệt tự giãn fp16 → fp32).
- VAE: AutoencoderTiny đi kèm SDXS.
