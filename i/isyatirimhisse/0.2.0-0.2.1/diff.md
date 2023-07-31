# Comparing `tmp/isyatirimhisse-0.2.0.tar.gz` & `tmp/isyatirimhisse-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isyatirimhisse-0.2.0.tar", last modified: Sun Jul 30 13:47:43 2023, max compression
+gzip compressed data, was "isyatirimhisse-0.2.1.tar", last modified: Mon Jul 31 11:05:59 2023, max compression
```

## Comparing `isyatirimhisse-0.2.0.tar` & `isyatirimhisse-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 13:47:43.133457 isyatirimhisse-0.2.0/
--rw-rw-rw-   0        0        0     1064 2023-07-23 21:22:22.000000 isyatirimhisse-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0      173 2023-07-30 13:45:41.000000 isyatirimhisse-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0    10397 2023-07-30 13:47:43.132449 isyatirimhisse-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     9827 2023-07-30 13:46:51.000000 isyatirimhisse-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 13:47:42.971879 isyatirimhisse-0.2.0/imgs/
--rw-rw-rw-   0        0        0   111188 2023-07-30 13:15:39.000000 isyatirimhisse-0.2.0/imgs/gorsel_ornek_1.png
--rw-rw-rw-   0        0        0    53435 2023-07-30 13:29:30.000000 isyatirimhisse-0.2.0/imgs/gorsel_ornek_2.png
--rw-rw-rw-   0        0        0   433600 2023-07-30 13:17:48.000000 isyatirimhisse-0.2.0/imgs/gorsel_ornek_3.png
-drwxrwxrwx   0        0        0        0 2023-07-30 13:47:43.030729 isyatirimhisse-0.2.0/isyatirimhisse/
--rw-rw-rw-   0        0        0     4721 2023-07-30 12:56:36.000000 isyatirimhisse-0.2.0/isyatirimhisse/VeriCek.py
--rw-rw-rw-   0        0        0     4784 2023-07-30 13:35:14.000000 isyatirimhisse-0.2.0/isyatirimhisse/VeriGorsel.py
--rw-rw-rw-   0        0        0       66 2023-07-28 15:01:43.000000 isyatirimhisse-0.2.0/isyatirimhisse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:47:43.089564 isyatirimhisse-0.2.0/isyatirimhisse.egg-info/
--rw-rw-rw-   0        0        0    10397 2023-07-30 13:47:42.000000 isyatirimhisse-0.2.0/isyatirimhisse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-07-30 13:47:42.000000 isyatirimhisse-0.2.0/isyatirimhisse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 13:47:42.000000 isyatirimhisse-0.2.0/isyatirimhisse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-30 13:47:42.000000 isyatirimhisse-0.2.0/isyatirimhisse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-30 13:47:42.000000 isyatirimhisse-0.2.0/isyatirimhisse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 13:47:43.133457 isyatirimhisse-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      880 2023-07-30 13:39:59.000000 isyatirimhisse-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:47:43.126465 isyatirimhisse-0.2.0/tests/
--rw-rw-rw-   0        0        0        0 2023-07-25 09:00:45.000000 isyatirimhisse-0.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0     5009 2023-07-30 12:17:59.000000 isyatirimhisse-0.2.0/tests/test_veri_cek.py
--rw-rw-rw-   0        0        0     2729 2023-07-30 13:36:49.000000 isyatirimhisse-0.2.0/tests/test_veri_gorsel.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:05:59.352568 isyatirimhisse-0.2.1/
+-rw-rw-rw-   0        0        0     1064 2023-07-23 21:22:22.000000 isyatirimhisse-0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      147 2023-07-31 11:05:35.000000 isyatirimhisse-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    11144 2023-07-31 11:05:59.350572 isyatirimhisse-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10574 2023-07-31 11:03:13.000000 isyatirimhisse-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 11:05:59.203101 isyatirimhisse-0.2.1/imgs/
+-rw-rw-rw-   0        0        0   111188 2023-07-30 13:15:39.000000 isyatirimhisse-0.2.1/imgs/gorsel_ornek_1.png
+-rw-rw-rw-   0        0        0    53435 2023-07-30 13:29:30.000000 isyatirimhisse-0.2.1/imgs/gorsel_ornek_2.png
+-rw-rw-rw-   0        0        0   433600 2023-07-30 13:17:48.000000 isyatirimhisse-0.2.1/imgs/gorsel_ornek_3.png
+drwxrwxrwx   0        0        0        0 2023-07-31 11:05:59.253960 isyatirimhisse-0.2.1/isyatirimhisse/
+-rw-rw-rw-   0        0        0     4721 2023-07-30 12:56:36.000000 isyatirimhisse-0.2.1/isyatirimhisse/VeriCek.py
+-rw-rw-rw-   0        0        0     4784 2023-07-30 13:35:14.000000 isyatirimhisse-0.2.1/isyatirimhisse/VeriGorsel.py
+-rw-rw-rw-   0        0        0       66 2023-07-28 15:01:43.000000 isyatirimhisse-0.2.1/isyatirimhisse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:05:59.311679 isyatirimhisse-0.2.1/isyatirimhisse.egg-info/
+-rw-rw-rw-   0        0        0    11144 2023-07-31 11:05:58.000000 isyatirimhisse-0.2.1/isyatirimhisse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-07-31 11:05:59.000000 isyatirimhisse-0.2.1/isyatirimhisse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 11:05:58.000000 isyatirimhisse-0.2.1/isyatirimhisse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-31 11:05:58.000000 isyatirimhisse-0.2.1/isyatirimhisse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-31 11:05:58.000000 isyatirimhisse-0.2.1/isyatirimhisse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 11:05:59.352568 isyatirimhisse-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      949 2023-07-31 09:19:32.000000 isyatirimhisse-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:05:59.347582 isyatirimhisse-0.2.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-25 09:00:45.000000 isyatirimhisse-0.2.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     5009 2023-07-30 12:17:59.000000 isyatirimhisse-0.2.1/tests/test_veri_cek.py
+-rw-rw-rw-   0        0        0     2729 2023-07-30 13:36:49.000000 isyatirimhisse-0.2.1/tests/test_veri_gorsel.py
```

### Comparing `isyatirimhisse-0.2.0/LICENSE.txt` & `isyatirimhisse-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `isyatirimhisse-0.2.0/PKG-INFO` & `isyatirimhisse-0.2.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,46 @@
-Metadata-Version: 2.1
-Name: isyatirimhisse
-Version: 0.2.0
-Summary: İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştıran ve isteğe göre özelleştirilebilen bir kütüphane.
-Home-page: https://github.com/urazakgul/isyatirimhisse
-Author: Uraz Akgül
-Author-email: urazdev@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+# isyatirimhisse v0.2.1
 
-# isyatirimhisse v0.2.0
+## Açıklama
 
-## Aciklama
-
-`isyatirimhisse`, Is Yatirim'in web sitesinden veri cekme islemlerini kolaylastirmak amaciyla gelistirilmis, istege gore ozellestirilebilir bir Python kutuphanesidir.
+`isyatirimhisse`, İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştırmak amacıyla geliştirilmiş, isteğe göre özelleştirilebilir bir Python kütüphanesidir.
 
 *** UYARI ***
 
-`isyatirimhisse`, resmi Is Yatirim Menkul Degerler A.S. kutuphanesi degildir ve sirket tarafindan dogrulanmamistir. Kullanicilar, bu kutuphaneyi kullanmadan once ilgili tum verilere erisim icin Is Yatirim Menkul Degerler A.S. kullanim kosullarini ve haklarini incelemelidir. `isyatirimhisse` kutuphanesi, yalnizca kisisel kullanim amaclari icin tasarlanmistir.
+`isyatirimhisse`, resmi İş Yatırım Menkul Değerler A.Ş. kütüphanesi değildir ve şirket tarafından doğrulanmamıştır. Kullanıcılar, bu kütüphaneyi kullanmadan önce ilgili tüm verilere erişim için İş Yatırım Menkul Değerler A.Ş. kullanım koşullarını ve haklarını incelemelidir. `isyatirimhisse` kütüphanesi, yalnızca kişisel kullanım amaçları için tasarlanmıştır.
 
 ## Kurulum
 
-Kutuphaneyi kullanmak icin asagidaki adimlari izleyin:
+Kütüphaneyi kullanmak için aşağıdaki adımları izleyin:
 
-1. Python'i sisteminize yukleyin: https://www.python.org/downloads/
-2. Terminali acin ve paketi yuklemek icin asagidaki komutu calistirin:
+1. Python'ı sisteminize yükleyin: https://www.python.org/downloads/
+2. Terminali açın ve paketi yüklemek için aşağıdaki komutu çalıştırın:
 
 ```bash
 pip install isyatirimhisse
 ```
 
-Spesifik bir versiyona ait kurulum yapacaksaniz asagidaki ornekte oldugu gibi komutu calistirabilirsiniz.
+Spesifik bir versiyona ait kurulum yapacaksanız aşağıdaki örnekte olduğu gibi komutu çalıştırabilirsiniz.
 
 ```bash
-pip install isyatirimhisse==0.2.0
+pip install isyatirimhisse==0.2.1
 ```
 
-## Kullanim
+## Kullanım
 
-### Kutuphanenin Iceri Aktarilmasi
+### Kütüphanenin İçeri Aktarılması
 
 ```python
 from isyatirimhisse import veri_cek, veri_gorsel
 ```
 
-### Veri Cekme Ornekleri
+### Veri Çekme Örnekleri
 
 ```python
-# Tek hisse, gunluk frekans, logaritmik getiri ve excel olarak kaydet
+# Tek hisse, günlük frekans, logaritmik getiri ve excel olarak kaydet
 sembol = 'AKBNK'
 baslangic_tarih = '03-01-2023'
 bitis_tarih = '21-07-2023'
 frekans = '1g'
 gozlem = 'son'
 getiri_hesapla = True
 logaritmik_getiri = True
@@ -74,15 +59,15 @@
     excel_kaydet=excel_kaydet
 )
 
 print(veriler)
 ```
 
 ```python
-# Bitis tarihi yok ve spesifik isim ile excel olarak kaydet
+# Bitiş tarihi yok ve spesifik isim ile excel olarak kaydet
 sembol = 'AKBNK'
 baslangic_tarih = '03-01-2023'
 frekans = '1g'
 gozlem = 'son'
 getiri_hesapla = True
 logaritmik_getiri = True
 na_kaldir = True
@@ -101,15 +86,15 @@
     excel_dosya_ismi=excel_dosya_ismi
 )
 
 print(veriler)
 ```
 
 ```python
-# Birden fazla hisse, haftalik frekans, basit getiri, NA kaldir ve spesifik isim ile excel olarak kaydet
+# Birden fazla hisse, haftalık frekans, basit getiri, NA kaldır ve spesifik isim ile excel olarak kaydet
 sembol = ['AKBNK','EUPWR']
 baslangic_tarih = '03-01-2023'
 bitis_tarih = '21-07-2023'
 frekans = '1h'
 gozlem = 'son'
 getiri_hesapla = True
 logaritmik_getiri = False
@@ -130,15 +115,15 @@
     excel_dosya_ismi=excel_dosya_ismi
 )
 
 print(veriler)
 ```
 
 ```python
-# Birden fazla hisse, aylik frekans, kapanis fiyati, NA birak ve spesifik isim ile excel olarak kaydet
+# Birden fazla hisse, aylık frekans, kapanış fiyatı, NA bırak ve spesifik isim ile excel olarak kaydet
 sembol = ['AKBNK','EUPWR']
 baslangic_tarih = '03-01-2023'
 bitis_tarih = '21-07-2023'
 frekans = '1a'
 gozlem = 'son'
 getiri_hesapla = False
 logaritmik_getiri = True
@@ -159,15 +144,15 @@
     excel_dosya_ismi=excel_dosya_ismi
 )
 
 print(veriler)
 ```
 
 ```python
-# Birden fazla hisse, yillik frekans, kapanis fiyati, ortalama fiyatlar, NA kaldir ve excel olarak kaydetme
+# Birden fazla hisse, yıllık frekans, kapanış fiyatı, ortalama fiyatlar, NA kaldır ve excel olarak kaydetme
 sembol = ['AKBNK','EUPWR']
 baslangic_tarih = '03-01-2023'
 bitis_tarih = '21-07-2023'
 frekans = '1y'
 gozlem = 'ortalama'
 getiri_hesapla = False
 logaritmik_getiri = True
@@ -183,134 +168,140 @@
     logaritmik_getiri=logaritmik_getiri,
     na_kaldir=na_kaldir
 )
 
 print(veriler)
 ```
 
-### Veri Gorsellestirme Ornekleri
+### Veri Görselleştirme Örnekleri
 
 ```python
 veriler_df = veri_cek(
     sembol=['AKBNK','THYAO','GARAN','SISE','EREGL','BIMAS'],
     baslangic_tarih='01-01-2013',
     bitis_tarih='28-07-2023',
     frekans='1g',
     getiri_hesapla=False
 )
 
-# Cizgi grafik, fiyatlari normalize et ve linewidth ekle
+# Çizgi grafik, fiyatları normalize et ve linewidth ekle
 veri_gorsel(
     df=veriler_df,
     gorsel_turu='1',
     normalizasyon=True,
     linewidth=2
 )
 ```
 
-![](/imgs/gorsel_ornek_1.png)
+![](https://github.com/urazakgul/isyatirimhisse/blob/main/imgs/gorsel_ornek_1.png?raw=true)
 
 ```python
 veriler_df = veri_cek(
     sembol=['AKBNK','THYAO','GARAN','SISE','EREGL','BIMAS'],
     baslangic_tarih='02-01-2013',
     bitis_tarih='28-07-2023',
     frekans='1g',
     getiri_hesapla=True
 )
 
-# Korelasyon isi matrisi ve ek bir parametre ekleme
+# Korelasyon ısı matrisi ve ek bir parametre ekleme
 veri_gorsel(
     df=veriler_df,
     gorsel_turu='2'
 )
 ```
 
-![](/imgs/gorsel_ornek_2.png)
+![](https://github.com/urazakgul/isyatirimhisse/blob/main/imgs/gorsel_ornek_2.png?raw=true)
 
 ```python
 veriler_df = veri_cek(
     sembol=['AKBNK','THYAO','GARAN','SISE','EREGL','BIMAS'],
     baslangic_tarih='02-01-2013',
     bitis_tarih='28-07-2023',
     frekans='1g',
     getiri_hesapla=True
 )
 
-# Dagilim matrisi ve seffafligi artir
+# Dağılım matrisi ve şeffaflığı artır
 veri_gorsel(
     df=veriler_df,
     gorsel_turu='3',
     alpha=.1
 )
 ```
 
-![](/imgs/gorsel_ornek_3.png)
+![](https://github.com/urazakgul/isyatirimhisse/blob/main/imgs/gorsel_ornek_3.png?raw=true)
 
 ### `veri_cek` Fonksiyonuna Ait Parametreler
 
-* `sembol` (str veya list, varsayilan None): Hisse senedi sembolu veya sembollerinin listesi (Orn. `'AKBNK'` veya `['AKBNK','EUPWR']`)
-* `baslangic_tarih` (str, 'GG-AA-YYYY', varsayilan None): Verilerin baslangic tarihi (Orn. `'03-01-2023'`).
-* `bitis_tarih` (str, 'GG-AA-YYYY', varsayilan None): Verilerin bitis tarihi (Orn. `'21-07-2023'`). Eger belirtilmezse, sistem tarihini (bugunku tarihi) otomatik olarak kullanir.
-* `frekans` (str, varsayilan '1g'): Veri frekansi (`'1g'`: Gunluk, `'1h'`: Haftalik, `'1a'`: Aylik, `'1y'`: Yillik).
-* `gozlem` (str, varsayilan 'son'): Haftalik, aylik ve yillik frekanslarda istenen gozlem (`'son'`: Son, `'ortalama'`: Ortalama)
-* `getiri_hesapla` (bool, varsayilan True): Getiri hesaplanacak mi?
-* `logaritmik_getiri` (bool, varsayilan True): Logaritmik getiri mi hesaplanacak?
-* `na_kaldir` (bool, varsayilan True): Eksik degerler kaldirilacak mi?
-* `excel_kaydet` (bool, varsayilan False): pandas DataFrame Excel dosyasina kaydedilsin mi?
-* `excel_dosya_ismi` (str, varsayilan None): Kaydedilecek Excel dosyasinin ismi (Orn. 'veriler.xlsx' veya 'veriler'). Gecerli bir dosya ismi belirtilmezse, sistem tarihi kullanilarak 'veriler_YYYYMMDD.xlsx' ismiyle kaydedilir. Eger kaydedilecek dizinde ayni isimden baska bir dosya varsa farkli bir isimle kaydeder.
+* `sembol` (str veya list, varsayılan None): Hisse senedi sembolü veya sembollerinin listesi (Örn. `'AKBNK'` veya `['AKBNK','EUPWR']`)
+* `baslangic_tarih` (str, 'GG-AA-YYYY', varsayılan None): Verilerin başlangıç tarihi (Örn. `'03-01-2023'`).
+* `bitis_tarih` (str, 'GG-AA-YYYY', varsayılan None): Verilerin bitiş tarihi (Örn. `'21-07-2023'`). Eğer belirtilmezse, sistem tarihini (bugünkü tarihi) otomatik olarak kullanır.
+* `frekans` (str, varsayılan '1g'): Veri frekansı (`'1g'`: Günlük, `'1h'`: Haftalık, `'1a'`: Aylık, `'1y'`: Yıllık).
+* `gozlem` (str, varsayılan 'son'): Haftalık, aylık ve yıllık frekanslarda istenen gözlem (`'son'`: Son, `'ortalama'`: Ortalama)
+* `getiri_hesapla` (bool, varsayılan True): Getiri hesaplanacak mı?
+* `logaritmik_getiri` (bool, varsayılan True): Logaritmik getiri mi hesaplanacak?
+* `na_kaldir` (bool, varsayılan True): Eksik değerler kaldırılacak mı?
+* `excel_kaydet` (bool, varsayılan False): pandas DataFrame Excel dosyasına kaydedilsin mi?
+* `excel_dosya_ismi` (str, varsayılan None): Kaydedilecek Excel dosyasının ismi (Örn. 'veriler.xlsx' veya 'veriler'). Geçerli bir dosya ismi belirtilmezse, sistem tarihi kullanılarak 'veriler_YYYYMMDD.xlsx' ismiyle kaydedilir. Eğer kaydedilecek dizinde aynı isimden başka bir dosya varsa farklı bir isimle kaydeder.
 
 ### `veri_gorsel` Fonksiyonuna Ait Parametreler
 
-* `df` (pandas DataFrame, varsayilan None): Hisse senedi verilerinin bulundugu pandas DataFrame. Bu parametre zorunludur ve veri cercevesini belirtmek gereklidir.
-* `gorsel_turu` (str, varsayilan '1'). Hangi turde gorsellestirme yapilacagini belirlemek icin kullanilir.
-  * Gorsellestirme turunu belirten parametreye ait degerler:
-    * `'1'`: Cizgi Grafigi
-    * `'2'`: Korelasyon Isi Matrisi
-    * `'3'`: Dagilim Matrisi
-* `normalizasyon` (bool, varsayilan False): Verilerin normalize edilip edilmeyecegini belirten bir bool degeri. `True` olarak ayarlandiginda, veriler 0 ile 1 arasinda olceklendirilir.
-* `**kwargs`: Gorsellestirme turlerine ozel ek secenekler. Bu parametreler, belirli bir gorsellestirme turu icin ozel ayarlamalar yapmak icin kullanilabilir. Ancak gorsellestirme turune gore farkli olabilir ve zorunlu degildir.
-  * Gorsellestirme Turleri icin **kwargs Parametreleri:
-    * Cizgi Grafigi (gorsel_turu == '1'):
-      * `linewidth` (float, varsayilan 1.5): Cizgi kalinligi.
-    * Korelasyon Isi Matrisi (gorsel_turu == '2'):
-      * `cmap` (str, varsayilan 'coolwarm'): Renk haritasi.
-      * `vmin` (float, varsayilan -1): Renk haritasindaki en kucuk deger.
-      * `vmax` (float, varsayilan 1): Renk haritasindaki en buyuk deger.
-    * Dagilim Matrisi (gorsel_turu == '3'):
-      * `alpha` (float, varsayilan 0.5): Nokta seffafligi.
+* `df` (pandas DataFrame, varsayılan None): Hisse senedi verilerinin bulunduğu pandas DataFrame. Bu parametre zorunludur ve veri çerçevesini belirtmek gereklidir.
+* `gorsel_turu` (str, varsayılan '1'). Hangi türde görselleştirme yapılacağını belirlemek için kullanılır.
+  * Görselleştirme türünü belirten parametreye ait değerler:
+    * `'1'`: Çizgi Grafiği
+    * `'2'`: Korelasyon Isı Matrisi
+    * `'3'`: Dağılım Matrisi
+* `normalizasyon` (bool, varsayılan False): Verilerin normalize edilip edilmeyeceğini belirten bir bool değeri. `True` olarak ayarlandığında, veriler 0 ile 1 arasında ölçeklendirilir.
+* `**kwargs`: Görselleştirme türlerine özel ek seçenekler. Bu parametreler, belirli bir görselleştirme türü için özel ayarlamalar yapmak için kullanılabilir. Ancak görselleştirme türüne göre farklı olabilir ve zorunlu değildir.
+  * Görselleştirme Türleri için **kwargs Parametreleri:
+    * Çizgi Grafiği (gorsel_turu == '1'):
+      * `linewidth` (float, varsayılan 1.5): Çizgi kalınlığı.
+    * Korelasyon Isı Matrisi (gorsel_turu == '2'):
+      * `cmap` (str, varsayılan 'coolwarm'): Renk haritası.
+      * `vmin` (float, varsayılan -1): Renk haritasındaki en küçük değer.
+      * `vmax` (float, varsayılan 1): Renk haritasindaki en büyük değer.
+    * Dağılım Matrisi (gorsel_turu == '3'):
+      * `alpha` (float, varsayılan 0.5): Nokta şeffaflığı.
 
-### Donen Deger
+### Dönen Değer
 
-* `veri_cek` fonksiyonu bir pandas DataFrame dondurur.
-* `veri_gorsel` fonksiyonu, pandas DataFrame icerisindeki verileri grafikler ve gorsel ogelerle temsil eder.
+* `veri_cek` fonksiyonu bir pandas DataFrame döndürür.
+* `veri_gorsel` fonksiyonu, pandas DataFrame içerisindeki verileri grafikler ve görsel öğelerle temsil eder.
 
 ## Notlar
 
-* Kutuphane, Is Yatirim'in web sitesindeki verilere bagimlidir. Bu nedenle, verilerin dogrulugu ve surekliligi icin lutfen ilgili web sitesini kontrol edin: [Is Yatirim](https://www.isyatirim.com.tr/tr-tr/Sayfalar/default.aspx)
-* Kutuphanenin gelistirilmesi ve iyilestirilmesi icin geri bildirimlerinizi bekliyorum. GitHub reposuna katkida bulunun: [GitHub Repo](https://github.com/urazakgul/isyatirimhisse)
-* Herhangi bir sorun veya oneride lutfen GitHub reposundaki "Issue" bolumunden yeni bir konu acarak bildirim saglayin: [GitHub Issues](https://github.com/urazakgul/isyatirimhisse/issues)
+* Kütüphane, İş Yatırım'ın web sitesindeki verilere bağımlıdır. Bu nedenle, verilerin doğruluğu ve sürekliliği için lütfen ilgili web sitesini kontrol edin: [İş Yatırım](https://www.isyatirim.com.tr/tr-tr/Sayfalar/default.aspx)
+* Kütüphanenin geliştirilmesi ve iyileştirilmesi için geri bildirimlerinizi bekliyorum. GitHub reposuna katkıda bulunun: [GitHub Repo](https://github.com/urazakgul/isyatirimhisse)
+* Herhangi bir sorun veya öneride lütfen GitHub reposundaki "Issue" bölümünden yeni bir konu açarak bildirim sağlayın: [GitHub Issues](https://github.com/urazakgul/isyatirimhisse/issues)
 
-## Degisiklikler
+## Değişiklikler
 
 ### v0.1.0 - 25/07/2023
 
-* Ilk surum yayinlandi.
+* İlk sürüm yayınlandı.
 
 ### v0.1.1 - 27/07/2023
 
-* `veri_cek` fonksiyonundaki parametreleri kontrol eden kosul ifadeleri guncellendi.
-* `json` kutuphanesi kaldirildi.
-* `veri_cek` fonksiyonuna `200` HTTP kodu kosul ile beraber eklendi ve takibe alindi.
+* `veri_cek` fonksiyonundaki parametreleri kontrol eden koşul ifadeleri güncellendi.
+* `json` kütüphanesi kaldırıldı.
+* `veri_cek` fonksiyonuna `200` HTTP kodu koşul ile beraber eklendi ve takibe alındı.
 
 ### v0.2.0 - 30/07/2023
 
-* `veri_gorsel` fonksiyonu eklendi. Fonksiyon, 3 farkli veri turunde gorsellestirme yapma imkani sunuyor.
+* `veri_gorsel` fonksiyonu eklendi. Fonksiyon, 3 farklı veri türünde görselleştirme yapma imkanı sunuyor.
 * `veri_cek` fonksiyonuna pandas DataFrame'i excel olarak kaydedecek parametreler eklendi.
 
+### v0.2.1 - 31/07/2023
+
+* 0.2.0 sürümündeki kurulum hatası giderildi.
+* Dokümantasyondaki Türkçe karakter problemi giderildi.
+* Dokümantasyonda görünmeyen görseller görünür hale getirildi.
+
 ## Lisans
 
-Bu proje MIT Lisansi altinda lisanslanmistir.
+Bu proje MIT Lisansı altında lisanslanmıştır.
 
-## Katkida Bulunanlar
+## Katkıda Bulunanlar
 
-- [Sinan Erdinc](https://github.com/sinanerdinc)
+- [Sinan Erdinç](https://github.com/sinanerdinc)
```

### Comparing `isyatirimhisse-0.2.0/README.md` & `isyatirimhisse-0.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,61 @@
-# isyatirimhisse v0.2.0
+Metadata-Version: 2.1
+Name: isyatirimhisse
+Version: 0.2.1
+Summary: İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştıran ve isteğe göre özelleştirilebilen bir kütüphane.
+Home-page: https://github.com/urazakgul/isyatirimhisse
+Author: Uraz Akgül
+Author-email: urazdev@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
-## Aciklama
+# isyatirimhisse v0.2.1
 
-`isyatirimhisse`, Is Yatirim'in web sitesinden veri cekme islemlerini kolaylastirmak amaciyla gelistirilmis, istege gore ozellestirilebilir bir Python kutuphanesidir.
+## Açıklama
+
+`isyatirimhisse`, İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştırmak amacıyla geliştirilmiş, isteğe göre özelleştirilebilir bir Python kütüphanesidir.
 
 *** UYARI ***
 
-`isyatirimhisse`, resmi Is Yatirim Menkul Degerler A.S. kutuphanesi degildir ve sirket tarafindan dogrulanmamistir. Kullanicilar, bu kutuphaneyi kullanmadan once ilgili tum verilere erisim icin Is Yatirim Menkul Degerler A.S. kullanim kosullarini ve haklarini incelemelidir. `isyatirimhisse` kutuphanesi, yalnizca kisisel kullanim amaclari icin tasarlanmistir.
+`isyatirimhisse`, resmi İş Yatırım Menkul Değerler A.Ş. kütüphanesi değildir ve şirket tarafından doğrulanmamıştır. Kullanıcılar, bu kütüphaneyi kullanmadan önce ilgili tüm verilere erişim için İş Yatırım Menkul Değerler A.Ş. kullanım koşullarını ve haklarını incelemelidir. `isyatirimhisse` kütüphanesi, yalnızca kişisel kullanım amaçları için tasarlanmıştır.
 
 ## Kurulum
 
-Kutuphaneyi kullanmak icin asagidaki adimlari izleyin:
+Kütüphaneyi kullanmak için aşağıdaki adımları izleyin:
 
-1. Python'i sisteminize yukleyin: https://www.python.org/downloads/
-2. Terminali acin ve paketi yuklemek icin asagidaki komutu calistirin:
+1. Python'ı sisteminize yükleyin: https://www.python.org/downloads/
+2. Terminali açın ve paketi yüklemek için aşağıdaki komutu çalıştırın:
 
 ```bash
 pip install isyatirimhisse
 ```
 
-Spesifik bir versiyona ait kurulum yapacaksaniz asagidaki ornekte oldugu gibi komutu calistirabilirsiniz.
+Spesifik bir versiyona ait kurulum yapacaksanız aşağıdaki örnekte olduğu gibi komutu çalıştırabilirsiniz.
 
 ```bash
-pip install isyatirimhisse==0.2.0
+pip install isyatirimhisse==0.2.1
 ```
 
-## Kullanim
+## Kullanım
 
-### Kutuphanenin Iceri Aktarilmasi
+### Kütüphanenin İçeri Aktarılması
 
 ```python
 from isyatirimhisse import veri_cek, veri_gorsel
 ```
 
-### Veri Cekme Ornekleri
+### Veri Çekme Örnekleri
 
 ```python
-# Tek hisse, gunluk frekans, logaritmik getiri ve excel olarak kaydet
+# Tek hisse, günlük frekans, logaritmik getiri ve excel olarak kaydet
 sembol = 'AKBNK'
 baslangic_tarih = '03-01-2023'
 bitis_tarih = '21-07-2023'
 frekans = '1g'
 gozlem = 'son'
 getiri_hesapla = True
 logaritmik_getiri = True
@@ -59,15 +74,15 @@
     excel_kaydet=excel_kaydet
 )
 
 print(veriler)
 ```
 
 ```python
-# Bitis tarihi yok ve spesifik isim ile excel olarak kaydet
+# Bitiş tarihi yok ve spesifik isim ile excel olarak kaydet
 sembol = 'AKBNK'
 baslangic_tarih = '03-01-2023'
 frekans = '1g'
 gozlem = 'son'
 getiri_hesapla = True
 logaritmik_getiri = True
 na_kaldir = True
@@ -86,15 +101,15 @@
     excel_dosya_ismi=excel_dosya_ismi
 )
 
 print(veriler)
 ```
 
 ```python
-# Birden fazla hisse, haftalik frekans, basit getiri, NA kaldir ve spesifik isim ile excel olarak kaydet
+# Birden fazla hisse, haftalık frekans, basit getiri, NA kaldır ve spesifik isim ile excel olarak kaydet
 sembol = ['AKBNK','EUPWR']
 baslangic_tarih = '03-01-2023'
 bitis_tarih = '21-07-2023'
 frekans = '1h'
 gozlem = 'son'
 getiri_hesapla = True
 logaritmik_getiri = False
@@ -115,15 +130,15 @@
     excel_dosya_ismi=excel_dosya_ismi
 )
 
 print(veriler)
 ```
 
 ```python
-# Birden fazla hisse, aylik frekans, kapanis fiyati, NA birak ve spesifik isim ile excel olarak kaydet
+# Birden fazla hisse, aylık frekans, kapanış fiyatı, NA bırak ve spesifik isim ile excel olarak kaydet
 sembol = ['AKBNK','EUPWR']
 baslangic_tarih = '03-01-2023'
 bitis_tarih = '21-07-2023'
 frekans = '1a'
 gozlem = 'son'
 getiri_hesapla = False
 logaritmik_getiri = True
@@ -144,15 +159,15 @@
     excel_dosya_ismi=excel_dosya_ismi
 )
 
 print(veriler)
 ```
 
 ```python
-# Birden fazla hisse, yillik frekans, kapanis fiyati, ortalama fiyatlar, NA kaldir ve excel olarak kaydetme
+# Birden fazla hisse, yıllık frekans, kapanış fiyatı, ortalama fiyatlar, NA kaldır ve excel olarak kaydetme
 sembol = ['AKBNK','EUPWR']
 baslangic_tarih = '03-01-2023'
 bitis_tarih = '21-07-2023'
 frekans = '1y'
 gozlem = 'ortalama'
 getiri_hesapla = False
 logaritmik_getiri = True
@@ -168,134 +183,140 @@
     logaritmik_getiri=logaritmik_getiri,
     na_kaldir=na_kaldir
 )
 
 print(veriler)
 ```
 
-### Veri Gorsellestirme Ornekleri
+### Veri Görselleştirme Örnekleri
 
 ```python
 veriler_df = veri_cek(
     sembol=['AKBNK','THYAO','GARAN','SISE','EREGL','BIMAS'],
     baslangic_tarih='01-01-2013',
     bitis_tarih='28-07-2023',
     frekans='1g',
     getiri_hesapla=False
 )
 
-# Cizgi grafik, fiyatlari normalize et ve linewidth ekle
+# Çizgi grafik, fiyatları normalize et ve linewidth ekle
 veri_gorsel(
     df=veriler_df,
     gorsel_turu='1',
     normalizasyon=True,
     linewidth=2
 )
 ```
 
-![](/imgs/gorsel_ornek_1.png)
+![](https://github.com/urazakgul/isyatirimhisse/blob/main/imgs/gorsel_ornek_1.png?raw=true)
 
 ```python
 veriler_df = veri_cek(
     sembol=['AKBNK','THYAO','GARAN','SISE','EREGL','BIMAS'],
     baslangic_tarih='02-01-2013',
     bitis_tarih='28-07-2023',
     frekans='1g',
     getiri_hesapla=True
 )
 
-# Korelasyon isi matrisi ve ek bir parametre ekleme
+# Korelasyon ısı matrisi ve ek bir parametre ekleme
 veri_gorsel(
     df=veriler_df,
     gorsel_turu='2'
 )
 ```
 
-![](/imgs/gorsel_ornek_2.png)
+![](https://github.com/urazakgul/isyatirimhisse/blob/main/imgs/gorsel_ornek_2.png?raw=true)
 
 ```python
 veriler_df = veri_cek(
     sembol=['AKBNK','THYAO','GARAN','SISE','EREGL','BIMAS'],
     baslangic_tarih='02-01-2013',
     bitis_tarih='28-07-2023',
     frekans='1g',
     getiri_hesapla=True
 )
 
-# Dagilim matrisi ve seffafligi artir
+# Dağılım matrisi ve şeffaflığı artır
 veri_gorsel(
     df=veriler_df,
     gorsel_turu='3',
     alpha=.1
 )
 ```
 
-![](/imgs/gorsel_ornek_3.png)
+![](https://github.com/urazakgul/isyatirimhisse/blob/main/imgs/gorsel_ornek_3.png?raw=true)
 
 ### `veri_cek` Fonksiyonuna Ait Parametreler
 
-* `sembol` (str veya list, varsayilan None): Hisse senedi sembolu veya sembollerinin listesi (Orn. `'AKBNK'` veya `['AKBNK','EUPWR']`)
-* `baslangic_tarih` (str, 'GG-AA-YYYY', varsayilan None): Verilerin baslangic tarihi (Orn. `'03-01-2023'`).
-* `bitis_tarih` (str, 'GG-AA-YYYY', varsayilan None): Verilerin bitis tarihi (Orn. `'21-07-2023'`). Eger belirtilmezse, sistem tarihini (bugunku tarihi) otomatik olarak kullanir.
-* `frekans` (str, varsayilan '1g'): Veri frekansi (`'1g'`: Gunluk, `'1h'`: Haftalik, `'1a'`: Aylik, `'1y'`: Yillik).
-* `gozlem` (str, varsayilan 'son'): Haftalik, aylik ve yillik frekanslarda istenen gozlem (`'son'`: Son, `'ortalama'`: Ortalama)
-* `getiri_hesapla` (bool, varsayilan True): Getiri hesaplanacak mi?
-* `logaritmik_getiri` (bool, varsayilan True): Logaritmik getiri mi hesaplanacak?
-* `na_kaldir` (bool, varsayilan True): Eksik degerler kaldirilacak mi?
-* `excel_kaydet` (bool, varsayilan False): pandas DataFrame Excel dosyasina kaydedilsin mi?
-* `excel_dosya_ismi` (str, varsayilan None): Kaydedilecek Excel dosyasinin ismi (Orn. 'veriler.xlsx' veya 'veriler'). Gecerli bir dosya ismi belirtilmezse, sistem tarihi kullanilarak 'veriler_YYYYMMDD.xlsx' ismiyle kaydedilir. Eger kaydedilecek dizinde ayni isimden baska bir dosya varsa farkli bir isimle kaydeder.
+* `sembol` (str veya list, varsayılan None): Hisse senedi sembolü veya sembollerinin listesi (Örn. `'AKBNK'` veya `['AKBNK','EUPWR']`)
+* `baslangic_tarih` (str, 'GG-AA-YYYY', varsayılan None): Verilerin başlangıç tarihi (Örn. `'03-01-2023'`).
+* `bitis_tarih` (str, 'GG-AA-YYYY', varsayılan None): Verilerin bitiş tarihi (Örn. `'21-07-2023'`). Eğer belirtilmezse, sistem tarihini (bugünkü tarihi) otomatik olarak kullanır.
+* `frekans` (str, varsayılan '1g'): Veri frekansı (`'1g'`: Günlük, `'1h'`: Haftalık, `'1a'`: Aylık, `'1y'`: Yıllık).
+* `gozlem` (str, varsayılan 'son'): Haftalık, aylık ve yıllık frekanslarda istenen gözlem (`'son'`: Son, `'ortalama'`: Ortalama)
+* `getiri_hesapla` (bool, varsayılan True): Getiri hesaplanacak mı?
+* `logaritmik_getiri` (bool, varsayılan True): Logaritmik getiri mi hesaplanacak?
+* `na_kaldir` (bool, varsayılan True): Eksik değerler kaldırılacak mı?
+* `excel_kaydet` (bool, varsayılan False): pandas DataFrame Excel dosyasına kaydedilsin mi?
+* `excel_dosya_ismi` (str, varsayılan None): Kaydedilecek Excel dosyasının ismi (Örn. 'veriler.xlsx' veya 'veriler'). Geçerli bir dosya ismi belirtilmezse, sistem tarihi kullanılarak 'veriler_YYYYMMDD.xlsx' ismiyle kaydedilir. Eğer kaydedilecek dizinde aynı isimden başka bir dosya varsa farklı bir isimle kaydeder.
 
 ### `veri_gorsel` Fonksiyonuna Ait Parametreler
 
-* `df` (pandas DataFrame, varsayilan None): Hisse senedi verilerinin bulundugu pandas DataFrame. Bu parametre zorunludur ve veri cercevesini belirtmek gereklidir.
-* `gorsel_turu` (str, varsayilan '1'). Hangi turde gorsellestirme yapilacagini belirlemek icin kullanilir.
-  * Gorsellestirme turunu belirten parametreye ait degerler:
-    * `'1'`: Cizgi Grafigi
-    * `'2'`: Korelasyon Isi Matrisi
-    * `'3'`: Dagilim Matrisi
-* `normalizasyon` (bool, varsayilan False): Verilerin normalize edilip edilmeyecegini belirten bir bool degeri. `True` olarak ayarlandiginda, veriler 0 ile 1 arasinda olceklendirilir.
-* `**kwargs`: Gorsellestirme turlerine ozel ek secenekler. Bu parametreler, belirli bir gorsellestirme turu icin ozel ayarlamalar yapmak icin kullanilabilir. Ancak gorsellestirme turune gore farkli olabilir ve zorunlu degildir.
-  * Gorsellestirme Turleri icin **kwargs Parametreleri:
-    * Cizgi Grafigi (gorsel_turu == '1'):
-      * `linewidth` (float, varsayilan 1.5): Cizgi kalinligi.
-    * Korelasyon Isi Matrisi (gorsel_turu == '2'):
-      * `cmap` (str, varsayilan 'coolwarm'): Renk haritasi.
-      * `vmin` (float, varsayilan -1): Renk haritasindaki en kucuk deger.
-      * `vmax` (float, varsayilan 1): Renk haritasindaki en buyuk deger.
-    * Dagilim Matrisi (gorsel_turu == '3'):
-      * `alpha` (float, varsayilan 0.5): Nokta seffafligi.
+* `df` (pandas DataFrame, varsayılan None): Hisse senedi verilerinin bulunduğu pandas DataFrame. Bu parametre zorunludur ve veri çerçevesini belirtmek gereklidir.
+* `gorsel_turu` (str, varsayılan '1'). Hangi türde görselleştirme yapılacağını belirlemek için kullanılır.
+  * Görselleştirme türünü belirten parametreye ait değerler:
+    * `'1'`: Çizgi Grafiği
+    * `'2'`: Korelasyon Isı Matrisi
+    * `'3'`: Dağılım Matrisi
+* `normalizasyon` (bool, varsayılan False): Verilerin normalize edilip edilmeyeceğini belirten bir bool değeri. `True` olarak ayarlandığında, veriler 0 ile 1 arasında ölçeklendirilir.
+* `**kwargs`: Görselleştirme türlerine özel ek seçenekler. Bu parametreler, belirli bir görselleştirme türü için özel ayarlamalar yapmak için kullanılabilir. Ancak görselleştirme türüne göre farklı olabilir ve zorunlu değildir.
+  * Görselleştirme Türleri için **kwargs Parametreleri:
+    * Çizgi Grafiği (gorsel_turu == '1'):
+      * `linewidth` (float, varsayılan 1.5): Çizgi kalınlığı.
+    * Korelasyon Isı Matrisi (gorsel_turu == '2'):
+      * `cmap` (str, varsayılan 'coolwarm'): Renk haritası.
+      * `vmin` (float, varsayılan -1): Renk haritasındaki en küçük değer.
+      * `vmax` (float, varsayılan 1): Renk haritasindaki en büyük değer.
+    * Dağılım Matrisi (gorsel_turu == '3'):
+      * `alpha` (float, varsayılan 0.5): Nokta şeffaflığı.
 
-### Donen Deger
+### Dönen Değer
 
-* `veri_cek` fonksiyonu bir pandas DataFrame dondurur.
-* `veri_gorsel` fonksiyonu, pandas DataFrame icerisindeki verileri grafikler ve gorsel ogelerle temsil eder.
+* `veri_cek` fonksiyonu bir pandas DataFrame döndürür.
+* `veri_gorsel` fonksiyonu, pandas DataFrame içerisindeki verileri grafikler ve görsel öğelerle temsil eder.
 
 ## Notlar
 
-* Kutuphane, Is Yatirim'in web sitesindeki verilere bagimlidir. Bu nedenle, verilerin dogrulugu ve surekliligi icin lutfen ilgili web sitesini kontrol edin: [Is Yatirim](https://www.isyatirim.com.tr/tr-tr/Sayfalar/default.aspx)
-* Kutuphanenin gelistirilmesi ve iyilestirilmesi icin geri bildirimlerinizi bekliyorum. GitHub reposuna katkida bulunun: [GitHub Repo](https://github.com/urazakgul/isyatirimhisse)
-* Herhangi bir sorun veya oneride lutfen GitHub reposundaki "Issue" bolumunden yeni bir konu acarak bildirim saglayin: [GitHub Issues](https://github.com/urazakgul/isyatirimhisse/issues)
+* Kütüphane, İş Yatırım'ın web sitesindeki verilere bağımlıdır. Bu nedenle, verilerin doğruluğu ve sürekliliği için lütfen ilgili web sitesini kontrol edin: [İş Yatırım](https://www.isyatirim.com.tr/tr-tr/Sayfalar/default.aspx)
+* Kütüphanenin geliştirilmesi ve iyileştirilmesi için geri bildirimlerinizi bekliyorum. GitHub reposuna katkıda bulunun: [GitHub Repo](https://github.com/urazakgul/isyatirimhisse)
+* Herhangi bir sorun veya öneride lütfen GitHub reposundaki "Issue" bölümünden yeni bir konu açarak bildirim sağlayın: [GitHub Issues](https://github.com/urazakgul/isyatirimhisse/issues)
 
-## Degisiklikler
+## Değişiklikler
 
 ### v0.1.0 - 25/07/2023
 
-* Ilk surum yayinlandi.
+* İlk sürüm yayınlandı.
 
 ### v0.1.1 - 27/07/2023
 
-* `veri_cek` fonksiyonundaki parametreleri kontrol eden kosul ifadeleri guncellendi.
-* `json` kutuphanesi kaldirildi.
-* `veri_cek` fonksiyonuna `200` HTTP kodu kosul ile beraber eklendi ve takibe alindi.
+* `veri_cek` fonksiyonundaki parametreleri kontrol eden koşul ifadeleri güncellendi.
+* `json` kütüphanesi kaldırıldı.
+* `veri_cek` fonksiyonuna `200` HTTP kodu koşul ile beraber eklendi ve takibe alındı.
 
 ### v0.2.0 - 30/07/2023
 
-* `veri_gorsel` fonksiyonu eklendi. Fonksiyon, 3 farkli veri turunde gorsellestirme yapma imkani sunuyor.
+* `veri_gorsel` fonksiyonu eklendi. Fonksiyon, 3 farklı veri türünde görselleştirme yapma imkanı sunuyor.
 * `veri_cek` fonksiyonuna pandas DataFrame'i excel olarak kaydedecek parametreler eklendi.
 
+### v0.2.1 - 31/07/2023
+
+* 0.2.0 sürümündeki kurulum hatası giderildi.
+* Dokümantasyondaki Türkçe karakter problemi giderildi.
+* Dokümantasyonda görünmeyen görseller görünür hale getirildi.
+
 ## Lisans
 
-Bu proje MIT Lisansi altinda lisanslanmistir.
+Bu proje MIT Lisansı altında lisanslanmıştır.
 
-## Katkida Bulunanlar
+## Katkıda Bulunanlar
 
-- [Sinan Erdinc](https://github.com/sinanerdinc)
+- [Sinan Erdinç](https://github.com/sinanerdinc)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `isyatirimhisse-0.2.0/imgs/gorsel_ornek_1.png` & `isyatirimhisse-0.2.1/imgs/gorsel_ornek_1.png`

 * *Files identical despite different names*

### Comparing `isyatirimhisse-0.2.0/imgs/gorsel_ornek_2.png` & `isyatirimhisse-0.2.1/imgs/gorsel_ornek_2.png`

 * *Files identical despite different names*

### Comparing `isyatirimhisse-0.2.0/imgs/gorsel_ornek_3.png` & `isyatirimhisse-0.2.1/imgs/gorsel_ornek_3.png`

 * *Files identical despite different names*

### Comparing `isyatirimhisse-0.2.0/isyatirimhisse/VeriCek.py` & `isyatirimhisse-0.2.1/isyatirimhisse/VeriCek.py`

 * *Files identical despite different names*

### Comparing `isyatirimhisse-0.2.0/isyatirimhisse/VeriGorsel.py` & `isyatirimhisse-0.2.1/isyatirimhisse/VeriGorsel.py`

 * *Files identical despite different names*

### Comparing `isyatirimhisse-0.2.0/isyatirimhisse.egg-info/PKG-INFO` & `isyatirimhisse-0.2.1/isyatirimhisse.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 Metadata-Version: 2.1
 Name: isyatirimhisse
-Version: 0.2.0
+Version: 0.2.1
 Summary: İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştıran ve isteğe göre özelleştirilebilen bir kütüphane.
 Home-page: https://github.com/urazakgul/isyatirimhisse
 Author: Uraz Akgül
 Author-email: urazdev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# isyatirimhisse v0.2.0
+# isyatirimhisse v0.2.1
 
-## Aciklama
+## Açıklama
 
-`isyatirimhisse`, Is Yatirim'in web sitesinden veri cekme islemlerini kolaylastirmak amaciyla gelistirilmis, istege gore ozellestirilebilir bir Python kutuphanesidir.
+`isyatirimhisse`, İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştırmak amacıyla geliştirilmiş, isteğe göre özelleştirilebilir bir Python kütüphanesidir.
 
 *** UYARI ***
 
-`isyatirimhisse`, resmi Is Yatirim Menkul Degerler A.S. kutuphanesi degildir ve sirket tarafindan dogrulanmamistir. Kullanicilar, bu kutuphaneyi kullanmadan once ilgili tum verilere erisim icin Is Yatirim Menkul Degerler A.S. kullanim kosullarini ve haklarini incelemelidir. `isyatirimhisse` kutuphanesi, yalnizca kisisel kullanim amaclari icin tasarlanmistir.
+`isyatirimhisse`, resmi İş Yatırım Menkul Değerler A.Ş. kütüphanesi değildir ve şirket tarafından doğrulanmamıştır. Kullanıcılar, bu kütüphaneyi kullanmadan önce ilgili tüm verilere erişim için İş Yatırım Menkul Değerler A.Ş. kullanım koşullarını ve haklarını incelemelidir. `isyatirimhisse` kütüphanesi, yalnızca kişisel kullanım amaçları için tasarlanmıştır.
 
 ## Kurulum
 
-Kutuphaneyi kullanmak icin asagidaki adimlari izleyin:
+Kütüphaneyi kullanmak için aşağıdaki adımları izleyin:
 
-1. Python'i sisteminize yukleyin: https://www.python.org/downloads/
-2. Terminali acin ve paketi yuklemek icin asagidaki komutu calistirin:
+1. Python'ı sisteminize yükleyin: https://www.python.org/downloads/
+2. Terminali açın ve paketi yüklemek için aşağıdaki komutu çalıştırın:
 
 ```bash
 pip install isyatirimhisse
 ```
 
-Spesifik bir versiyona ait kurulum yapacaksaniz asagidaki ornekte oldugu gibi komutu calistirabilirsiniz.
+Spesifik bir versiyona ait kurulum yapacaksanız aşağıdaki örnekte olduğu gibi komutu çalıştırabilirsiniz.
 
 ```bash
-pip install isyatirimhisse==0.2.0
+pip install isyatirimhisse==0.2.1
 ```
 
-## Kullanim
+## Kullanım
 
-### Kutuphanenin Iceri Aktarilmasi
+### Kütüphanenin İçeri Aktarılması
 
 ```python
 from isyatirimhisse import veri_cek, veri_gorsel
 ```
 
-### Veri Cekme Ornekleri
+### Veri Çekme Örnekleri
 
 ```python
-# Tek hisse, gunluk frekans, logaritmik getiri ve excel olarak kaydet
+# Tek hisse, günlük frekans, logaritmik getiri ve excel olarak kaydet
 sembol = 'AKBNK'
 baslangic_tarih = '03-01-2023'
 bitis_tarih = '21-07-2023'
 frekans = '1g'
 gozlem = 'son'
 getiri_hesapla = True
 logaritmik_getiri = True
@@ -74,15 +74,15 @@
     excel_kaydet=excel_kaydet
 )
 
 print(veriler)
 ```
 
 ```python
-# Bitis tarihi yok ve spesifik isim ile excel olarak kaydet
+# Bitiş tarihi yok ve spesifik isim ile excel olarak kaydet
 sembol = 'AKBNK'
 baslangic_tarih = '03-01-2023'
 frekans = '1g'
 gozlem = 'son'
 getiri_hesapla = True
 logaritmik_getiri = True
 na_kaldir = True
@@ -101,15 +101,15 @@
     excel_dosya_ismi=excel_dosya_ismi
 )
 
 print(veriler)
 ```
 
 ```python
-# Birden fazla hisse, haftalik frekans, basit getiri, NA kaldir ve spesifik isim ile excel olarak kaydet
+# Birden fazla hisse, haftalık frekans, basit getiri, NA kaldır ve spesifik isim ile excel olarak kaydet
 sembol = ['AKBNK','EUPWR']
 baslangic_tarih = '03-01-2023'
 bitis_tarih = '21-07-2023'
 frekans = '1h'
 gozlem = 'son'
 getiri_hesapla = True
 logaritmik_getiri = False
@@ -130,15 +130,15 @@
     excel_dosya_ismi=excel_dosya_ismi
 )
 
 print(veriler)
 ```
 
 ```python
-# Birden fazla hisse, aylik frekans, kapanis fiyati, NA birak ve spesifik isim ile excel olarak kaydet
+# Birden fazla hisse, aylık frekans, kapanış fiyatı, NA bırak ve spesifik isim ile excel olarak kaydet
 sembol = ['AKBNK','EUPWR']
 baslangic_tarih = '03-01-2023'
 bitis_tarih = '21-07-2023'
 frekans = '1a'
 gozlem = 'son'
 getiri_hesapla = False
 logaritmik_getiri = True
@@ -159,15 +159,15 @@
     excel_dosya_ismi=excel_dosya_ismi
 )
 
 print(veriler)
 ```
 
 ```python
-# Birden fazla hisse, yillik frekans, kapanis fiyati, ortalama fiyatlar, NA kaldir ve excel olarak kaydetme
+# Birden fazla hisse, yıllık frekans, kapanış fiyatı, ortalama fiyatlar, NA kaldır ve excel olarak kaydetme
 sembol = ['AKBNK','EUPWR']
 baslangic_tarih = '03-01-2023'
 bitis_tarih = '21-07-2023'
 frekans = '1y'
 gozlem = 'ortalama'
 getiri_hesapla = False
 logaritmik_getiri = True
@@ -183,134 +183,140 @@
     logaritmik_getiri=logaritmik_getiri,
     na_kaldir=na_kaldir
 )
 
 print(veriler)
 ```
 
-### Veri Gorsellestirme Ornekleri
+### Veri Görselleştirme Örnekleri
 
 ```python
 veriler_df = veri_cek(
     sembol=['AKBNK','THYAO','GARAN','SISE','EREGL','BIMAS'],
     baslangic_tarih='01-01-2013',
     bitis_tarih='28-07-2023',
     frekans='1g',
     getiri_hesapla=False
 )
 
-# Cizgi grafik, fiyatlari normalize et ve linewidth ekle
+# Çizgi grafik, fiyatları normalize et ve linewidth ekle
 veri_gorsel(
     df=veriler_df,
     gorsel_turu='1',
     normalizasyon=True,
     linewidth=2
 )
 ```
 
-![](/imgs/gorsel_ornek_1.png)
+![](https://github.com/urazakgul/isyatirimhisse/blob/main/imgs/gorsel_ornek_1.png?raw=true)
 
 ```python
 veriler_df = veri_cek(
     sembol=['AKBNK','THYAO','GARAN','SISE','EREGL','BIMAS'],
     baslangic_tarih='02-01-2013',
     bitis_tarih='28-07-2023',
     frekans='1g',
     getiri_hesapla=True
 )
 
-# Korelasyon isi matrisi ve ek bir parametre ekleme
+# Korelasyon ısı matrisi ve ek bir parametre ekleme
 veri_gorsel(
     df=veriler_df,
     gorsel_turu='2'
 )
 ```
 
-![](/imgs/gorsel_ornek_2.png)
+![](https://github.com/urazakgul/isyatirimhisse/blob/main/imgs/gorsel_ornek_2.png?raw=true)
 
 ```python
 veriler_df = veri_cek(
     sembol=['AKBNK','THYAO','GARAN','SISE','EREGL','BIMAS'],
     baslangic_tarih='02-01-2013',
     bitis_tarih='28-07-2023',
     frekans='1g',
     getiri_hesapla=True
 )
 
-# Dagilim matrisi ve seffafligi artir
+# Dağılım matrisi ve şeffaflığı artır
 veri_gorsel(
     df=veriler_df,
     gorsel_turu='3',
     alpha=.1
 )
 ```
 
-![](/imgs/gorsel_ornek_3.png)
+![](https://github.com/urazakgul/isyatirimhisse/blob/main/imgs/gorsel_ornek_3.png?raw=true)
 
 ### `veri_cek` Fonksiyonuna Ait Parametreler
 
-* `sembol` (str veya list, varsayilan None): Hisse senedi sembolu veya sembollerinin listesi (Orn. `'AKBNK'` veya `['AKBNK','EUPWR']`)
-* `baslangic_tarih` (str, 'GG-AA-YYYY', varsayilan None): Verilerin baslangic tarihi (Orn. `'03-01-2023'`).
-* `bitis_tarih` (str, 'GG-AA-YYYY', varsayilan None): Verilerin bitis tarihi (Orn. `'21-07-2023'`). Eger belirtilmezse, sistem tarihini (bugunku tarihi) otomatik olarak kullanir.
-* `frekans` (str, varsayilan '1g'): Veri frekansi (`'1g'`: Gunluk, `'1h'`: Haftalik, `'1a'`: Aylik, `'1y'`: Yillik).
-* `gozlem` (str, varsayilan 'son'): Haftalik, aylik ve yillik frekanslarda istenen gozlem (`'son'`: Son, `'ortalama'`: Ortalama)
-* `getiri_hesapla` (bool, varsayilan True): Getiri hesaplanacak mi?
-* `logaritmik_getiri` (bool, varsayilan True): Logaritmik getiri mi hesaplanacak?
-* `na_kaldir` (bool, varsayilan True): Eksik degerler kaldirilacak mi?
-* `excel_kaydet` (bool, varsayilan False): pandas DataFrame Excel dosyasina kaydedilsin mi?
-* `excel_dosya_ismi` (str, varsayilan None): Kaydedilecek Excel dosyasinin ismi (Orn. 'veriler.xlsx' veya 'veriler'). Gecerli bir dosya ismi belirtilmezse, sistem tarihi kullanilarak 'veriler_YYYYMMDD.xlsx' ismiyle kaydedilir. Eger kaydedilecek dizinde ayni isimden baska bir dosya varsa farkli bir isimle kaydeder.
+* `sembol` (str veya list, varsayılan None): Hisse senedi sembolü veya sembollerinin listesi (Örn. `'AKBNK'` veya `['AKBNK','EUPWR']`)
+* `baslangic_tarih` (str, 'GG-AA-YYYY', varsayılan None): Verilerin başlangıç tarihi (Örn. `'03-01-2023'`).
+* `bitis_tarih` (str, 'GG-AA-YYYY', varsayılan None): Verilerin bitiş tarihi (Örn. `'21-07-2023'`). Eğer belirtilmezse, sistem tarihini (bugünkü tarihi) otomatik olarak kullanır.
+* `frekans` (str, varsayılan '1g'): Veri frekansı (`'1g'`: Günlük, `'1h'`: Haftalık, `'1a'`: Aylık, `'1y'`: Yıllık).
+* `gozlem` (str, varsayılan 'son'): Haftalık, aylık ve yıllık frekanslarda istenen gözlem (`'son'`: Son, `'ortalama'`: Ortalama)
+* `getiri_hesapla` (bool, varsayılan True): Getiri hesaplanacak mı?
+* `logaritmik_getiri` (bool, varsayılan True): Logaritmik getiri mi hesaplanacak?
+* `na_kaldir` (bool, varsayılan True): Eksik değerler kaldırılacak mı?
+* `excel_kaydet` (bool, varsayılan False): pandas DataFrame Excel dosyasına kaydedilsin mi?
+* `excel_dosya_ismi` (str, varsayılan None): Kaydedilecek Excel dosyasının ismi (Örn. 'veriler.xlsx' veya 'veriler'). Geçerli bir dosya ismi belirtilmezse, sistem tarihi kullanılarak 'veriler_YYYYMMDD.xlsx' ismiyle kaydedilir. Eğer kaydedilecek dizinde aynı isimden başka bir dosya varsa farklı bir isimle kaydeder.
 
 ### `veri_gorsel` Fonksiyonuna Ait Parametreler
 
-* `df` (pandas DataFrame, varsayilan None): Hisse senedi verilerinin bulundugu pandas DataFrame. Bu parametre zorunludur ve veri cercevesini belirtmek gereklidir.
-* `gorsel_turu` (str, varsayilan '1'). Hangi turde gorsellestirme yapilacagini belirlemek icin kullanilir.
-  * Gorsellestirme turunu belirten parametreye ait degerler:
-    * `'1'`: Cizgi Grafigi
-    * `'2'`: Korelasyon Isi Matrisi
-    * `'3'`: Dagilim Matrisi
-* `normalizasyon` (bool, varsayilan False): Verilerin normalize edilip edilmeyecegini belirten bir bool degeri. `True` olarak ayarlandiginda, veriler 0 ile 1 arasinda olceklendirilir.
-* `**kwargs`: Gorsellestirme turlerine ozel ek secenekler. Bu parametreler, belirli bir gorsellestirme turu icin ozel ayarlamalar yapmak icin kullanilabilir. Ancak gorsellestirme turune gore farkli olabilir ve zorunlu degildir.
-  * Gorsellestirme Turleri icin **kwargs Parametreleri:
-    * Cizgi Grafigi (gorsel_turu == '1'):
-      * `linewidth` (float, varsayilan 1.5): Cizgi kalinligi.
-    * Korelasyon Isi Matrisi (gorsel_turu == '2'):
-      * `cmap` (str, varsayilan 'coolwarm'): Renk haritasi.
-      * `vmin` (float, varsayilan -1): Renk haritasindaki en kucuk deger.
-      * `vmax` (float, varsayilan 1): Renk haritasindaki en buyuk deger.
-    * Dagilim Matrisi (gorsel_turu == '3'):
-      * `alpha` (float, varsayilan 0.5): Nokta seffafligi.
+* `df` (pandas DataFrame, varsayılan None): Hisse senedi verilerinin bulunduğu pandas DataFrame. Bu parametre zorunludur ve veri çerçevesini belirtmek gereklidir.
+* `gorsel_turu` (str, varsayılan '1'). Hangi türde görselleştirme yapılacağını belirlemek için kullanılır.
+  * Görselleştirme türünü belirten parametreye ait değerler:
+    * `'1'`: Çizgi Grafiği
+    * `'2'`: Korelasyon Isı Matrisi
+    * `'3'`: Dağılım Matrisi
+* `normalizasyon` (bool, varsayılan False): Verilerin normalize edilip edilmeyeceğini belirten bir bool değeri. `True` olarak ayarlandığında, veriler 0 ile 1 arasında ölçeklendirilir.
+* `**kwargs`: Görselleştirme türlerine özel ek seçenekler. Bu parametreler, belirli bir görselleştirme türü için özel ayarlamalar yapmak için kullanılabilir. Ancak görselleştirme türüne göre farklı olabilir ve zorunlu değildir.
+  * Görselleştirme Türleri için **kwargs Parametreleri:
+    * Çizgi Grafiği (gorsel_turu == '1'):
+      * `linewidth` (float, varsayılan 1.5): Çizgi kalınlığı.
+    * Korelasyon Isı Matrisi (gorsel_turu == '2'):
+      * `cmap` (str, varsayılan 'coolwarm'): Renk haritası.
+      * `vmin` (float, varsayılan -1): Renk haritasındaki en küçük değer.
+      * `vmax` (float, varsayılan 1): Renk haritasindaki en büyük değer.
+    * Dağılım Matrisi (gorsel_turu == '3'):
+      * `alpha` (float, varsayılan 0.5): Nokta şeffaflığı.
 
-### Donen Deger
+### Dönen Değer
 
-* `veri_cek` fonksiyonu bir pandas DataFrame dondurur.
-* `veri_gorsel` fonksiyonu, pandas DataFrame icerisindeki verileri grafikler ve gorsel ogelerle temsil eder.
+* `veri_cek` fonksiyonu bir pandas DataFrame döndürür.
+* `veri_gorsel` fonksiyonu, pandas DataFrame içerisindeki verileri grafikler ve görsel öğelerle temsil eder.
 
 ## Notlar
 
-* Kutuphane, Is Yatirim'in web sitesindeki verilere bagimlidir. Bu nedenle, verilerin dogrulugu ve surekliligi icin lutfen ilgili web sitesini kontrol edin: [Is Yatirim](https://www.isyatirim.com.tr/tr-tr/Sayfalar/default.aspx)
-* Kutuphanenin gelistirilmesi ve iyilestirilmesi icin geri bildirimlerinizi bekliyorum. GitHub reposuna katkida bulunun: [GitHub Repo](https://github.com/urazakgul/isyatirimhisse)
-* Herhangi bir sorun veya oneride lutfen GitHub reposundaki "Issue" bolumunden yeni bir konu acarak bildirim saglayin: [GitHub Issues](https://github.com/urazakgul/isyatirimhisse/issues)
+* Kütüphane, İş Yatırım'ın web sitesindeki verilere bağımlıdır. Bu nedenle, verilerin doğruluğu ve sürekliliği için lütfen ilgili web sitesini kontrol edin: [İş Yatırım](https://www.isyatirim.com.tr/tr-tr/Sayfalar/default.aspx)
+* Kütüphanenin geliştirilmesi ve iyileştirilmesi için geri bildirimlerinizi bekliyorum. GitHub reposuna katkıda bulunun: [GitHub Repo](https://github.com/urazakgul/isyatirimhisse)
+* Herhangi bir sorun veya öneride lütfen GitHub reposundaki "Issue" bölümünden yeni bir konu açarak bildirim sağlayın: [GitHub Issues](https://github.com/urazakgul/isyatirimhisse/issues)
 
-## Degisiklikler
+## Değişiklikler
 
 ### v0.1.0 - 25/07/2023
 
-* Ilk surum yayinlandi.
+* İlk sürüm yayınlandı.
 
 ### v0.1.1 - 27/07/2023
 
-* `veri_cek` fonksiyonundaki parametreleri kontrol eden kosul ifadeleri guncellendi.
-* `json` kutuphanesi kaldirildi.
-* `veri_cek` fonksiyonuna `200` HTTP kodu kosul ile beraber eklendi ve takibe alindi.
+* `veri_cek` fonksiyonundaki parametreleri kontrol eden koşul ifadeleri güncellendi.
+* `json` kütüphanesi kaldırıldı.
+* `veri_cek` fonksiyonuna `200` HTTP kodu koşul ile beraber eklendi ve takibe alındı.
 
 ### v0.2.0 - 30/07/2023
 
-* `veri_gorsel` fonksiyonu eklendi. Fonksiyon, 3 farkli veri turunde gorsellestirme yapma imkani sunuyor.
+* `veri_gorsel` fonksiyonu eklendi. Fonksiyon, 3 farklı veri türünde görselleştirme yapma imkanı sunuyor.
 * `veri_cek` fonksiyonuna pandas DataFrame'i excel olarak kaydedecek parametreler eklendi.
 
+### v0.2.1 - 31/07/2023
+
+* 0.2.0 sürümündeki kurulum hatası giderildi.
+* Dokümantasyondaki Türkçe karakter problemi giderildi.
+* Dokümantasyonda görünmeyen görseller görünür hale getirildi.
+
 ## Lisans
 
-Bu proje MIT Lisansi altinda lisanslanmistir.
+Bu proje MIT Lisansı altında lisanslanmıştır.
 
-## Katkida Bulunanlar
+## Katkıda Bulunanlar
 
-- [Sinan Erdinc](https://github.com/sinanerdinc)
+- [Sinan Erdinç](https://github.com/sinanerdinc)
```

### Comparing `isyatirimhisse-0.2.0/setup.py` & `isyatirimhisse-0.2.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from setuptools import setup, find_packages
 
+with open("README.md", "r", encoding = "utf-8") as fh:
+    long_description = fh.read()
+
 setup(
     name="isyatirimhisse",
-    version="0.2.0",
+    version="0.2.1",
     packages=find_packages(),
     author="Uraz Akgül",
     author_email="urazdev@gmail.com",
     description="İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştıran ve isteğe göre özelleştirilebilen bir kütüphane.",
-    long_description=open('README.md').read(),
+    long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/urazakgul/isyatirimhisse",
     license="MIT",
     install_requires=[
         "requests",
         "pandas",
         "numpy",
         "matplotlib",
         "seaborn",
-        "os",
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires=">=3.8",
```

### Comparing `isyatirimhisse-0.2.0/tests/test_veri_cek.py` & `isyatirimhisse-0.2.1/tests/test_veri_cek.py`

 * *Files identical despite different names*

### Comparing `isyatirimhisse-0.2.0/tests/test_veri_gorsel.py` & `isyatirimhisse-0.2.1/tests/test_veri_gorsel.py`

 * *Files identical despite different names*

