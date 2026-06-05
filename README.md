# Java API Test Otomasyon Projesi

Bu depo (repository), **Yazılım Test Mühendisliği** dersi kapsamında geliştirilmiş; **Java**, **Rest-Assured** ve **JUnit 5** teknolojilerini kullanan güçlü ve yapılandırılmış bir API test otomasyon projesidir. Proje, **Apache Maven** derleme yönetimi aracı üzerinde kurgulanmış olup, RESTful API uç noktalarını (endpoints) hızlı, tekrarlanabilir ve ölçeklenebilir şekilde test etmek amacıyla tasarlanmıştır. Projede profesyonel hata yönetimi (exception handling) ve negatif test senaryoları da kapsamlı bir şekilde ele alınmıştır.

---

## 🎓 Akademik Bağlam

Bu proje, Bilgisayar Mühendisliği Bölümü **Yazılım Test Mühendisliği** dersi dönemi/projesi dahilinde, yazılım kalite güvencesi (QA) ve test otomasyonu pratiklerini uygulamalı olarak göstermek amacıyla hazırlanmıştır. Proje; modern yazılım test yaşam döngülerine (STLC), entegrasyon testlerine ve sürekli entegrasyon (CI/CD) süreçlerine tam uyumluluk göstermektedir.

---

## 🚀 Öne Çıkan Özellikler

- **Akıcı API Testleri (Fluent API Testing):** Rest-Assured kullanılarak BDD tarzı (`given-when-then`) temiz ve okunabilir bir yapıda kodlanmıştır.
- **Güçlü Hata Yönetimi:** Dinamik API hata yanıtlarını yakalamak ve derleme (build) sürecini kesintiye uğratmadan konsola loglamak amacıyla `try-catch` blokları ile negatif test senaryoları kurgulanmıştır.
- **Otomatik Yaşam Döngüsü Yönetimi:** Maven Yaşam Döngüsü (Maven Lifecycle) ile tam entegre çalışarak temizleme (clean), derleme (compile) ve test işlemlerini deterministik bir şekilde yürütür.

---

## 🛠️ Teknolojiler ve Bağımlılıklar

- **Programlama Dili:** Java (JDK 8 veya üzeri)
- **Derleme ve Bağımlılık Yönetimi:** Apache Maven (v3.9.x)
- **Test Çatısı:** JUnit Jupiter (JUnit 5)
- **API Test Kütüphanesi:** Rest-Assured
- **Doğrulama Kütüphanesi (Assertions):** Hamcrest Matchers

Gerekli tüm eklenti ve kütüphane bağımlılıkları merkezi `pom.xml` dosyası içerisinde yapılandırılmıştır.

---

## 📂 Proje Yapısı

```text
simple-java-maven-app/
│
├── src/
│   ├── main/
│   │   └── java/            # Uygulama kaynak kodları (varsa)
│   └── test/
│       └── java/            # Otomatize edilmiş test sınıfları
│           └── com/mycompany/app/
│               └── AppTest.java   # Temel REST API test senaryoları
│
├── .vscode/                 # IDE ortam yapılandırma ayarları
├── pom.xml                  # Maven yapılandırmaları, bağımlılıklar ve eklentiler
└── README.md                # Proje dokümantasyonu
