# Fine-tune: Hukuk Verileri Üzerine LLaMA Tabanlı Model Eğitimi

Bu proje, **Trendyol-LLM-7B-chat-v4.1.0** ve benzeri LLaMA tabanlı büyük dil modellerini Türkiye'deki hukuk verileri üzerine fine-tune etmeye odaklanır. Model eğitimi, [Unsloth](https://github.com/unslothai/unsloth) kütüphanesi ile 4-bit quantization, PEFT (LoRA) ve Alpaca-style prompt formatları kullanılarak gerçekleştirilmiştir.

---

## 🚀 Özellikler

- LLaMA-3 destekli 4-bit model eğitimi  
- Türkiye’deki hukuki diyalog verileriyle eğitilmiş  
- Unsloth ile optimize edilmiş düşük VRAM kullanımı  
- Alpaca tarzı formatla doğal etkileşimli cevap üretimi  
- PEFT (LoRA) ile hızlı ve hafif fine-tuning  

---

## 🔧 Kurulum

```bash
pip install unsloth
pip install datasets trl bitsandbytes peft accelerate
