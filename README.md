<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://bulutbilisimciler.com/">
    <img src="md_images/bb.png" alt="Logo" width="200">
  </a>

  <h3 align="center">Bulut Bilişimciler</h3>

  <p align="center">
    Tarayıcınızda gerçek ortamları kullanarak bulut teknolojilerini öğrenin.
    <br />
    <a href="https://github.com/YunusEmreAlps/bb-scenario-template/archive/refs/heads/master.zip">Download</a>
    ·
    <a href="https://github.com/YunusEmreAlps/bb-scenario-template/issues">Report Bug</a>
    ·
    <a href="https://github.com/YunusEmreAlps/bb-scenario-template/issues">Request Feature</a>
  </p>
</p>

## Bulut Bilişimciler Senaryo Şablonu

İfadeyi, öğrenmeyi ve uygulamayı ilerleten türden yaratıcı keşiflere ilham vermek ve bunları çoğaltmak istiyoruz. Bulut Bilişimciler, yaratıcı ve meraklı insanlar için frontend, backend, bulut teknolojileri ve daha fazlasını içeren senaryolarla kavramları ve araçları kendiniz test ederek öğrenebileceğiniz interaktif bir çevrimiçi öğrenme topluluğudur.

---

Bu kaynak, "Bulut Bilişimciler" platformu için örnek senaryo şablonunu barındıran ve senaryo bilgilerini içeren depodur. **Yazacağınız senaryolar için bu şablonu kullanabilirsiniz**

Örnek Senaryolara bu URL üzerinden ulaşabilirsiniz:
<https://github.com/katacoda/scenario-examples>

---

### Senaryo Oluşturma Adımları

- Adım 1 - Senaryo yazacağımız teknolojinin adı ile bir dosya oluşturuyoruz. (Örn: Git, Go veya Linux gibi...)
- Adım 2 - 1. Adımı tamamladıktan sonra konu başlıklarına göre dosyalar oluşturuyoruz. (bash-basics-1, basics-1, gibi bir isim verebilirsiniz.)
- Adım 3 - Bu dosyanın içerisinde

  - en_finish.md
  - en_intro.md
  - en_step1.md
  - index.json
  - tr_finish.md
  - tr_intro.md
  - tr_step1.md dosyaları kesinlikle olmalıdır.
  
**Adım sayısına göre en_step1.md ve tr_step1.md dosyaları en_stepx.md ve tr_stepx.md şeklinde arttırabilirsiniz.**

Platformu evrensel yapmayı düşünüyoruz. Bu yüzden senaryoların iki dilde olması daha geniş bir kitleye hitap etmemizi sağlayacak.

tr ile başlayan markdown (.md) dosyaları Türkçe, en ile başlayan markdown (.md) dosyaları ise İngilizce olmalıdır.

![Scenario Files](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/scenario_files.png?raw=true)

- Adım 4 - Bu dosyaları oluşturduktan sonra index.json dosyasına bu adımları, video varsa linkini vs. vermeniz aşağıdaki gibi girmemiz gerekiyor.

```sh
{
    "scenario": {
      "steps": [
        {
          "text": "step1.md" // Adım 1
        }
        {
          "text": "step2.md" // Adım 2
        }
        {
          "text": "step3.md" // Adım 3
        }
      ],
      "intro": {
        "text": "intro.md" // Başlangıç
      },
      "finish": {
        "text": "finish.md" // Bitiş
      },
      "video": {
        "text": {
          "en": "https://youtube.com/embed/zRiZZwGSl0M", // İngilizce Video
          "tr": "https://youtube.com/embed/zRiZZwGSl0M"  // Türkçe Video
        }
      }
    },
    "environment": {
      "uilayout": "editor-terminal"
    },
    "backend": {
      "imageid": "alpine" // Kullanılacak Image Adı
    }
  }
```

![Index.json](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/index.json.png?raw=true)


---

#### Dosyaların Platformda Görünümü

- Adım 1: Eğitimler
![Scenarios](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/lesson.png?raw=true)
- Adım 2: Senaryoların Gösterilmesi
![Scenarios](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/scenario_tab.png?raw=true)
- Adım 3: Senaryo'nun Çalıştırılması
![Specific Scenario](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/scenario_tab.png?raw=true)
- Adım 4: Senaryo Başlangıç (tr_intro.md)
![tr_intro.md](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/tr_intro.md.png?raw=true)
- Adım 5: Senaryo Adımları (tr_step1.md)
![tr_step1.md](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/tr_step1_top.png?raw=true)

![tr_step1.md](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/tr_step1_bottom.png?raw=true)

- Adım 6: Senarya Bitirme Kısmı (tr_finish.md)
![tr_finish.md](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/tr_finish.md.png?raw=true)
