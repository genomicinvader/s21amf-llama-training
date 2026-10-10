# 🚀 S21AMF Local AI & Hybrid Pipeline Suite

This suite enables you to run AI tasks locally on your PC, saving **100% of Antigravity Cloud tokens** for heavy document parsing, photo generation, and model training.

---

## 📂 Tools Included

### 1. Hybrid Book & Document Parser (`hybrid_book_parser.py`)
Reads any PDF or text book, extracts technical content, and uses your local Ollama model to generate structured modules, lessons, and capstone quiz questions.

**Usage:**
```bash
python hybrid_book_parser.py "path/to/book.pdf" --start 1 --pages 15 --model qwen2.5-coder:7b
```
*Note: You can switch `--model` to `llama3.1:8b` once download finishes.*

---

### 2. Auto-Importer to Live WordPress (`import_to_tutor.py`)
Takes the JSON output from `hybrid_book_parser.py` and imports it directly into your live website (`s21amf.com`) Tutor LMS courses and Content Bank!

**Usage:**
```bash
python import_to_tutor.py "test_output/sample_curriculum.json" 4593
```
*(Replace `4593` with your target Course ID).*

---

### 3. AI Photo Generator (`generate_photo.py`)
Instant, high-definition photorealistic image generator (using state-of-the-art Flux / SDXL architecture). Completely free, unlimited, zero token cost.

**Usage:**
```bash
python generate_photo.py "Modern amateur radio station with glowing antennas at dusk, 8k" --out my_shack.png
```

---

### 4. 1-Click Google Colab Training Notebook (`S21AMF_FineTune_Llama3_Colab.ipynb`)
For fine-tuning custom models on free cloud GPUs (Google Colab T4 16GB) without hardware limits.

**How to use:**
1. Open [Google Colab](https://colab.research.google.com/).
2. Click **File > Upload notebook** and select `S21AMF_FineTune_Llama3_Colab.ipynb`.
3. Go to **Runtime > Change runtime type** and ensure **T4 GPU** is selected.
4. Click **Runtime > Run all** (Ctrl + F9).
5. At the end, the notebook automatically downloads the fine-tuned `.gguf` model for your local Ollama!
