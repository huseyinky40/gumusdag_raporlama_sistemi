# Gümüşdağ Raporlama Sistemi

Bu depo, PySide6 ile geliştirilen tek dosyalık masaüstü raporlama prototipini içerir. Uygulama SQLite üzerinde çalışır ve günlük üretim kayıtlarıyla ilgili temel işlevleri sunar.

## Gereksinimler

Projeyi çalıştırmak için [Python 3.10+](https://www.python.org/downloads/) ve gerekli Python paketlerine ihtiyacınız vardır. Dışa bağımlı tek paket **PySide6**'dır ve `requirements.txt` dosyası aracılığıyla kurulabilir.

## Kurulum

1. (İsteğe bağlı) Temiz bir sanal ortam oluşturun ve etkinleştirin:
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # Windows: .venv\\Scripts\\activate
   ```
2. Gerekli paketleri kurun:
   ```bash
   pip install -r requirements.txt
   ```

Kurulum sırasında PySide6 modülü indirilip kurulacaktır. Eksik olduğunda uygulama "ModuleNotFoundError: No module named 'PySide6'" hatası verir; bu adım hatayı giderir.

## Çalıştırma

Uygulamayı başlatmak için proje kök dizininde aşağıdaki komutu çalıştırın:

```bash
python gumusdaga_raporlama_sistemi/raporlama_sistemi
```

(İsterseniz dosyayı bir `.py` uzantısı ile yeniden adlandırabilirsiniz; Python uzantısız dosyaları da yorumlayabilir.)

Uygulama açıldığında üretim bandı kayıtlarını ekleyip görüntüleyebilirsiniz. Veriler `raporlama.db` adlı SQLite veritabanında saklanır.
