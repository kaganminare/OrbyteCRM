# Orbyte sosyal medya analitik prosedürü

Araçlar: Buffer get_account, list_channels, get_aggregated_post_metrics (7 ve 31 gün, kanal bazında), list_posts (status sent, includeMetrics true).

Boyutlar: platform, format (kinetik video, karusel, tek görsel, metin), konu, gün/saat, müzikli mi, haftalık gönderi sayısı.

Kurallar: n<5 hücre "kesin değil"; tek gönderiden sonuç çıkarılmaz; takipçi verisi yoksa "veri yok". Toplu metrik gecikmeli olabilir, list_posts ile çapraz kontrol edilir. Yeni yayınlanmış gönderilerin 0 değerleri yetersiz veri sayılır.

Deneyler (aynı anda tek değişken): Sıklık A (2 hf: LI 3, IG 2, FB 1) sonra B (2 hf: LI 5, IG 4, FB 2); B'de ort. erişim %25'ten fazla düşerse A'ya dön. Format: her format en az 3 deneme, sonra %70 en iyi, %30 keşif. Saat: LinkedIn 09:00-12:00 hipotezi.
