🔄 Stack & Queue Ters Çevirme Simülasyonu

Bu proje, Veri Yapıları (Data Structures) derslerinde sıkça karşılaşılan bir algoritma probleminin interaktif görselleştirmesidir. Bir Yığın (Stack) veri yapısındaki elemanların, bir Kuyruk (Queue) yardımıyla nasıl tersine çevrildiğini (Reverse işlemi) adım adım simüle eder.

🎯 Proje Hakkında

Genellikle sınavlarda veya algoritma analizlerinde sorulan QST (Queue-Stack-Transfer) metodunun çalışma mantığını görselleştirir. Bu algoritma şu iki temel adımdan oluşur:

Stack -> Queue: Stack boşalana kadar elemanlar çıkarılır (pop) ve kuyruğa eklenir (enqueue).

Queue -> Stack: Kuyruk boşalana kadar elemanlar çıkarılır (dequeue) ve tekrar stack'e eklenir (push).

Sonuç olarak, Stack'in orijinal sırası tamamen tersine döner (LIFO mantığı gereği).

🚀 Özellikler

Adım Adım Görselleştirme: Elemanların bir yapıdan diğerine geçişini animasyonla izleyin.

Kod Takibi: Sağ panelde Java kodunun o an hangi satırının çalıştığını canlı olarak takip edin.

Durum Bilgilendirmesi: Her adımda hangi değerin pop, push, enqueue veya dequeue edildiğini görün.

Tek Dosya: Harici bağımlılık gerektirmez, sadece index.html dosyasını tarayıcıda açmanız yeterlidir.

🛠️ Kullanılan Teknolojiler

HTML5 & CSS3

JavaScript (ES6+)

Tailwind CSS (CDN üzerinden stil işlemleri için)

FontAwesome (İkonlar için)

💻 Kurulum ve Kullanım

Bu projeyi çalıştırmak için herhangi bir kuruluma ihtiyacınız yoktur.

Bu repoyu bilgisayarınıza indirin (veya git clone yapın).

index.html dosyasına çift tıklayarak tarayıcınızda açın.

"Başlat" butonuna basarak simülasyonu izleyin.

GitHub Pages ile Canlı Önizleme

Bu projeyi GitHub Pages üzerinden saniyeler içinde yayınlayabilirsiniz:

Reponuzun Settings (Ayarlar) sekmesine gidin.

Sol menüden Pages'i seçin.

Branch kısmından main (veya master) seçip Save'e tıklayın.

GitHub size canlı bir link verecektir (örn: https://kullaniciadi.github.io/repo-adi/).

📝 Algoritma Mantığı (Java)

Simülasyonun temel aldığı Java kodu şöyledir:

public static void QST(Stack<E> s) {
    Queue<E> q = new Queue<E>();
    
    // Adım 1: Stack'i Kuyruğa boşalt
    while (!s.empty()) {
        q.enqueue(s.pop());
    }
    
    // Adım 2: Kuyruğu Stack'e geri boşalt
    while (!q.empty()) {
        s.push(q.dequeue());
    }
}


🤝 Katkıda Bulunma

Öneri ve düzeltmeleriniz için "Pull Request" göndermekten çekinmeyin!

📄 Lisans

Bu proje MIT License altında lisanslanmıştır.
