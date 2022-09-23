<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://bulutbilisimciler.com/">
    <img src="md_images/bb-slogan.png" alt="Logo" width="200">
  </a>
  <p align="center">
  İfadeyi, öğrenmeyi ve uygulamayı ilerleten türden yaratıcı keşiflere ilham vermek ve bunları çoğaltmak istiyoruz. Bulut Bilişimciler, yaratıcı ve meraklı insanlar için frontend, backend, bulut teknolojileri ve daha fazlasını içeren senaryolarla kavramları ve araçları kendiniz test ederek öğrenebileceğiniz interaktif bir çevrimiçi öğrenme topluluğudur.
  <br/><br/>
    <a href="https://github.com/YunusEmreAlps/bb-scenario-template/archive/refs/heads/master.zip">Download</a>
    ·
    <a href="https://github.com/YunusEmreAlps/bb-scenario-template/issues">Report Bug</a>
    ·
    <a href="https://github.com/YunusEmreAlps/bb-scenario-template/issues">Request Feature</a>
  </p>
</p>

<br/>

## Bulut Bilişimciler Senaryo Şablonu

Bu doküman, "Bulut Bilişimciler" platformu için örnek senaryo şablonunu barındıran ve senaryo bilgilerini içeren bir kaynaktır. **Yazacağınız senaryolar için bu şablonu kullanabilirsiniz**</p>

Örnek Senaryolara bu URL üzerinden ulaşabilirsiniz:
<https://github.com/katacoda/scenario-examples>

---

### Senaryo Oluşturma Adımları

- **Adım 1** - Senaryo yazacağımız teknolojinin adı ile bir dosya oluşturuyoruz. (Örn: Git, Go veya Linux gibi...) Bu dosyayı ağacın kökü gibi düşünebiliriz.

![Create Base File](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/create_base_file.png?raw=true)

---
- **Adım 2** - 1. Adımı tamamladıktan sonra konu başlıklarına göre dosyalar oluşturuyoruz. (bash-basics-1, basics-1, gibi bir isim verebilirsiniz.). Bu dosyayı ise ağacın dalları gibi düşünebiliriz.

![Create Base File](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/create_scenario_file.png?raw=true)


---
- **Adım 3** - Oluşturduğumuz her konu başlık dosyasının içerisinde aşağıda belirtilen .md uzantılı dosyaları oluşturuyoruz.
  - en_finish.md
  - en_intro.md
  - en_step1.md
  - index.json
  - tr_finish.md
  - tr_intro.md
  - tr_step1.md

  
![Create MD Files](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/md_files.png?raw=true)

**Adım sayısına göre en_step1.md ve tr_step1.md dosyaları en_stepx.md ve tr_stepx.md şeklinde arttırabilirsiniz.**

Platformu evrensel yapmayı düşünüyoruz. Bu yüzden senaryoların iki dilde olması daha geniş bir kitleye hitap etmemizi sağlayacak. Bu yüzden **tr ile başlayan markdown (.md) dosyaları Türkçe, en ile başlayan markdown (.md) dosyaları da İngilizce olmalıdır.**

![Scenario Files](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/scenario_files.png?raw=true)

---

- **Adım 4** - Bu dosyaları oluşturduktan sonra **index.json** dosyasına bu adımları, video varsa linkini vs. vermeniz aşağıdaki gibi girmemiz gerekiyor.

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
        "text": "intro.md" // Dersin içeriği ile ilgili girizgâh yapılan dosya
      },
      "finish": {
        "text": "finish.md" // Dersin sonunda elde edilen yetkinliklerin anlatıldığı dosya
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

### Dosyaların Platformda Görünümü

- Adım 1: Eğitimler
![Scenarios](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/lesson.png?raw=true)
- Adım 2: Senaryoların Gösterilmesi
![Scenarios](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/scenario_list.png?raw=true)
- Adım 3: Senaryo'nun Çalıştırılması
![Specific Scenario](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/scenario_tab.png?raw=true)
- Adım 4: Senaryo Başlangıç (tr_intro.md)
![tr_intro.md](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/tr_intro.md.png?raw=true)
- Adım 5: Senaryo Adımları (tr_step1.md)
![tr_step1.md](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/tr_step1_top.png?raw=true)

![tr_step1.md](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/tr_step1_bottom.png?raw=true)

- Adım 6: Senaryo Bitirme Kısmı (tr_finish.md)
![tr_finish.md](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/tr_finish.md.png?raw=true)
