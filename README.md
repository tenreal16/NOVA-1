# NOVA-1 🤖
### Neural On-device Voice Assistant — Concept Blueprint

> *A pocket-sized Jarvis. No cloud. No subscription. Just AI.*

![Status](https://img.shields.io/badge/Status-Concept%20Phase-blue?style=flat-square)
![Made by](https://img.shields.io/badge/Concept%20by-Aniket%20Yadav-cyan?style=flat-square)

---

## 🔷 What is NOVA-1?

NOVA-1 is a **hardware concept** for a fully self-contained AI voice assistant gadget that runs entirely on-device — no internet required for core AI, no subscriptions, no data sent to any cloud.

Think of it as a physical Jarvis that lives in your pocket.

**Form Factor:** 6 × 2 × 2 inches cuboid  
**Inspired by:** Iron Man's J.A.R.V.I.S

---

## 🖥️ Interactive Blueprint

> **[→ View Full Engineering Blueprint](./NOVA-1_Engineering_Spec.html)**  
> Open in browser for the full interactive design schematic, specs, and system architecture.

---

## ✨ Key Features

| Feature | Details |
|---|---|
| 🧠 On-Device AI | Self-hosted 3B–7B LLM — runs fully offline |
| 📡 Connectivity | Built-in WiFi 6E + Nano SIM (4G/5G) for live queries |
| 🖥️ Display | 2×2 inch AMOLED panel |
| 🎧 Slide-Out Earbuds | Magnetic slide mechanism — auto-pairs via Bluetooth 5.3 |
| ⚡ Charging | USB-C 65W PD |
| 🎙️ Audio Jack | 3.5mm analog output |
| 🌊 Waterproof | IP68 rated (1.5m / 30 min) |
| 🎭 Emotion Engine | Detects 7 emotional states — adapts tone & response style |
| 🧬 Adaptive Memory | Learns your habits, preferences, behaviour over time |
| 🗣️ Voice Modules | Jarvis / Female / Custom Cloned / Whisper / Multilingual |
| ⏱️ Response Time | Voice reply in under 5 seconds |

---

## 🔧 System Architecture

```
[Wake Word] → [STT: Whisper] → [Emotion Detection]
                                        ↓
                            [LLM: LLaMA 3.2 / Phi-3]
                                        ↓
                         [Memory Injection: ChromaDB]
                                        ↓
                      [Internet? WiFi/SIM if needed]
                                        ↓
                          [TTS: Kokoro / Voice Module]
                                        ↓
                         [Slide-Out Earbuds / Speaker]
```

Total pipeline latency target: **< 5 seconds**

---

## 🧠 AI Stack (Proposed)

- **LLM:** LLaMA 3.2 3B (INT4 quantized) or Phi-3 Mini
- **STT:** OpenAI Whisper Base (on-device)
- **TTS:** Kokoro / Coqui TTS (selectable voice modules)
- **Memory:** ChromaDB vector database (on-device)
- **Emotion:** Sentiment analysis layer (pre-inference)
- **SoC:** Qualcomm Snapdragon 8 Gen 3 (NPU-accelerated)

---

## 🎭 Emotion Engine

NOVA-1 detects your emotional state from voice tone and adapts its behaviour:

| Emotion | NOVA Response |
|---|---|
| 😤 Stressed | Slower, calmer TTS. Short direct answers. |
| 😄 Excited | Matches energy. Faster pace. |
| 😴 Tired | Whisper mode. Low brightness. Minimal interaction. |
| 🤔 Curious | Pulls from internet. Detailed answers. Shows on display. |
| 😠 Angry | Non-confrontational. Offers help calmly. |
| 😊 Happy | Conversational. Adds light humour. |
| 😐 Neutral | Default Jarvis mode. Efficient and direct. |

---

## 🗣️ Voice Module Selection

- **JARVIS MODE** — Default British AI assistant voice
- **NOVA FEMALE** — Female AI voice
- **CUSTOM CLONED** — Record 30 seconds, NOVA clones your choice
- **WHISPER MODE** — Low energy, quiet environments
- **MULTILINGUAL** — Hindi / English switching

---

## 📦 Hardware Specs (Proposed)

```
Dimensions     : 6.0 × 2.0 × 2.0 inches (152 × 51 × 51 mm)
Display        : 2×2 in AMOLED, 400×400px
SoC            : Qualcomm Snapdragon 8 Gen 3
RAM            : 12GB LPDDR5X
Storage        : 256GB UFS 4.0
Battery        : 4000 mAh (~12h AI use)
Charging       : USB-C 65W Power Delivery
Audio Out      : 3.5mm analog jack
Microphones    : 3× beamforming array
Speaker        : 2W stereo driver
Bluetooth      : BT 5.3 LE Audio (earbuds auto-pair)
WiFi           : 802.11ax WiFi 6E (2.4 / 5 / 6 GHz)
Cellular       : Nano SIM, 4G LTE / 5G
Waterproofing  : IP68 (1.5m / 30min)
Weight         : ~180g (estimated)
```

---

## 🚀 Prototype Roadmap

### Phase 1 — Software (₹0)
- [ ] Run LLaMA 3.2 3B on Android device
- [ ] Integrate Whisper STT locally
- [ ] Build voice pipeline app
- [ ] Emotion detection module
- [ ] ChromaDB memory layer
- [ ] TTS voice module selector

### Phase 2 — Hardware Dev (₹8,000–15,000)
- [ ] 3D print 6×2×2 enclosure
- [ ] Source dev board (RPi CM4 or similar)
- [ ] Wire AMOLED 2×2 display
- [ ] Add mic array + speaker
- [ ] SIM module integration

### Phase 3 — Final Build (₹50,000+)
- [ ] Custom PCB design
- [ ] Slide earbud mechanism (hall sensor + pogo pins)
- [ ] IP68 waterproof sealing
- [ ] Qualcomm SoC integration
- [ ] CNC machined chassis

---

## 💡 Why This?

Current AI assistants all have one problem — **they need your data, your internet, and your subscription.**

NOVA-1 flips that:
- Your AI runs **on the device**
- Your memory stays **on the device**
- Your voice never leaves **the device**
- It learns **you** — not a generic user

---

© 2026 Aniket Yadav — Concept Design

---

## 🤝 Open To

- Collaboration on Phase 1 software
- Hardware engineers interested in the build
- Investors / Accelerators interested in the concept
- Feedback, ideas, improvements

**Contact:** [Open an Issue](../../issues) or reach out directly.

---

> *"Sometimes you gotta run before you can walk."* — Tony Stark
