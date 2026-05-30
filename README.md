# 🛒 Alisizm Blackmarket for FiveM

[![Tebex Store](https://img.shields.io/badge/Purchase-Tebex-orange?style=flat-square&logo=tebex)](https://alisizm.tebex.io/package/7436434)
[![Framework](https://img.shields.io/badge/Framework-QBCore%20%7C%20ESX-blue?style=flat-square)](#)
[![YouTube Channel](https://img.shields.io/badge/YouTube-Subscribe-red?style=flat-square&logo=youtube)](https://www.youtube.com/@Alisizmsc)

A dynamic, fully configurable black market system with a modern NUI shop interface, rotating NPC dealers, and robust server-side economy validation.

---

## 🔗 Links
*   **🛒 Purchase:** [Tebex Store](https://alisizm.tebex.io/package/7436434)
*   **📺 YouTube Channel:** [Alisizm Development](https://www.youtube.com/@Alisizmsc)
*   **🛍️ My Store:** [View all scripts](https://alisizm.tebex.io/package/)

---

## 🇬🇧 English Description

### 📖 Overview
Alisizm Blackmarket provides a controlled way to sell illegal or premium items in your RP economy. Players interact with dealer NPCs around the map and purchase items through a modern NUI shop interface. The script supports both **QBCore** and **ESX**, and is extremely easy to customize for your server's needs.

### ✨ Key Features
*   **Dynamic Dealer System:** Dealer NPCs can automatically rotate to different locations on a configurable timer, keeping the black market hidden and dynamic.
*   **Modern NUI Shop UI:** Features category filters, a search bar, a cart system, quantity controls, and a smooth checkout flow.
*   **Dual Payment Methods:** Players can choose to pay via cash or bank account.
*   **Framework Support:** Works seamlessly with both QBCore and ESX (switchable via config).
*   **TextUI Compatibility:** Built-in safe calls for `nation-textui` display/hide exports.
*   **Image Fallback Logic:** Automatically tries multiple inventory image paths (e.g., `qb-inventory`, `ox_inventory`) to ensure item images load correctly.
*   **Server-Side Security:** Robust purchase validation including money checks, item validation, delivery logic, and rollback/refund handling (especially robust in the QBCore flow).

### 🛠️ Technical Flow & Customization
*   **How it works:** A player approaches the NPC, opens the market, builds a cart, and confirms payment. A server callback builds a sanitized order (validating keys, counts, total price, and payment method) before removing funds and granting items.
*   **Configurable via `config.lua`:**
    *   Framework selection (`CAS.Framework`)
    *   Dealer definitions (coordinates, ped hash, display text) and rotating location points (`moveCoords`).
    *   Full item catalog, prices, and categories (`CAS.Items`).
    *   Interaction distance, image base paths, and success notification texts.

### 🚀 Installation Notes
1.  Keep the resource name exactly as `alisizm-blackmarket` (name check is enforced).
2.  Ensure you have the required framework started (`qb-core` for QBCore, `es_extended` for ESX).
3.  Add `ensure alisizm-blackmarket` to your `server.cfg`.

---
---

## 🇹🇷 Türkçe Açıklama

### 📖 Genel Bakış
Alisizm Blackmarket, RP ekonomisinde yasa dışı veya premium ekipman satışını kontrollü bir şekilde yönetmenizi sağlayan dinamik bir kara borsa sistemidir. Oyuncular haritadaki satıcı NPC’leri ile etkileşime girerek NUI market arayüzünden ürün satın alabilir. Hem **QBCore** hem de **ESX** altyapısını destekler.

### ✨ Öne Çıkan Özellikler
*   **Dinamik Satıcı Sistemi:** Satıcı NPC, config üzerinden belirlenen zaman aralıklarıyla otomatik olarak konum değiştirir (Kara borsanın yerinin sürekli değişmesini sağlar).
*   **Modern NUI Market:** Kategori filtreleme, arama çubuğu, sepet sistemi, adet artır/azalt ve toplu ödeme akışı.
*   **Çift Ödeme Yöntemi:** Oyuncular alışverişi nakit veya banka hesabıyla tamamlayabilir.
*   **Framework Desteği:** Konfigürasyon dosyası üzerinden qb ve esx arasında kolayca geçiş yapılabilir.
*   **TextUI Entegrasyonu:** `nation-textui` için uyumlu gösterim/gizleme çağrıları içerir.
*   **Görsel Fallback Sistemi:** Ürün görselleri farklı envanter yollarında otomatik denenir (`qb-inventory`, `ox_inventory` vb.).
*   **Sunucu Tarafı Güvenlik:** Satın alma doğrulaması, bakiye kontrolü, item teslimi ve hatada geri iade/rollback mekanizması ile hileye karşı korumalıdır.

### 🛠️ Çalışma Mantığı ve Konfigürasyon
*   **Nasıl Çalışır:** Oyuncu NPC’ye yaklaşır, marketi açar, sepet oluşturur ve ödemeyi tamamlar. Sunucu (server callback) siparişi normalize eder (item key, count, toplam tutar ve ödeme yöntemi doğrulaması). İşlem başarılıysa para düşer ve item envantere eklenir; başarısızsa iade (rollback) yapılır.
*   **`config.lua` üzerinden ayarlanabilir alanlar:**
    *   Framework seçimi (`CAS.Framework`).
    *   Satıcı konumları, ped modeli, text etiketi ve hareket edecek rotasyon noktaları (`moveCoords`).
    *   Tüm ürünler, fiyatlar, tipler ve kategoriler (`CAS.Items`).
    *   Etkileşim mesafesi, ürün görsel yolları ve bildirim metinleri.

### 🚀 Kurulum Notları
1.  Klasör adı kesinlikle `alisizm-blackmarket` olarak kalmalıdır (script içinde isim doğrulaması mevcuttur).
2.  Kullandığınız framework'ün (`qb-core` veya `es_extended`) kurulu ve çalışır olduğundan emin olun.
3.  `server.cfg` dosyanıza `ensure alisizm-blackmarket` ekleyin.

---

## ⚖️ License Information / Lisans Bilgilendirmesi

### English
**This software is NOT Open Source.** 
"Alisizm Blackmarket" is a commercial product licensed and distributed exclusively via the official Tebex store. This resource is protected by the FiveM Asset Escrow system and copyright laws.

### Terms of Use:
*   **Usage:** By purchasing this resource from the official Tebex store, you are granted a non-exclusive license to use it on your own FiveM server.
*   **Customization:** You are **ALLOWED** to modify the unencrypted configuration file (`config.lua`) to manage items, prices, locations, and settings.
*   **Transfer:** You may transfer the asset license to another Keymaster account using the official transfer feature provided by the Cfx.re Keymaster system. Reselling the asset outside of this official system is strictly prohibited.
*   **Redistribution:** You may **NOT** redistribute, share, publish, resell, or leak any part of this software (including UI files or config) to third parties. Others must acquire their own license via the official Tebex store.

### Tracking & Enforcement:
Hidden cryptographic markers and watermarks are securely embedded within the software files to track unauthorized redistribution and use. If unauthorized distribution, leaking, reselling (external to Keymaster), or claims of false ownership are detected:
An official DMCA takedown notice and copyright complaint will be submitted directly to **Cfx.re (FiveM)** and **Tebex**.
This action will result in the permanent ban of your Keymaster account, the blacklisting of your FiveM server, and the termination of any associated Tebex store.

All copyrights and intellectual property rights belong to **alisizm**.

---

### Türkçe
**Bu yazılım Açık Kaynak (Open Source) DEĞİLDİR.**
"Alisizm Blackmarket", ticari bir üründür ve yalnızca resmi Tebex mağazası üzerinden lisanslanarak dağıtılmaktadır. Bu eklenti, FiveM Asset Escrow sistemi ve telif hakkı yasalarıyla korunmaktadır.

### Kullanım Koşulları:
*   **Kullanım:** Bu ürünü resmi Tebex mağazasından satın alarak, yalnızca kendi FiveM sunucunuzda kullanmak üzere münhasır olmayan bir kullanım hakkı elde edersiniz.
*   **Özelleştirme:** Eşyaları, fiyatları, satıcı konumlarını ve genel ayarları düzenlemek için şifrelenmemiş yapılandırma dosyasını (`config.lua`) düzenlemenize **İZİN VERİLİR**.
*   **Transfer:** Lisansınızı resmi Cfx.re Keymaster sistemi üzerinden başka bir Keymaster hesabına transfer edebilirsiniz. Bu resmi sistem haricinde ürünün üçüncü şahıslara satılması kesinlikle yasaktır.
*   **Dağıtım:** Bu yazılımın herhangi bir parçasını (arayüz dosyaları ve yapılandırma dahil) üçüncü şahıslarla dağıtmak, paylaşmak, yayınlamak, satmak veya sızdırmak **YASAKTIR**. Diğer kullanıcılar kendi lisanslarını resmi Tebex mağazası üzerinden edinmelidir.

### Takip ve Yaptırım:
İzinsiz dağıtımları, kullanımı ve sızıntıları tespit edebilmek amacıyla eklenti dosyalarının içerisine gizlenmiş şifreler ve filigranlar (watermark) yerleştirilmiştir. Yetkisiz dağıtım, sızıntı, satış (Keymaster harici) veya ürünü kendinizinmiş gibi gösterme eylemlerinin tespiti halinde:
Doğrudan **Cfx.re (FiveM)** ve **Tebex** platformlarına resmi telif ihtarı (DMCA) ve şikayet gönderilecektir.
Bu işlem; Keymaster hesabınızın kalıcı olarak yasaklanması, FiveM sunucunuzun kara listeye (blacklist) alınması ve varsa ilişkili Tebex mağazanızın kapatılması ile sonuçlanacaktır.

Tüm telif hakları ve fikri mülkiyet hakları **alisizm**'e aittir.
