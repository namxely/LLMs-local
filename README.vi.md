# LLMs-local (Chạy LLM Cục Bộ)

> 🌐 **Ngôn ngữ:** [English](README.md) | **Tiếng Việt**

Danh sách tổng hợp các nền tảng, công cụ, inference engine và tài nguyên chất lượng cao giúp triển khai và chạy mô hình ngôn ngữ lớn (LLM) cục bộ trên máy cá nhân.

<img src="https://preview.redd.it/my-160gb-local-llm-rig-v0-qukd2c1lzk5f1.jpeg?auto=webp&s=eda341738c4e87aa8d6940d138804df741ea2b08">

## Mục lục

- [Nền tảng chạy Inference](#nền-tảng-chạy-inference)
- [Inference Engines](#inference-engines)
- [Giao diện người dùng (UI)](#giao-diện-người-dùng-ui)
- [Mô hình ngôn ngữ lớn (LLMs)](#mô-hình-ngôn-ngữ-lớn-llms)
  - [Khám phá, Benchmark & Bảng xếp hạng](#khám-phá-benchmark--bảng-xếp-hạng)
  - [Nhà cung cấp mô hình](#nhà-cung-cấp-mô-hình)
  - [Các mô hình cụ thể](#các-mô-hình-cụ-thể)
    - [Đa dụng (General purpose)](#đa-dụng-general-purpose)
    - [Lập trình (Coding)](#lập-trình-coding)
    - [Đa phương thức (Multimodal)](#đa-phương-thức-multimodal)
    - [Hình ảnh (Image)](#hình-ảnh-image)
    - [Âm thanh (Audio)](#âm-thanh-audio)
    - [Mô hình khác](#mô-hình-khác)
- [Công cụ & Hệ sinh thái](#công-cụ--hệ-sinh-thái)
  - [Công cụ tối ưu mô hình](#công-cụ-tối-ưu-mô-hình)
  - [Agent Frameworks](#agent-frameworks)
  - [Model Context Protocol (MCP)](#model-context-protocol-mcp)
  - [Retrieval-Augmented Generation (RAG)](#retrieval-augmented-generation-rag)
  - [Coding Agents (Trợ lý lập trình)](#coding-agents-trợ-lý-lập-trình)
  - [Computer Use (Điều khiển máy tính)](#computer-use-điều-khiển-máy-tính)
  - [Tự động hóa trình duyệt](#tự-động-hóa-trình-duyệt)
  - [Quản lý bộ nhớ (Memory Management)](#quản-lý-bộ-nhớ-memory-management)
  - [Kiểm thử, Đánh giá & Giám sát](#kiểm-thử-đánh-giá--giám-sát)
  - [Nghiên cứu chuyên sâu (Research)](#nghiên-cứu-chuyên-sâu-research)
  - [Huấn luyện & Fine-tuning](#huấn-luyện--fine-tuning)
  - [Công cụ khác](#công-cụ-khác)
- [Phần cứng (Hardware)](#phần-cứng-hardware)
- [Tài liệu & Hướng dẫn (Tutorials)](#tài-liệu--hướng-dẫn-tutorials)
  - [Kiến thức Mô hình](#kiến-thức-mô-hình)
  - [Prompt Engineering](#prompt-engineering)
  - [Context Engineering](#context-engineering)
  - [Triển khai Inference](#triển-khai-inference)
  - [Xây dựng AI Agents](#xây-dựng-ai-agents)
  - [Kỹ thuật RAG](#kỹ-thuật-rag)
  - [Hướng dẫn khác](#hướng-dẫn-khác)
- [Credits & References (Nguồn tham khảo & Bản quyền)](#credits--references-nguồn-tham-khảo--bản-quyền)

## Nền tảng chạy Inference

- [LM Studio](https://lmstudio.ai/) - ứng dụng desktop giúp tìm kiếm, tải và chạy LLM cục bộ dễ dàng
- <img src="https://img.shields.io/github/stars/menloresearch/jan?style=social" height="17" align="texttop"/> [jan](https://github.com/menloresearch/jan) - giải pháp thay thế ChatGPT mã nguồn mở chạy 100% offline trên máy tính của bạn
- <img src="https://img.shields.io/github/stars/mudler/LocalAI?style=social" height="17" align="texttop"/> [LocalAI](https://github.com/mudler/LocalAI) - nền tảng mã nguồn mở thay thế OpenAI, Claude API ngay trên hạ tầng cục bộ
- <img src="https://img.shields.io/github/stars/ChatBoxAI/ChatBox?style=social" height="17" align="texttop"/> [ChatBox](https://github.com/ChatBoxAI/ChatBox) - ứng dụng desktop thân thiện để kết nối và trò chuyện với các mô hình AI/LLM
- <img src="https://img.shields.io/github/stars/lemonade-sdk/lemonade?style=social" height="17" align="texttop"/> [lemonade](https://github.com/lemonade-sdk/lemonade) - máy chủ LLM cục bộ hỗ trợ tăng tốc GPU và NPU
- <img src="https://img.shields.io/github/stars/nomic-ai/gpt4all?style=social" height="17" align="texttop"/> [GPT4All](https://github.com/nomic-ai/gpt4all) - ứng dụng desktop đa nền tảng chạy LLM cục bộ tích hợp sẵn LocalDocs RAG bảo mật dữ liệu

[Quay lại Mục lục](#mục-lục)

## Inference Engines

- <img src="https://img.shields.io/github/stars/ollama/ollama?style=social" height="17" align="texttop"/> [ollama](https://github.com/ollama/ollama) - công cụ CLI phổ biến nhất để tải và chạy LLM cục bộ nhanh chóng
- <img src="https://img.shields.io/github/stars/ggml-org/llama.cpp?style=social" height="17" align="texttop"/> [llama.cpp](https://github.com/ggml-org/llama.cpp) - engine suy luận LLM tối ưu viết bằng C/C++
- <img src="https://img.shields.io/github/stars/vllm-project/vllm?style=social" height="17" align="texttop"/> [vllm](https://github.com/vllm-project/vllm) - engine serving thông lượng cao và tối ưu bộ nhớ (PagedAttention) cho LLM
- <img src="https://img.shields.io/github/stars/exo-explore/exo?style=social" height="17" align="texttop"/> [exo](https://github.com/exo-explore/exo) - ghép nhiều thiết bị phổ thông tại nhà thành cụm AI cluster
- <img src="https://img.shields.io/github/stars/microsoft/BitNet?style=social" height="17" align="texttop"/> [BitNet](https://github.com/microsoft/BitNet) - framework suy luận chính thức từ Microsoft cho các mô hình LLM 1-bit
- <img src="https://img.shields.io/github/stars/sgl-project/sglang?style=social" height="17" align="texttop"/> [sglang](https://github.com/sgl-project/sglang) - framework serving tốc độ cao cho LLM và mô hình ngôn ngữ - thị giác (VLM)
- <img src="https://img.shields.io/github/stars/GeeeekExplorer/nano-vllm?style=social" height="17" align="texttop"/> [Nano-vLLM](https://github.com/GeeeekExplorer/nano-vllm) - bản cài đặt vLLM gọn nhẹ viết lại từ đầu
- <img src="https://img.shields.io/github/stars/LostRuins/koboldcpp?style=social" height="17" align="texttop"/> [koboldcpp](https://github.com/LostRuins/koboldcpp) - chạy mô hình GGUF dễ dàng đi kèm giao diện KoboldAI
- <img src="https://img.shields.io/github/stars/gpustack/gpustack?style=social" height="17" align="texttop"/> [gpustack](https://github.com/gpustack/gpustack) - triển khai cụm mô hình AI phân tán trên nhiều GPU đơn giản, dễ mở rộng
- <img src="https://img.shields.io/github/stars/ml-explore/mlx-lm?style=social" height="17" align="texttop"/> [mlx-lm](https://github.com/ml-explore/mlx-lm) - sinh văn bản và fine-tune LLM trên chip Apple Silicon bằng MLX
- <img src="https://img.shields.io/github/stars/b4rtaz/distributed-llama?style=social" height="17" align="texttop"/> [distributed-llama](https://github.com/b4rtaz/distributed-llama) - kết nối các thiết bị gia đình thành cụm tăng tốc suy luận LLM
- <img src="https://img.shields.io/github/stars/ikawrakow/ik_llama.cpp?style=social" height="17" align="texttop"/> [ik_llama.cpp](https://github.com/ikawrakow/ik_llama.cpp) - bản fork của llama.cpp bổ sung nhiều định dạng quant mới và tối ưu hiệu năng
- <img src="https://img.shields.io/github/stars/FastFlowLM/FastFlowLM?style=social" height="17" align="texttop"/> [FastFlowLM](https://github.com/FastFlowLM/FastFlowLM) - chạy LLM trực tiếp trên NPU AMD Ryzen™ AI
- <img src="https://img.shields.io/github/stars/nlzy/vllm-gfx906?style=social" height="17" align="texttop"/> [vllm-gfx906](https://github.com/nlzy/vllm-gfx906) - bản vLLM tối ưu cho GPU AMD gfx906 (Radeon VII / MI50 / MI60)
- <img src="https://img.shields.io/github/stars/intel/llm-scaler?style=social" height="17" align="texttop"/> [llm-scaler](https://github.com/intel/llm-scaler) - chạy LLM tối ưu trên GPU Intel Arc™ Pro B60
- <img src="https://img.shields.io/github/stars/Mozilla-Ocho/llamafile?style=social" height="17" align="texttop"/> [llamafile](https://github.com/Mozilla-Ocho/llamafile) - đóng gói và chạy LLM chỉ bằng một tệp thực thi duy nhất (Mozilla Ocho)
- <img src="https://img.shields.io/github/stars/theroyallab/tabbyAPI?style=social" height="17" align="texttop"/> [TabbyAPI](https://github.com/theroyallab/tabbyAPI) - máy chủ API suy luận cục bộ tương thích OpenAI tốc độ cao dùng ExLlamaV2/ExLlamaV3
- <img src="https://img.shields.io/github/stars/containers/ramalama?style=social" height="17" align="texttop"/> [RamaLama](https://github.com/containers/ramalama) - công cụ CLI dựa trên container để quản lý và chạy mô hình AI cục bộ an toàn

[Quay lại Mục lục](#mục-lục)

## Giao diện người dùng (UI)

- <img src="https://img.shields.io/github/stars/open-webui/open-webui?style=social" height="17" align="texttop"/> [Open WebUI](https://github.com/open-webui/open-webui) - giao diện web AI thân thiện, hỗ trợ Ollama, OpenAI API và RAG
- <img src="https://img.shields.io/github/stars/lobehub/lobe-chat?style=social" height="17" align="texttop"/> [Lobe Chat](https://github.com/lobehub/lobe-chat) - nền tảng chat AI mã nguồn mở với thiết kế hiện đại và hệ thống plugin phong phú
- <img src="https://img.shields.io/github/stars/oobabooga/text-generation-webui?style=social" height="17" align="texttop"/> [Text generation web UI](https://github.com/oobabooga/text-generation-webui) - giao diện Gradio cho LLM hỗ trợ nhiều backend và tùy biến sâu
- <img src="https://img.shields.io/github/stars/SillyTavern/SillyTavern?style=social" height="17" align="texttop"/> [SillyTavern](https://github.com/SillyTavern/SillyTavern) - giao diện LLM chuyên sâu cho người dùng nâng cao và roleplay
- <img src="https://img.shields.io/github/stars/n4ze3m/page-assist?style=social" height="17" align="texttop"/> [Page Assist](https://github.com/n4ze3m/page-assist) - tiện ích trình duyệt kết nối LLM cục bộ để hỗ trợ đọc và tóm tắt trang web
- <img src="https://img.shields.io/github/stars/CherryHQ/cherry-studio?style=social" height="17" align="texttop"/> [Cherry Studio](https://github.com/CherryHQ/cherry-studio) - ứng dụng AI desktop hỗ trợ Ollama, API tương thích OpenAI cục bộ và MCP servers

[Quay lại Mục lục](#mục-lục)

## Mô hình ngôn ngữ lớn (LLMs)

### Khám phá, Benchmark & Bảng xếp hạng

- [AI Models & API Providers Analysis](https://artificialanalysis.ai/) - phân tích tốc độ, chi phí và chất lượng các mô hình và nhà cung cấp AI
- [LLM Explorer](https://llm-explorer.com/) - tra cứu danh sách các mô hình LLM mã nguồn mở
- [Dubesor LLM Benchmark table](https://dubesor.de/benchtable) - bảng so sánh hiệu năng suy luận thực tế trên phần cứng cá nhân
- [oobabooga benchmark](https://oobabooga.github.io/benchmark.html) - bảng đo lường điểm chuẩn sắp xếp theo dung lượng lưu trữ trên đĩa

[Quay lại Mục lục](#mục-lục)

### Nhà cung cấp mô hình

- [Qwen](https://huggingface.co/Qwen) - dòng mô hình mở mạnh mẽ phát triển bởi Alibaba Cloud
- <img src="https://img.shields.io/badge/Mistral%20AI-%23FA520F?logo=mistralai&logoColor=%23FFFFFF" height="17" align="texttop"/> [Mistral AI](https://huggingface.co/mistralai) - startup AI hàng đầu tại Pháp với nhiều mô hình open-weights hiệu năng cao
- [Tencent](https://huggingface.co/tencent) - kho mô hình mã nguồn mở từ tập đoàn công nghệ Tencent
- [Unsloth AI](https://huggingface.co/unsloth) - cung cấp các bản lượng tử hóa GGUF/Dynamic tối ưu và bộ công cụ fine-tune nhanh
- [bartowski](https://huggingface.co/bartowski) - cộng tác viên uy tín chuyên cung cấp bản lượng tử hóa GGUF của các LLM phổ biến
- [Beijing Academy of Artificial Intelligence](https://huggingface.co/BAAI) - viện nghiên cứu AI phi lợi nhuận với nhiều mô hình embedding và LLM chất lượng
- [Open Thoughts](https://huggingface.co/open-thoughts) - nhóm nghiên cứu tổng hợp các bộ dữ liệu suy luận (reasoning datasets) mở

[Quay lại Mục lục](#mục-lục)

### Các mô hình cụ thể

#### Đa dụng (General purpose)

- [DiffusionGemma-26B-A4B-it](https://huggingface.co/google/diffusiongemma-26B-A4B-it) - mô hình đa phương thức dựa trên kiến trúc khuếch tán (diffusion) 26B MoE từ Google, tốc độ cao trên phần cứng cá nhân
- [MiniMax M3](https://huggingface.co/minimax-ai/MiniMax-M3) - mô hình open-weights ngữ cảnh 1M token, đa phương thức và tối ưu cho lập trình/agent
- [DeepSeek-V4](https://huggingface.co/deepseek-ai/DeepSeek-V4) - dòng mô hình mới nhất của DeepSeek (V4-Pro & Flash) nổi bật về suy luận dài và viết mã
- [Kimi-K2.6](https://huggingface.co/moonshotai/Kimi-K2.6) - mô hình ngữ cảnh dài định hướng tác vụ agent từ Moonshot AI
- [Qwen3-Next](https://huggingface.co/collections/Qwen/qwen3-next-68c25fd6838e585db8eeea9d) - bộ sưu tập các mô hình Qwen thế hệ mới nhất
- <img src="https://img.shields.io/badge/Google-%234285F4?logo=google&logoColor=red" height="17" align="texttop"/> [Gemma 3](https://huggingface.co/collections/google/gemma-3-release-67c6c6f89c4f76621268bb6d) - họ mô hình mở gọn nhẹ, hiệu suất cao của Google xây dựng trên công nghệ Gemini
- <img src="https://img.shields.io/badge/OpenAI-%23412991?logo=openai" height="17" align="texttop"/> [gpt-oss](https://huggingface.co/collections/openai/gpt-oss-68911959590a1634ba11c7a4) - bộ mô hình open-weights từ OpenAI phục vụ suy luận, tác vụ agent và phát triển phần mềm
- <img src="https://img.shields.io/badge/Mistral%20AI-%23FA520F?logo=mistralai&logoColor=%23FFFFFF" height="17" align="texttop"/> [Ministral 3](https://huggingface.co/collections/mistralai/ministral-3) - dòng mô hình chạy biên (3B, 8B, 14B) hỗ trợ xử lý thị giác
- [GLM-4.5](https://huggingface.co/collections/zai-org/glm-45-687c621d34bda8c9e4bf503b) - dòng mô hình suy luận lai (hybrid reasoning) thiết kế cho agent thông minh
- [Hunyuan](https://huggingface.co/collections/tencent/hunyuan-dense-model-6890632cda26b19119c9c5e7) - dòng LLM hiệu năng cao mã nguồn mở của Tencent
- [Phi-4-mini-instruct](https://huggingface.co/microsoft/Phi-4-mini-instruct) - mô hình nhỏ gọn từ Microsoft huấn luyện trên dữ liệu tổng hợp chất lượng cao
- [NVIDIA Nemotron v3](https://huggingface.co/collections/nvidia/nvidia-nemotron-v3) - họ mô hình mở từ NVIDIA tối ưu cho agent chuyên biệt
- [Llama Nemotron](https://huggingface.co/collections/nvidia/llama-nemotron-67d92346030a2691293f200b) - dòng mô hình doanh nghiệp sẵn sàng triển khai từ NVIDIA
- [OpenReasoning-Nemotron](https://huggingface.co/collections/nvidia/openreasoning-nemotron-687730dae0170059860f1f01) - mô hình NVIDIA huấn luyện trên 5 triệu chuỗi suy luận toán, code và khoa học
- [Granite 4.0](https://huggingface.co/collections/ibm-granite/granite-40-language-models-6811a18b820ef362d9e5a82c) - họ mô hình nền tảng đa ngôn ngữ của IBM hỗ trợ RAG, gọi công cụ và JSON có cấu trúc
- [EXAONE-4.0](https://huggingface.co/collections/LGAI-EXAONE/exaone-40-686b2e0069800c835ed48375) - dòng LLM từ LG AI Research tích hợp chế độ suy luận và phản hồi nhanh
- [ERNIE 4.5](https://huggingface.co/collections/baidu/ernie-45-6861cd4c9be84540645f35c9) - bộ mô hình đa phương thức quy mô lớn từ Baidu
- [Seed-OSS](https://huggingface.co/collections/ByteDance-Seed/seed-oss-68a609f4201e788db05b5dcd) - bộ mô hình từ đội ngũ Seed của ByteDance tối ưu ngữ cảnh dài và tác vụ agent

[Quay lại Mục lục](#mục-lục)

#### Lập trình (Coding)

- [Qwen3-Coder](https://huggingface.co/collections/Qwen/qwen3-coder-687fc861e53c939e52d52d10) - dòng mô hình lập trình agentic mạnh mẽ của Qwen
- <img src="https://img.shields.io/badge/Mistral%20AI-%23FA520F?logo=mistralai&logoColor=%23FFFFFF" height="17" align="texttop"/> [Devstral 2](https://huggingface.co/collections/mistralai/devstral-2) - mô hình kỹ thuật phần mềm xuất sắc trong việc khám phá codebase và sửa nhiều tệp cùng lúc
- [Mellum-4b-base](https://huggingface.co/JetBrains/Mellum-4b-base) - mô hình 4B từ JetBrains tối ưu cho tác vụ hoàn thiện mã nguồn
- [OlympicCoder-32B](https://huggingface.co/open-r1/OlympicCoder-32B) - mô hình lập trình đạt điểm cao trên LiveCodeBench và các kỳ thi lập trình
- [NextCoder](https://huggingface.co/collections/microsoft/nextcoder-6815ee6bfcf4e42f20d45028) - họ mô hình chỉnh sửa mã nguồn từ Microsoft phát triển trên nền Qwen2.5-Coder

[Quay lại Mục lục](#mục-lục)

#### Đa phương thức (Multimodal)

- [Qwen3-Omni](https://huggingface.co/collections/Qwen/qwen3-omni-68d100a86cd0906843ceccbe) - bộ mô hình nền tảng đa phương thức toàn diện đầu-cuối đa ngôn ngữ từ Qwen

[Quay lại Mục lục](#mục-lục)

#### Hình ảnh (Image)

- [Qwen-Image](https://huggingface.co/Qwen/Qwen-Image) - mô hình sinh ảnh nền tảng nổi bật với khả năng hiển thị chữ phức tạp và chỉnh sửa ảnh chính xác
- [Qwen-Image-Edit-2509](https://huggingface.co/Qwen/Qwen-Image-Edit-2509) - phiên bản chuyên chỉnh sửa ảnh và văn bản trên ảnh của Qwen-Image
- [Qwen3-VL](https://huggingface.co/collections/Qwen/qwen3-vl-68d2a7c1b8a8afce4ebd2dbe) - bộ mô hình thị giác - ngôn ngữ (VLM) mạnh nhất dòng Qwen
- [GLM-4.5V](https://huggingface.co/zai-org/GLM-4.5V) - mô hình VLM phát triển trên nền tảng GLM-4.5-Air
- [HunyuanImage-2.1](https://huggingface.co/tencent/HunyuanImage-2.1) - mô hình khuếch tán sinh ảnh độ phân giải 2K hiệu quả của Tencent
- [FastVLM](https://huggingface.co/collections/apple/fastvlm-68ac97b9cd5cacefdd04872e) - bộ mô hình VLM tối ưu tốc độ mã hóa hình ảnh từ Apple
- [MiniCPM-V-4_5](https://huggingface.co/openbmb/MiniCPM-V-4_5) - mô hình đa phương thức gọn nhẹ xử lý ảnh đơn, đa ảnh và video ngay trên điện thoại
- [LFM2-VL](https://huggingface.co/collections/LiquidAI/lfm2-vl-68963bbc84a610f7638d5ffa) - họ mô hình thị giác - ngôn ngữ tối ưu triển khai trực tiếp trên thiết bị (on-device)
- [ClipTagger-12b](https://huggingface.co/inference-net/ClipTagger-12b) - mô hình VLM 12B chuyên hiểu và gắn thẻ nội dung video quy mô lớn

[Quay lại Mục lục](#mục-lục)

#### Âm thanh (Audio)

- <img src="https://img.shields.io/badge/Mistral%20AI-%23FA520F?logo=mistralai&logoColor=%23FFFFFF" height="17" align="texttop"/> [Voxtral-Small-24B-2507](https://huggingface.co/mistralai/Voxtral-Small-24B-2507) - mô hình xử lý đầu vào âm thanh chất lượng cao dựa trên Mistral Small 3
- [chatterbox](https://huggingface.co/ResembleAI/chatterbox) - mô hình chuyển văn bản thành giọng nói (TTS) mã nguồn mở cấp độ production từ ResembleAI
- [VibeVoice](https://huggingface.co/collections/microsoft/vibevoice-68a2ef24a875c44be47b034f) - bộ mô hình TTS tiên tiến từ Microsoft
- [canary-1b-v2](https://huggingface.co/nvidia/canary-1b-v2) - mô hình nhận dạng và dịch giọng nói đa tác vụ từ NVIDIA
- [parakeet-tdt-0.6b-v3](https://huggingface.co/nvidia/parakeet-tdt-0.6b-v3) - mô hình chuyển giọng nói thành văn bản (STT) đa ngôn ngữ gọn nhẹ từ NVIDIA
- [Kitten TTS](https://huggingface.co/KittenML/models) - bộ mô hình TTS mã nguồn mở siêu nhẹ cho triển khai cục bộ

[Quay lại Mục lục](#mục-lục)

#### Mô hình khác

- [Jan-v1-4B](https://huggingface.co/janhq/Jan-v1-4B) - mô hình đầu tiên trong họ Jan tối ưu cho suy luận và giải quyết vấn đề trong Jan App
- [Jan-nano](https://huggingface.co/Menlo/Jan-nano) - mô hình 4B gọn nhẹ huấn luyện chuyên sâu cho tác vụ tra cứu nghiên cứu
- [Jan-nano-128k](https://huggingface.co/Menlo/Jan-nano-128k) - phiên bản Jan-nano hỗ trợ cửa sổ ngữ cảnh gốc 128k token
- [Arch-Router-1.5B](https://huggingface.co/katanemo/Arch-Router-1.5B) - mô hình điều phối (router) tốc độ cao định tuyến prompt theo sở thích người dùng
- [gpt-oss-safeguard](https://huggingface.co/collections/openai/gpt-oss-safeguard) - bộ mô hình kiểm duyệt an toàn xây dựng trên nền gpt-oss
- [Qwen3Guard](https://huggingface.co/collections/Qwen/qwen3guard-68d2729abbfae4716f3343a1) - bộ mô hình kiểm duyệt an toàn xây dựng trên nền Qwen3
- [HunyuanWorld-1](https://huggingface.co/tencent/HunyuanWorld-1) - mô hình sinh thế giới 3D mã nguồn mở
- [Hunyuan-GameCraft-1.0](https://huggingface.co/tencent/Hunyuan-GameCraft-1.0) - framework sinh video tương tác động cao trong môi trường game

[Quay lại Mục lục](#mục-lục)

## Công cụ & Hệ sinh thái

### Công cụ tối ưu mô hình

- <img src="https://img.shields.io/github/stars/unslothai/unsloth?style=social" height="17" align="texttop"/> [unsloth](https://github.com/unslothai/unsloth) - công cụ fine-tuning và học tăng cường (RL) cho LLM nhanh và tiết kiệm VRAM
- <img src="https://img.shields.io/github/stars/dottxt-ai/outlines?style=social" height="17" align="texttop"/> [outlines](https://github.com/dottxt-ai/outlines) - ép đầu ra có cấu trúc (JSON, regex, schema) cho LLM
- <img src="https://img.shields.io/github/stars/p-e-w/heretic?style=social" height="17" align="texttop"/> [heretic](https://github.com/p-e-w/heretic) - công cụ tự động gỡ bỏ cơ chế từ chối/kiểm duyệt trên mô hình ngôn ngữ mở
- <img src="https://img.shields.io/github/stars/mostlygeek/llama-swap?style=social" height="17" align="texttop"/> [llama-swap](https://github.com/mostlygeek/llama-swap) - chuyển đổi mô hình linh hoạt cho mọi máy chủ tương thích OpenAI cục bộ (llama.cpp, vLLM,...)

[Quay lại Mục lục](#mục-lục)

### Agent Frameworks

- <img src="https://img.shields.io/github/stars/Significant-Gravitas/AutoGPT?style=social" height="17" align="texttop"/> [AutoGPT](https://github.com/Significant-Gravitas/AutoGPT) - nền tảng tạo, triển khai và quản lý AI agent tự động hóa quy trình phức tạp
- <img src="https://img.shields.io/github/stars/langflow-ai/langflow?style=social" height="17" align="texttop"/> [langflow](https://github.com/langflow-ai/langflow) - công cụ trực quan xây dựng và triển khai AI agent cùng workflow
- <img src="https://img.shields.io/github/stars/langchain-ai/langchain?style=social" height="17" align="texttop"/> [langchain](https://github.com/langchain-ai/langchain) - framework phổ biến xây dựng ứng dụng suy luận nhận biết ngữ cảnh
- <img src="https://img.shields.io/github/stars/microsoft/autogen?style=social" height="17" align="texttop"/> [autogen](https://github.com/microsoft/autogen) - framework lập trình đa tác tử (multi-agent AI) từ Microsoft
- <img src="https://img.shields.io/github/stars/Mintplex-Labs/anything-llm?style=social" height="17" align="texttop"/> [anything-llm](https://github.com/Mintplex-Labs/anything-llm) - ứng dụng AI tất-cả-trong-một (Desktop & Docker) tích hợp sẵn RAG, AI agent no-code và MCP
- <img src="https://img.shields.io/github/stars/FlowiseAI/Flowise?style=social" height="17" align="texttop"/> [Flowise](https://github.com/FlowiseAI/Flowise) - kéo thả trực quan để thiết kế luồng AI agent và RAG
- <img src="https://img.shields.io/github/stars/run-llama/llama_index?style=social" height="17" align="texttop"/> [llama_index](https://github.com/run-llama/llama_index) - framework hàng đầu kết nối LLM và agent với dữ liệu riêng của bạn
- <img src="https://img.shields.io/github/stars/crewAIInc/crewAI?style=social" height="17" align="texttop"/> [crewAI](https://github.com/crewAIInc/crewAI) - framework điều phối nhiều AI agent đóng vai phối hợp tự động
- <img src="https://img.shields.io/github/stars/agno-agi/agno?style=social" height="17" align="texttop"/> [agno](https://github.com/agno-agi/agno) - framework full-stack xây dựng hệ thống Multi-Agent kèm bộ nhớ, tri thức và suy luận
- <img src="https://img.shields.io/github/stars/simstudioai/sim?style=social" height="17" align="texttop"/> [sim](https://github.com/simstudioai/sim) - nền tảng mã nguồn mở xây dựng và triển khai workflow AI agent
- <img src="https://img.shields.io/badge/OpenAI-%23412991?logo=openai" height="17" align="texttop"/> <img src="https://img.shields.io/github/stars/openai/openai-agents-python?style=social" height="17" align="texttop"/> [openai-agents-python](https://github.com/openai/openai-agents-python) - framework Python gọn nhẹ cho các luồng multi-agent
- <img src="https://img.shields.io/github/stars/TransformerOptimus/SuperAGI?style=social" height="17" align="texttop"/> [SuperAGI](https://github.com/TransformerOptimus/SuperAGI) - framework mã nguồn mở giúp xây dựng, quản lý và vận hành AI agent tự chủ
- <img src="https://img.shields.io/github/stars/camel-ai/camel?style=social" height="17" align="texttop"/> [camel](https://github.com/camel-ai/camel) - framework nghiên cứu và triển khai hệ thống đa tác tử (multi-agent)
- <img src="https://img.shields.io/github/stars/pydantic/pydantic-ai?style=social" height="17" align="texttop"/> [pydantic-ai](https://github.com/pydantic/pydantic-ai) - framework AI agent Python chuẩn type-safe cho môi trường production
- <img src="https://img.shields.io/github/stars/neuml/txtai?style=social" height="17" align="texttop"/> [txtai](https://github.com/neuml/txtai) - framework AI tìm kiếm ngữ nghĩa, điều phối LLM và pipeline dữ liệu
- <img src="https://img.shields.io/github/stars/katanemo/archgw?style=social" height="17" align="texttop"/> [archgw](https://github.com/katanemo/archgw) - proxy hiệu năng cao xử lý guardrail, định tuyến prompt và thống nhất API LLM
- <img src="https://img.shields.io/github/stars/badboysm890/ClaraVerse?style=social" height="17" align="texttop"/> [ClaraVerse](https://github.com/badboysm890/ClaraVerse) - workspace AI cục bộ ưu tiên riêng tư tích hợp Ollama, agent builder, Stable Diffusion và tự động hóa kiểu n8n
- <img src="https://img.shields.io/github/stars/deepsense-ai/ragbits?style=social" height="17" align="texttop"/> [ragbits](https://github.com/deepsense-ai/ragbits) - các khối lắp ghép mô-đun giúp phát triển nhanh ứng dụng GenAI

[Quay lại Mục lục](#mục-lục)

### Model Context Protocol (MCP)

- <img src="https://img.shields.io/github/stars/mindsdb/mindsdb?style=social" height="17" align="texttop"/> [mindsdb](https://github.com/mindsdb/mindsdb) - engine truy vấn liên kết dữ liệu cho AI kiêm MCP Server đa nguồn dữ liệu
- <img src="https://img.shields.io/github/stars/github/github-mcp-server?style=social" height="17" align="texttop"/> [github-mcp-server](https://github.com/github/github-mcp-server) - MCP Server chính thức từ GitHub
- <img src="https://img.shields.io/github/stars/microsoft/playwright-mcp?style=social" height="17" align="texttop"/> [playwright-mcp](https://github.com/microsoft/playwright-mcp) - MCP server điều khiển trình duyệt bằng Playwright
- <img src="https://img.shields.io/github/stars/ChromeDevTools/chrome-devtools-mcp?style=social" height="17" align="texttop"/> [chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) - kết nối Chrome DevTools trực tiếp cho coding agent
- <img src="https://img.shields.io/github/stars/czlonkowski/n8n-mcp?style=social" height="17" align="texttop"/> [n8n-mcp](https://github.com/czlonkowski/n8n-mcp) - MCP giúp AI agent tự động thiết kế và dựng workflow n8n
- <img src="https://img.shields.io/github/stars/awslabs/mcp?style=social" height="17" align="texttop"/> [awslabs/mcp](https://github.com/awslabs/mcp) - bộ AWS MCP Servers chính thức hỗ trợ thao tác hạ tầng AWS
- <img src="https://img.shields.io/github/stars/sooperset/mcp-atlassian?style=social" height="17" align="texttop"/> [mcp-atlassian](https://github.com/sooperset/mcp-atlassian) - MCP server tích hợp Atlassian (Confluence, Jira)

[Quay lại Mục lục](#mục-lục)

### Retrieval-Augmented Generation (RAG)

- <img src="https://img.shields.io/github/stars/pathwaycom/pathway?style=social" height="17" align="texttop"/> [pathway](https://github.com/pathwaycom/pathway) - framework ETL Python xử lý luồng thời gian thực và pipeline RAG
- <img src="https://img.shields.io/github/stars/microsoft/graphrag?style=social" height="17" align="texttop"/> [graphrag](https://github.com/microsoft/graphrag) - hệ thống RAG dựa trên đồ thị tri thức mô-đun hóa của Microsoft
- <img src="https://img.shields.io/github/stars/HKUDS/LightRAG?style=social" height="17" align="texttop"/> [LightRAG](https://github.com/HKUDS/LightRAG) - hệ thống RAG gọn nhẹ, tốc độ truy xuất nhanh
- <img src="https://img.shields.io/github/stars/deepset-ai/haystack?style=social" height="17" align="texttop"/> [haystack](https://github.com/deepset-ai/haystack) - framework điều phối AI cho tìm kiếm ngữ nghĩa, hỏi đáp và chatbot RAG production
- <img src="https://img.shields.io/github/stars/vanna-ai/vanna?style=social" height="17" align="texttop"/> [vanna](https://github.com/vanna-ai/vanna) - framework RAG Python mã nguồn mở chuyên sinh truy vấn SQL
- <img src="https://img.shields.io/github/stars/getzep/graphiti?style=social" height="17" align="texttop"/> [graphiti](https://github.com/getzep/graphiti) - xây dựng đồ thị tri thức thời gian thực làm bộ nhớ cho AI Agent
- <img src="https://img.shields.io/github/stars/onyx-dot-app/onyx?style=social" height="17" align="texttop"/> [onyx](https://github.com/onyx-dot-app/onyx) - nền tảng AI kết nối tài liệu, ứng dụng và tri thức nội bộ doanh nghiệp
- <img src="https://img.shields.io/github/stars/zilliztech/claude-context?style=social" height="17" align="texttop"/> [claude-context](https://github.com/zilliztech/claude-context) - lập chỉ mục toàn bộ codebase làm ngữ cảnh cho coding agent
- <img src="https://img.shields.io/github/stars/pipeshub-ai/pipeshub-ai?style=social" height="17" align="texttop"/> [pipeshub-ai](https://github.com/pipeshub-ai/pipeshub-ai) - nền tảng tìm kiếm doanh nghiệp và tự động hóa workflow có giải thích nguồn gốc

[Quay lại Mục lục](#mục-lục)

### Coding Agents (Trợ lý lập trình)

- <img src="https://img.shields.io/github/stars/zed-industries/zed?style=social" height="17" align="texttop"/> [zed](https://github.com/zed-industries/zed) - trình soạn thảo code thế hệ mới hiệu năng cao tích hợp cộng tác AI
- <img src="https://img.shields.io/github/stars/All-Hands-AI/OpenHands?style=social" height="17" align="texttop"/> [OpenHands](https://github.com/All-Hands-AI/OpenHands) - nền tảng agent tự động phát triển phần mềm mã nguồn mở
- <img src="https://img.shields.io/github/stars/cline/cline?style=social" height="17" align="texttop"/> [cline](https://github.com/cline/cline) - coding agent tự chủ ngay trong IDE có thể tạo/sửa file, chạy lệnh và điều khiển trình duyệt
- <img src="https://img.shields.io/github/stars/Aider-AI/aider?style=social" height="17" align="texttop"/> [aider](https://github.com/Aider-AI/aider) - trợ lý lập trình theo cặp (AI pair programming) ngay trên terminal
- <img src="https://img.shields.io/github/stars/sst/opencode?style=social" height="17" align="texttop"/> [opencode](https://github.com/sst/opencode) - coding agent mã nguồn mở tối ưu cho terminal
- <img src="https://img.shields.io/github/stars/TabbyML/tabby?style=social" height="17" align="texttop"/> [tabby](https://github.com/TabbyML/tabby) - giải pháp tự host thay thế GitHub Copilot bằng mô hình cục bộ
- <img src="https://img.shields.io/github/stars/continuedev/continue?style=social" height="17" align="texttop"/> [continue](https://github.com/continuedev/continue) - tiện ích IDE mã nguồn mở cho phép tùy biến trợ lý code và kết nối mọi LLM cục bộ
- <img src="https://img.shields.io/github/stars/voideditor/void?style=social" height="17" align="texttop"/> [void](https://github.com/voideditor/void) - trình soạn thảo mã nguồn mở thay thế Cursor hỗ trợ host mô hình cục bộ
- <img src="https://img.shields.io/github/stars/block/goose?style=social" height="17" align="texttop"/> [goose](https://github.com/block/goose) - AI agent mã nguồn mở có khả năng mở rộng vượt ra ngoài gợi ý code đơn thuần
- <img src="https://img.shields.io/github/stars/RooCodeInc/Roo-Code?style=social" height="17" align="texttop"/> [Roo-Code](https://github.com/RooCodeInc/Roo-Code) - đội ngũ AI agent lập trình đa vai trò ngay trong editor
- <img src="https://img.shields.io/github/stars/charmbracelet/crush?style=social" height="17" align="texttop"/> [crush](https://github.com/charmbracelet/crush) - coding agent giao diện đẹp mắt ngay trên terminal
- <img src="https://img.shields.io/github/stars/Kilo-Org/kilocode?style=social" height="17" align="texttop"/> [kilocode](https://github.com/Kilo-Org/kilocode) - trợ lý AI mã nguồn mở hỗ trợ lập kế hoạch, xây dựng và sửa lỗi code
- <img src="https://img.shields.io/github/stars/humanlayer/humanlayer?style=social" height="17" align="texttop"/> [humanlayer](https://github.com/humanlayer/humanlayer) - công cụ giúp coding agent giải quyết bài toán khó trong codebase lớn với sự giám sát của con người
- <img src="https://img.shields.io/github/stars/carlrobertoh/ProxyAI?style=social" height="17" align="texttop"/> [ProxyAI](https://github.com/carlrobertoh/ProxyAI) - plugin AI copilot mã nguồn mở hàng đầu cho hệ sinh thái JetBrains

[Quay lại Mục lục](#mục-lục)

### Computer Use (Điều khiển máy tính)

- <img src="https://img.shields.io/github/stars/OpenInterpreter/open-interpreter?style=social" height="17" align="texttop"/> [open-interpreter](https://github.com/OpenInterpreter/open-interpreter) - giao diện ngôn ngữ tự nhiên giúp LLM thực thi mã trực tiếp trên máy tính
- <img src="https://img.shields.io/github/stars/microsoft/OmniParser?style=social" height="17" align="texttop"/> [OmniParser](https://github.com/microsoft/OmniParser) - công cụ phân tích màn hình hỗ trợ GUI agent thuần thị giác
- <img src="https://img.shields.io/github/stars/trycua/cua?style=social" height="17" align="texttop"/> [cua](https://github.com/trycua/cua) - môi trường Docker sandbox cho AI Agent điều khiển máy tính
- <img src="https://img.shields.io/github/stars/OthersideAI/self-operating-computer?style=social" height="17" align="texttop"/> [self-operating-computer](https://github.com/OthersideAI/self-operating-computer) - framework cho phép mô hình đa phương thức tự thao tác chuột/bàn phím trên máy tính
- <img src="https://img.shields.io/github/stars/simular-ai/Agent-S?style=social" height="17" align="texttop"/> [Agent-S](https://github.com/simular-ai/Agent-S) - framework agent mở điều khiển máy tính theo cách của con người

[Quay lại Mục lục](#mục-lục)

### Tự động hóa trình duyệt

- <img src="https://img.shields.io/github/stars/puppeteer/puppeteer?style=social" height="17" align="texttop"/> [puppeteer](https://github.com/puppeteer/puppeteer) - thư viện JavaScript tự động hóa Chrome và Firefox
- <img src="https://img.shields.io/github/stars/microsoft/playwright?style=social" height="17" align="texttop"/> [playwright](https://github.com/microsoft/playwright) - framework kiểm thử và tự động hóa trình duyệt đa nền tảng của Microsoft
- <img src="https://img.shields.io/github/stars/browser-use/browser-use?style=social" height="17" align="texttop"/> [browser-use](https://github.com/browser-use/browser-use) - kết nối trình duyệt để AI agent tương tác tự động với website
- <img src="https://img.shields.io/github/stars/mendableai/firecrawl?style=social" height="17" align="texttop"/> [firecrawl](https://github.com/mendableai/firecrawl) - chuyển đổi toàn bộ website thành Markdown hoặc dữ liệu có cấu trúc cho LLM
- <img src="https://img.shields.io/github/stars/browserbase/stagehand?style=social" height="17" align="texttop"/> [stagehand](https://github.com/browserbase/stagehand) - framework tự động hóa trình duyệt kết hợp AI và mã Playwright
- <img src="https://img.shields.io/github/stars/nanobrowser/nanobrowser?style=social" height="17" align="texttop"/> [nanobrowser](https://github.com/nanobrowser/nanobrowser) - tiện ích Chrome mã nguồn mở hỗ trợ tự động hóa web bằng AI

[Quay lại Mục lục](#mục-lục)

### Quản lý bộ nhớ (Memory Management)

- <img src="https://img.shields.io/github/stars/mem0ai/mem0?style=social" height="17" align="texttop"/> [mem0](https://github.com/mem0ai/mem0) - lớp bộ nhớ dài hạn phổ quát cho AI Agents
- <img src="https://img.shields.io/github/stars/letta-ai/letta?style=social" height="17" align="texttop"/> [letta](https://github.com/letta-ai/letta) - framework agent có trạng thái (stateful) với cơ chế quản lý bộ nhớ và ngữ cảnh
- <img src="https://img.shields.io/github/stars/supermemoryai/supermemory?style=social" height="17" align="texttop"/> [supermemory](https://github.com/supermemoryai/supermemory) - hệ thống lưu trữ và truy hồi bộ nhớ tốc độ cao
- <img src="https://img.shields.io/github/stars/topoteretes/cognee?style=social" height="17" align="texttop"/> [cognee](https://github.com/topoteretes/cognee) - tạo bộ nhớ đồ thị cho AI Agents chỉ với vài dòng code
- <img src="https://img.shields.io/github/stars/LMCache/LMCache?style=social" height="17" align="texttop"/> [LMCache](https://github.com/LMCache/LMCache) - tăng tốc suy luận LLM thông qua lớp lưu trữ KV Cache tốc độ cao
- <img src="https://img.shields.io/github/stars/NevaMind-AI/memU?style=social" height="17" align="texttop"/> [memU](https://github.com/NevaMind-AI/memU) - framework bộ nhớ mã nguồn mở cho AI đồng hành
- <img src="https://img.shields.io/github/stars/vectorize-io/hindsight?style=social" height="17" align="texttop"/> [Hindsight](https://github.com/vectorize-io/hindsight) - hệ thống bộ nhớ dài hạn tự host hoàn toàn mã nguồn mở cho AI agents

[Quay lại Mục lục](#mục-lục)

### Kiểm thử, Đánh giá & Giám sát

- <img src="https://img.shields.io/github/stars/langfuse/langfuse?style=social" height="17" align="texttop"/> [langfuse](https://github.com/langfuse/langfuse) - nền tảng LLMOps mã nguồn mở: theo dõi trace, đánh giá, quản lý prompt và tích hợp OpenTelemetry
- <img src="https://img.shields.io/github/stars/comet-ml/opik?style=social" height="17" align="texttop"/> [opik](https://github.com/comet-ml/opik) - gỡ lỗi, đánh giá và giám sát ứng dụng LLM, RAG và agentic workflows
- <img src="https://img.shields.io/github/stars/traceloop/openllmetry?style=social" height="17" align="texttop"/> [openllmetry](https://github.com/traceloop/openllmetry) - bộ công cụ giám sát (observability) cho LLM xây dựng trên chuẩn OpenTelemetry
- <img src="https://img.shields.io/github/stars/NVIDIA/garak?style=social" height="17" align="texttop"/> [garak](https://github.com/NVIDIA/garak) - công cụ quét lỗ hổng bảo mật và jailbreak cho LLM từ NVIDIA
- <img src="https://img.shields.io/github/stars/Giskard-AI/giskard?style=social" height="17" align="texttop"/> [giskard](https://github.com/Giskard-AI/giskard) - công cụ đánh giá và kiểm thử chất lượng hệ thống AI/LLM mã nguồn mở
- <img src="https://img.shields.io/github/stars/Agenta-AI/agenta?style=social" height="17" align="texttop"/> [agenta](https://github.com/Agenta-AI/agenta) - nền tảng LLMOps quản lý prompt, đánh giá và giám sát tất cả trong một

[Quay lại Mục lục](#mục-lục)

### Nghiên cứu chuyên sâu (Research)

- <img src="https://img.shields.io/github/stars/ItzCrazyKns/Perplexica?style=social" height="17" align="texttop"/> [Perplexica](https://github.com/ItzCrazyKns/Perplexica) - công cụ tìm kiếm AI mã nguồn mở thay thế Perplexity AI chạy được với LLM cục bộ
- <img src="https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social" height="17" align="texttop"/> [gpt-researcher](https://github.com/assafelovic/gpt-researcher) - agent tự động nghiên cứu tài liệu cục bộ và web để tổng hợp báo cáo có trích dẫn
- <img src="https://img.shields.io/github/stars/MODSetter/SurfSense?style=social" height="17" align="texttop"/> [SurfSense](https://github.com/MODSetter/SurfSense) - giải pháp thay thế NotebookLM và Perplexity mã nguồn mở
- <img src="https://img.shields.io/github/stars/lfnovo/open-notebook?style=social" height="17" align="texttop"/> [open-notebook](https://github.com/lfnovo/open-notebook) - bản triển khai mã nguồn mở của NotebookLM hỗ trợ nhiều nhà cung cấp mô hình cục bộ
- <img src="https://img.shields.io/github/stars/microsoft/RD-Agent?style=social" height="17" align="texttop"/> [RD-Agent](https://github.com/microsoft/RD-Agent) - tự động hóa quy trình nghiên cứu và phát triển (R&D) bằng AI agent
- <img src="https://img.shields.io/github/stars/langchain-ai/local-deep-researcher?style=social" height="17" align="texttop"/> [local-deep-researcher](https://github.com/langchain-ai/local-deep-researcher) - trợ lý nghiên cứu web và viết báo cáo chạy hoàn toàn cục bộ
- <img src="https://img.shields.io/github/stars/LearningCircuit/local-deep-research?style=social" height="17" align="texttop"/> [local-deep-research](https://github.com/LearningCircuit/local-deep-research) - trợ lý nghiên cứu AI lặp sâu hỗ trợ mô hình cục bộ
- <img src="https://img.shields.io/github/stars/murtaza-nasir/maestro?style=social" height="17" align="texttop"/> [maestro](https://github.com/murtaza-nasir/maestro) - ứng dụng hỗ trợ nghiên cứu và tổng hợp tác vụ phức tạp

[Quay lại Mục lục](#mục-lục)

### Huấn luyện & Fine-tuning

- <img src="https://img.shields.io/github/stars/OpenRLHF/OpenRLHF?style=social" height="17" align="texttop"/> [OpenRLHF](https://github.com/OpenRLHF/OpenRLHF) - framework huấn luyện RLHF hiệu năng cao xây dựng trên Ray, vLLM, ZeRO-3 và HuggingFace
- <img src="https://img.shields.io/github/stars/kiln-ai/kiln?style=social" height="17" align="texttop"/> [Kiln](https://github.com/kiln-ai/kiln) - công cụ trực quan giúp fine-tune LLM, tạo dữ liệu tổng hợp và cộng tác bộ dữ liệu
- <img src="https://img.shields.io/github/stars/e-p-armstrong/augmentoolkit?style=social" height="17" align="texttop"/> [augmentoolkit](https://github.com/e-p-armstrong/augmentoolkit) - tạo dữ liệu huấn luyện để fine-tune LLM mã nguồn mở trên tri thức mới

[Quay lại Mục lục](#mục-lục)

### Công cụ khác

- <img src="https://img.shields.io/github/stars/upstash/context7?style=social" height="17" align="texttop"/> [context7](https://github.com/upstash/context7) - cung cấp tài liệu thư viện code cập nhật mới nhất cho LLM và AI editor
- <img src="https://img.shields.io/github/stars/aliasrobotics/cai?style=social" height="17" align="texttop"/> [cai](https://github.com/aliasrobotics/cai) - Cybersecurity AI (CAI), framework AI cho lĩnh vực an toàn thông tin
- <img src="https://img.shields.io/github/stars/murtaza-nasir/speakr?style=social" height="17" align="texttop"/> [speakr](https://github.com/murtaza-nasir/speakr) - ứng dụng web tự host để gỡ băng ghi âm cục bộ
- <img src="https://img.shields.io/github/stars/presenton/presenton?style=social" height="17" align="texttop"/> [presenton](https://github.com/presenton/presenton) - công cụ tạo slide thuyết trình AI và API mã nguồn mở
- <img src="https://img.shields.io/github/stars/VectorSpaceLab/OmniGen2?style=social" height="17" align="texttop"/> [OmniGen2](https://github.com/VectorSpaceLab/OmniGen2) - mô hình khám phá khả năng tạo sinh đa phương thức nâng cao
- <img src="https://img.shields.io/github/stars/TheAhmadOsman/4o-ghibli-at-home?style=social" height="17" align="texttop"/> [4o-ghibli-at-home](https://github.com/TheAhmadOsman/4o-ghibli-at-home) - công cụ chuyển phong cách ảnh tự host ưu tiên hiệu năng và quyền riêng tư
- <img src="https://img.shields.io/github/stars/Roy3838/Observer?style=social" height="17" align="texttop"/> [Observer](https://github.com/Roy3838/Observer) - micro-agent cục bộ quan sát, ghi nhật ký và phản hồi bảo mật dữ liệu
- <img src="https://img.shields.io/github/stars/minitap-ai/mobile-use?style=social" height="17" align="texttop"/> [mobile-use](https://github.com/minitap-ai/mobile-use) - AI agent mã nguồn mở điều khiển thiết bị Android hoặc iOS bằng ngôn ngữ tự nhiên
- <img src="https://img.shields.io/github/stars/gabber-dev/gabber?style=social" height="17" align="texttop"/> [gabber](https://github.com/gabber-dev/gabber) - xây dựng ứng dụng AI đa phương thức nhìn, nghe và nói theo thời gian thực
- <img src="https://img.shields.io/github/stars/sevenreasons/promptcat?style=social" height="17" align="texttop"/> [promptcat](https://github.com/sevenreasons/promptcat) - trình quản lý thư viện prompt không phụ thuộc ngoài gói gọn trong một tệp HTML

[Quay lại Mục lục](#mục-lục)

## Phần cứng (Hardware)

- <img src="https://img.shields.io/youtube/channel/subscribers/UCajiMK_CY9icRhLepS8_3ug?style=social" height="17" align="texttop"/> [Alex Ziskind](https://www.youtube.com/@AZisk) - kênh đánh giá PC, laptop, Mac và GPU chạy LLM cục bộ
- <img src="https://img.shields.io/youtube/channel/subscribers/UCiaQzXI5528Il6r2NNkrkJA?style=social" height="17" align="texttop"/> [Digital Spaceport](https://www.youtube.com/@DigitalSpaceport) - đánh giá các cấu hình phần cứng chuyên dụng cho suy luận LLM
- <img src="https://img.shields.io/youtube/channel/subscribers/UCQs0lwV6E4p7LQaGJ6fgy5Q?style=social" height="17" align="texttop"/> [JetsonHacks](https://www.youtube.com/@JetsonHacks) - hướng dẫn phát triển AI trên bộ kit NVIDIA Jetson
- <img src="https://img.shields.io/youtube/channel/subscribers/UC8h2Sf-yyo1WXeEUr-OHgyg?style=social" height="17" align="texttop"/> [Miyconst](https://www.youtube.com/@Miyconst) - thử nghiệm hiệu năng phần cứng và GPU đa dạng cho LLM
- [LLM Inference VRAM & GPU Requirement Calculator](https://app.linpp2009.com/en/llm-gpu-memory-calculator) - công cụ tính lượng VRAM và số GPU cần thiết để triển khai LLM
- <img src="https://img.shields.io/github/stars/vosen/ZLUDA?style=social" height="17" align="texttop"/> [ZLUDA](https://github.com/vosen/ZLUDA) - chạy ứng dụng CUDA trên các GPU không phải của NVIDIA

[Quay lại Mục lục](#mục-lục)

## Tài liệu & Hướng dẫn (Tutorials)

### Kiến thức Mô hình

- <img src="https://img.shields.io/youtube/views/l8pRSuU81PU?style=social" height="17" align="texttop"/> [Let's reproduce GPT-2 (124M)](https://www.youtube.com/watch?v=l8pRSuU81PU)
- <img src="https://img.shields.io/github/stars/karpathy/nanochat?style=social" height="17" align="texttop"/> [nanochat](https://github.com/karpathy/nanochat) - codebase tối giản của Andrej Karpathy cài đặt toàn bộ pipeline huấn luyện LLM giống ChatGPT
- <img src="https://img.shields.io/youtube/views/jrJKRYAdh7I?style=social" height="17" align="texttop"/> [Knowledge Distillation: How LLMs train each other](https://www.youtube.com/watch?v=jrJKRYAdh7I)
- <img src="https://img.shields.io/github/stars/iuliaturc/gguf-docs?style=social" height="17" align="texttop"/> [gguf-docs](https://github.com/iuliaturc/gguf-docs) - tài liệu giải thích chi tiết định dạng lượng tử hóa GGUF

[Quay lại Mục lục](#mục-lục)

### Prompt Engineering

- <img src="https://img.shields.io/github/stars/dair-ai/Prompt-Engineering-Guide?style=social" height="17" align="texttop"/> [Prompt Engineering Guide](https://github.com/dair-ai/Prompt-Engineering-Guide) - cẩm nang, bài báo và notebook hướng dẫn kỹ thuật viết prompt
- <img src="https://img.shields.io/github/stars/NirDiamant/Prompt_Engineering?style=social" height="17" align="texttop"/> [Prompt Engineering by NirDiamant](https://github.com/NirDiamant/Prompt_Engineering) - bộ sưu tập hướng dẫn và cài đặt thực tế các kỹ thuật Prompt Engineering từ cơ bản đến nâng cao
- <img src="https://img.shields.io/badge/Google-%234285F4?logo=google&logoColor=red" height="17" align="texttop"/> [Prompt Engineering by Google](https://drive.google.com/file/d/1AbaBYbEa_EbPelsT40-vj64L-2IwUJHy/view) - tài liệu kỹ thuật viết prompt chính thức của Google
- <img src="https://img.shields.io/badge/Anthropic-%23191919?logo=anthropic" height="17" align="texttop"/> [Prompt Engineering by Anthropic](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview) - hướng dẫn thiết kế prompt của Anthropic
- <img src="https://img.shields.io/badge/Anthropic-%23191919?logo=anthropic" height="17" align="texttop"/> [Prompt Engineering Interactive Tutorial](https://github.com/anthropics/courses/blob/master/prompt_engineering_interactive_tutorial/README.md) - khóa học tương tác về Prompt Engineering của Anthropic
- <img src="https://img.shields.io/badge/Anthropic-%23191919?logo=anthropic" height="17" align="texttop"/> [Real world prompting](https://github.com/anthropics/courses/blob/master/real_world_prompting/README.md) - hướng dẫn áp dụng prompt trong bài toán thực tế
- <img src="https://img.shields.io/badge/Anthropic-%23191919?logo=anthropic" height="17" align="texttop"/> [Prompt evaluations](https://github.com/anthropics/courses/blob/master/prompt_evaluations/README.md) - khóa học đánh giá chất lượng prompt của Anthropic
- <img src="https://img.shields.io/github/stars/x1xhlol/system-prompts-and-models-of-ai-tools?style=social" height="17" align="texttop"/> [system-prompts-and-models-of-ai-tools](https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools) - tổng hợp system prompt tham khảo từ các công cụ AI phổ biến
- <img src="https://img.shields.io/github/stars/asgeirtj/system_prompts_leaks?style=social" height="17" align="texttop"/> [system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) - tổng hợp system prompt tham khảo của ChatGPT, Claude & Gemini
- <img src="https://img.shields.io/badge/OpenAI-%23412991?logo=openai" height="17" align="texttop"/> <img src="https://img.shields.io/github/stars/openai/codex?style=social" height="17" align="texttop"/> [OpenAI Codex](https://github.com/openai/codex) - coding agent gọn nhẹ của OpenAI và cấu trúc system prompt

[Quay lại Mục lục](#mục-lục)

### Context Engineering

- <img src="https://img.shields.io/github/stars/davidkimai/Context-Engineering?style=social" height="17" align="texttop"/> [Context-Engineering](https://github.com/davidkimai/Context-Engineering) - cẩm nang chuyên sâu về thiết kế, điều phối và tối ưu ngữ cảnh (Context Engineering)
- <img src="https://img.shields.io/github/stars/Meirtz/Awesome-Context-Engineering?style=social" height="17" align="texttop"/> [Awesome-Context-Engineering](https://github.com/Meirtz/Awesome-Context-Engineering) - tổng quan toàn diện về Context Engineering từ prompt tới hệ thống AI production

[Quay lại Mục lục](#mục-lục)

### Triển khai Inference

- <img src="https://img.shields.io/github/stars/vllm-project/production-stack?style=social" height="17" align="texttop"/> [vLLM Production Stack](https://github.com/vllm-project/production-stack) - kiến trúc tham chiếu của vLLM để triển khai trên cụm Kubernetes

[Quay lại Mục lục](#mục-lục)

### Xây dựng AI Agents

- <img src="https://img.shields.io/github/stars/NirDiamant/GenAI_Agents?style=social" height="17" align="texttop"/> [GenAI Agents](https://github.com/NirDiamant/GenAI_Agents) - hướng dẫn và mã nguồn cài đặt các kỹ thuật AI Agent đa dạng
- <img src="https://img.shields.io/github/stars/ashishpatel26/500-AI-Agents-Projects?style=social" height="17" align="texttop"/> [500+ AI Agent Projects](https://github.com/ashishpatel26/500-AI-Agents-Projects) - bộ sưu tập 500+ tình huống ứng dụng AI agent theo ngành nghề
- <img src="https://img.shields.io/github/stars/humanlayer/12-factor-agents?style=social" height="17" align="texttop"/> [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) - 12 nguyên tắc xây dựng ứng dụng LLM Agent đáng tin cậy
- <img src="https://img.shields.io/github/stars/NirDiamant/agents-towards-production?style=social" height="17" align="texttop"/> [Agents towards production](https://github.com/NirDiamant/agents-towards-production) - hướng dẫn từ ý tưởng tới vận hành AI agent ở quy mô production
- <img src="https://img.shields.io/github/stars/oxbshw/LLM-Agents-Ecosystem-Handbook?style=social" height="17" align="texttop"/> [LLM Agents & Ecosystem Handbook](https://github.com/oxbshw/LLM-Agents-Ecosystem-Handbook) - cẩm nang toàn diện xây dựng, triển khai và đánh giá hệ sinh thái LLM agent
- <img src="https://img.shields.io/badge/Google-%234285F4?logo=google&logoColor=red" height="17" align="texttop"/> [601 real-world gen AI use cases](https://cloud.google.com/transform/101-real-world-generative-ai-use-cases-from-industry-leaders) - 601 bài toán ứng dụng GenAI thực tế từ các doanh nghiệp hàng đầu (Google Cloud)
- <img src="https://img.shields.io/badge/OpenAI-%23412991?logo=openai" height="17" align="texttop"/> [A practical guide to building agents](https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf) - tài liệu hướng dẫn thực hành xây dựng AI agent từ OpenAI

[Quay lại Mục lục](#mục-lục)

### Kỹ thuật RAG

- <img src="https://img.shields.io/github/stars/pathwaycom/llm-app?style=social" height="17" align="texttop"/> [Pathway AI Pipelines](https://github.com/pathwaycom/llm-app) - các mẫu pipeline RAG và tìm kiếm dữ liệu thời gian thực sẵn sàng chạy
- <img src="https://img.shields.io/github/stars/NirDiamant/RAG_Techniques?style=social" height="17" align="texttop"/> [RAG Techniques](https://github.com/NirDiamant/RAG_Techniques) - tổng hợp các kỹ thuật nâng cao cho hệ thống Retrieval-Augmented Generation (RAG)
- <img src="https://img.shields.io/github/stars/NirDiamant/Controllable-RAG-Agent?style=social" height="17" align="texttop"/> [Controllable RAG Agent](https://github.com/NirDiamant/Controllable-RAG-Agent) - giải pháp RAG dùng thuật toán đồ thị xử lý câu hỏi phức tạp
- <img src="https://img.shields.io/github/stars/lokeswaran-aj/langchain-rag-cookbook?style=social" height="17" align="texttop"/> [LangChain RAG Cookbook](https://github.com/lokeswaran-aj/langchain-rag-cookbook) - bộ công thức mô-đun cài đặt kỹ thuật RAG với LangChain và Python

[Quay lại Mục lục](#mục-lục)

### Hướng dẫn khác

- [Self-hosted AI coding that just works](https://www.reddit.com/r/LocalLLaMA/comments/1lt4y1z/selfhosted_ai_coding_that_just_works/)

[Quay lại Mục lục](#mục-lục)

## Credits & References (Nguồn tham khảo & Bản quyền)

- **Kho gốc (Original Repository)**: [0xSojalSec/LLMs-local](https://github.com/0xSojalSec/LLMs-local)
- **Tác giả gốc (Original Author)**: [@0xSojalSec](https://github.com/0xSojalSec)
- **Cập nhật & Việt hóa**: Sắp xếp lại mục lục, loại bỏ liên kết hỏng, cập nhật liên kết OpenAI Codex, bổ sung 5 công cụ mới (GPT4All, llamafile, TabbyAPI, RamaLama, Cherry Studio) và biên dịch phiên bản tiếng Việt ([README.md](README.md)).
- **Giấy phép (License)**: Kho gốc không đính kèm tệp `LICENSE`; toàn bộ nguồn tham khảo và tác giả gốc được giữ nguyên ghi nhận tại đây.
