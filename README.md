# yas-cinsiyet-tahmini

  <h2>Veri Seti</h2>
  Projede <i>UTKFace</i> veri setlerini kullandım. Bu veri setinde bulunan veriler ham yüz verileridir.<i>Imdb-Wiki</i> veri setlerini isterseniz kullanabilirsiniz.
  
  <h2>Veri setinin bilgilerinin ayrılması</h2>
  Ham verileri creat_db_utkface.py üzerinde çalıştırarak (python3 create_db_utkface.py -i input/UTKFace -o input/UTKFace.mat veri seti neredeyse inputun yolu orası olması lazım ve nereye çıkarıcaksanız outputun yolu orası olması lazım) bir .mat dosyası oluşturuyoruz bu mat dosyasında veriler isimleri üzerinde verilen bilgilere göre ayrılarak yaş cinsiyet gibi tablolara ayrılıyor.
  
  <h2>Train</h2>
  Çıkan bu .mat dosyasını daha sonra train ederek bir kaç epoch sürüdyse eğitme .h5 dosyasında belirterek modelimizin çıktısını alıyoruz ve demo.py kısmında hangi modeli kullanacağımızı seçiyoruz ve modelimize göre anlık veya fotoğraftan yaş ve cinsiyetin tahminini yapıyor.
  
  <h3>NOT:</h3> Düşük sistemli bilgisayarlarda eğitim can sıkıcı derecede uzun olabilmektedir. Hazır eğitilmiş model boyut olarak fazla olduğu için konulamamaktadır.
