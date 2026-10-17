# Signal Analysis: Fourier Transform, Modulation and Convolution (Python)

Üçgen darbe işareti `x(t) = Λ(t)` üzerinde zaman ve frekans düzlemi analizi.
Sinyaller ve Sistemler dersi kapsamında hazırlanmıştır.

## İçerik

| Şık | Konu |
|-----|------|
| a | `x(t) = tri(t)` zaman grafiği |
| b | `X(f) = sinc²(f)` genlik ve faz spektrumu |
| c | Zaman kaydırma: `y(t) = x(t-5)` → faz `-10πf` |
| d | Modülasyon: `y(t) = x(t)cos(2πf₀t)`, `f₀ = 927 kHz` |
| e | Zaman ölçekleme: `y(t) = (1/3)x(t/3)` → `sinc²(3f)` |
| f | `h(t) = rect(t)` dürtü cevabı, frekans cevabı ve elle yazılmış konvolüsyon |

## Nasıl Çalıştırılır?

```bash
pip install numpy matplotlib jupyter
jupyter notebook fourier_analysis.ipynb
```

## Kullanılan Kavramlar

- Fourier dönüşümü özellikleri (kaydırma, ölçekleme, modülasyon)
- Genlik ve faz spektrumu
- Doğrusal zamanla değişmeyen (LTI) sistemler ve konvolüsyon
- NumPy ile vektörel hesap, Matplotlib ile görselleştirme

## Bilinen Eksikler

- Modülasyon şıkkının geniş frekans görünümünde dar ana loblar örnekleme nedeniyle zor seçilir; yakınlaştırılmış grafikler esas alınmalıdır.
- Konvolüsyon çift döngüyle yazıldı, büyük diziler için `np.convolve` daha hızlıdır.

## Hakkında

Bu proje Gebze Teknik Üniversitesi ELM264 dersi kapsamında geliştirilmiştir.
