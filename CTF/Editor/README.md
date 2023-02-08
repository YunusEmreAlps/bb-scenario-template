<!-- PROJECT LOGO -->
# CTF Oluşturma Adımları

**1. Adım** —— CTF yazacağımız teknolojinin adı ile bir dosya oluşturuyoruz. (Örn: Nginx-Resolver, Bandit, vs)

![Create Base File](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/create_base_file.png?raw=true)

Bu dosyaları, kök dizin olarak düşünebiliriz.

**template adlı dosyayı yazacağınız CTF'e göre düzenleyebilirsiniz**

---

**2. Adım** —— 1. Adımı tamamladıktan sonra "ctf-" ön eki ile konu başlıklarına veya seviyelerine göre yeni dosyalar oluşturuyoruz. (ctf-nginx-resolver, ctf-level-1, ctf-level-2, gibi bir isim verebilirsiniz.). Bu dosyaları ise ağacın dalları gibi düşünebiliriz.

![Create Base File](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/create_scenario_file.png?raw=true)

**template adlı dosyanın içerisinde yer alan ctf-template-X dosyasının adını isteğe bağlı olarak değiştirebilirsiniz. Burada dikkat edilmesi gereken en önemli detay küçük karakter kullanılmalı ve boşluk yerine "-" işareti kullanılmalıdır**

---

**3. Adım** —— Oluşturduğumuz her konu başlık dosyasının içerisinde aşağıda belirtilen dosyaları oluşturuyoruz.

- en_finish.md
- en_intro.md
- en_step1.md
- index.json
- tr_finish.md
- tr_intro.md
- tr_step1.md

<pre>
  CTF Adı (Örn: Nginx-Resolver, Bandit, vs)
    |__Seviye 1
       |__en_finish.md
       |__en_intro.md
       |__en_step1.md
       |__index.json
       |__tr_finish.md
       |__tr_intro.md
       |__tr_step1.md
    |__Seviye 2
       |__en_finish.md
       |__en_intro.md
       |__en_step1.md
       |__index.json
       |__tr_finish.md
       |__tr_intro.md
       |__tr_step1.md
    |__Seviye 3
       |__en_finish.md
       |__en_intro.md
       |__en_step1.md
       |__index.json
       |__tr_finish.md
       |__tr_intro.md
       |__tr_step1.md
    |__Seviye 4
       |__en_finish.md
       |__en_intro.md
       |__en_step1.md
       |__index.json
       |__tr_finish.md
       |__tr_intro.md
       |__tr_step1.md
</pre>

***CTF Senaryolarını tek adımda bitirebilirsiniz ama bu çözümünü uzun ve karmaşık bir hale getirecektir. Bu yüzden adımlara ayırmanız çözüm sürecini daha kolay ve akıcı bir hale getirecektir. Adım sayısına göre en_step1.md ve tr_step1.md dosyalarını en_stepx.md ve tr_stepx.md şeklinde arttırabilirsiniz.***

***Dünya'nın her yerinde ulaşılabilir olmak istiyoruz. Bu yüzden yazılan CTF senaryolarını bu aşamada iki dili destekleyecek şekilde istiyoruz. Tr ile başlayan markdown (.md) dosyaları Türkçe, en ile başlayan markdown (.md) dosyaları ise İngilizce olmalıdır.***

![Create MD Files](https://github.com/YunusEmreAlps/bb-scenario-template/blob/master/md_images/md_files.png?raw=true)

---

**4. Adım** —— Son adımda ise oluşturduğumuz dosyaları **index.json** dosyasına tanımlıyoruz. Adımları, kullanılacak image adını ve video linkini aşağıdaki gibi girmemiz gerekiyor.

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
        "text": "intro.md" // CTF içeriği ile ilgili girizgâh yapılan dosya
      },
      "finish": {
        "text": "finish.md" // CTF sonunda yapılması gerekenlerin anlatıldığı dosya
      },
      "video": {
        "text": {
          "en": "", // İngilizce Video
          "tr": ""  // Türkçe Video
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

...
