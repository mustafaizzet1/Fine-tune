# 🧠 Fine-tune: Hukuk Verileri Üzerine LLaMA Tabanlı Model Eğitimi

Bu proje, **Trendyol-LLM-7B-chat-v4.1.0** ve benzeri LLaMA tabanlı büyük dil modellerini Türkiye'deki **hukuk verileri** üzerine fine-tune etmeye odaklanır. Model eğitimi, [Unsloth](https://github.com/unslothai/unsloth) kütüphanesi kullanılarak 4-bit quantization, PEFT (LoRA) ve Alpaca-style prompt formatlarıyla gerçekleştirilmiştir.

---

## 🚀 Özellikler

- ⚖️ Türkiye'deki hukuki diyaloglarla eğitilmiş özel veri seti  
- 🦙 LLaMA-3 uyumlu 4-bit düşük bellekli model eğitimi  
- 🧩 **Unsloth** ile optimize edilmiş düşük VRAM kullanımı  
- 💬 Alpaca tarzı etkileşimli prompt yapısı  
- 🔁 PEFT (LoRA) ile hızlı, düşük kaynaklı fine-tuning  
- 🖥️ **T4 GPU** üzerinde bile sorunsuz çalışır — yüksek veri boyutlarına gerek olmadan büyük modelleri eğitebilir

---

## 🔧 Kurulum

```bash
pip install unsloth
pip install datasets trl bitsandbytes peft accelerate



📁 Veri Formatı
Eğitim verisi .jsonl formatında olup her satır şu yapıya sahiptir:

json
{
  "messages": [
    {"role": "system", "content": "Sistem mesajı"},
    {"role": "user", "content": "Kullanıcı mesajı"},
    {"role": "assistant", "content": "Model cevabı"}
  ]
}
