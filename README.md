# ⚡ 3-Phase Pure Sine Wave Inverter (SPWM) using ATmega328P

This repository contains the hardware design and embedded firmware for a **3-Phase Full-Bridge Inverter**, designed primarily for electric vehicle (EV) power transmission system simulations. The project demonstrates the generation of Sinusoidal Pulse Width Modulation (SPWM) signals using an ATmega328P microcontroller to drive a 3-phase load.

## 🚀 Project Features
* **Microcontroller:** ATmega328P.
* **Power Stage:** 6x IRF540 MOSFETs and 3x IR2110 High/Low Side Gate Drivers.
* **Control Method:** Sinusoidal PWM (SPWM) with precise 120° phase shifts.
* **Switching Frequency:** ~31.25 kHz for smooth sine wave generation and reduced harmonic distortion.
* **Gate Driving:** Implementation of a proper bootstrap circuit for the high-side MOSFETs to ensure stable continuous operation.

## 🛠 Hardware & Circuit Diagram
The circuit is optimized for stable simulation and real-world application, featuring proper grounding for the IR2110 Shutdown (SD) pins and calculated bootstrap capacitors.

![Circuit Diagram](Docs/circuit_diagram.png)
*(Note: If your image format is different, e.g., .jpg, please update the extension in the code)*

## 📊 Simulation & Oscilloscope Outputs
The hardware and software integration was verified using Proteus. The oscilloscope output below confirms the successful generation of three distinct SPWM signals, perfectly interweaved with a 120-degree phase difference.

![Oscilloscope Output](Docs/oscilloscope.png)

## 📂 Repository Structure
* `/Hardware`: Contains the Proteus schematic files (`.dsn`).
* `/Firmware`: Contains the ATmega328P C source code and the compiled `.hex` file.
* `/Docs`: Contains project documentation, circuit diagrams, and waveform screenshots.

---

### 👨‍💻 Author
* **Ahmet**
* Electrical and Electronics Engineering Student

---
---

# ⚡ ATmega328P ile 3-Fazlı Tam Sinüs İnvertör (SPWM)

Bu depo, özellikle elektrikli araç (EV) güç aktarma sistemleri simülasyonları için tasarlanmış bir **3-Fazlı Tam Köprü (Full-Bridge) İnvertör** projesinin donanım tasarımını ve gömülü yazılımını içermektedir. Proje, 3-fazlı bir yükü sürmek için ATmega328P mikrodenetleyicisi kullanılarak Sinüzoidal Darbe Genişlik Modülasyonu (SPWM) sinyallerinin üretilmesini amaçlamaktadır.

## 🚀 Proje Özellikleri
* **Mikrodenetleyici:** ATmega328P.
* **Güç Katı:** 6 adet IRF540 MOSFET ve 3 adet IR2110 High/Low Side Gate Sürücü.
* **Kontrol Metodu:** Tam 120° faz farkıyla üretilen Sinüzoidal PWM (SPWM).
* **Anahtarlama Frekansı:** Pürüzsüz sinüs dalgası ve düşük harmonik bozulma için ~31.25 kHz.
* **Sürücü Tasarımı:** Üst kol MOSFET'lerinin kararlı çalışması için uygun Bootstrap devresi tasarımı.

## 🛠 Donanım ve Devre Şeması
Devre, IR2110 Shutdown (SD) bacaklarının doğru şekilde topraklanması ve hesaplanmış bootstrap kapasitörleri ile kararlı simülasyon ve gerçek dünya uygulamaları için optimize edilmiştir.

![Devre Şeması](Docs/circuit_diagram.png)
*(Not: Fotoğraf formatın .jpg ise koddaki uzantıyı değiştirmeyi unutma)*

## 📊 Simülasyon ve Osiloskop Çıktıları
Donanım ve yazılım entegrasyonu Proteus üzerinde doğrulanmıştır. Aşağıdaki osiloskop çıktısı, aralarında tam 120 derece faz farkı bulunan 3 ayrı SPWM sinyalinin başarılı bir şekilde üretildiğini kanıtlamaktadır.

![Osiloskop Görüntüsü](Docs/oscilloscope.png)

## 📂 Klasör Yapısı
* `/Hardware`: Proteus şema dosyalarını (`.dsn`) içerir.
* `/Firmware`: ATmega328P C kaynak kodunu ve derlenmiş `.hex` dosyasını içerir.
* `/Docs`: Proje dökümanlarını, devre şemalarını ve dalga formu ekran görüntülerini içerir.

---

### 👨‍💻 Geliştirici
* **Ahmet**
* Elektrik Elektronik Mühendisliği Öğrencisi
