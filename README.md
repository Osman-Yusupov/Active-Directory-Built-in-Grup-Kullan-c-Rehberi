# 🔐 Active Directory Built-in Grup & Kullanıcı Rehberi

<!-- Shields.io badges -->
![Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![Offline Ready](https://img.shields.io/badge/offline-ready-brightgreen)
![Responsive](https://img.shields.io/badge/responsive-yes-success)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)

> **Tek bir HTML dosyası ile Active Directory'nin tüm varsayılan kullanıcı ve gruplarının yetkilerini anında görüntüleyin, filtreleyin ve güvenlik risklerini öğrenin. İnternet bağlantısı gerektirmez, her cihazda çalışır.**


## ✨ Özellikler

| 🔍 Özellik | Açıklama |
|----------|-----------|
| **Anlık Arama** | İsim veya açıklama üzerinde anında filtreleme |
| **Tür Bazlı Filtre** | `User`, `Domain Local`, `Global`, `Universal` gruplarını tek tıkla listeleme |
| **Karanlık / Aydınlık Mod** | Göz yorgunluğunu azaltan tema desteği |
| **Mobil Uyumlu** | Telefon, tablet, masaüstü fark etmeksizin kusursuz görünüm |
| **Offline Çalışma** | İnternet bağlantısı olmadan, herhangi bir sunucuya ihtiyaç duymadan kullanım |
| **Güvenlik Uyarıları Paneli** | Yüksek riskli grup ve hesaplar için özel uyarı alanı |
| **Yazdırılabilir** | Doğrudan yazıcı çıktısı alarak fiziksel referans kartı oluşturma |
| **Açık Kaynak** | MIT lisansı ile özgürce kullanın, değiştirin ve paylaşın |

---

## 🎯 Neden Bu Araç?

Active Directory yönetimi sırasında **"Bu grup hangi yetkiye sahipti?"** sorusu sıkça sorulur. Microsoft'un resmi dokümantasyonuna her an ulaşamayabilirsiniz veya internete bağlı olmayabilirsiniz. Bu araç sayesinde:

- 🧠 Tüm Built-in kullanıcı ve grupların açıklamaları tek bir yerde
- ⏱️ Saniyeler içinde ihtiyacınız olan bilgiye ulaşma
- 🔒 Kritik gruplar için ek güvenlik notları ile riskleri hızlıca fark etme
- 📱 Mobil cihazınızdan dahi sunucu odasında referans alma

imkanına sahip olursunuz. **Özellikle sistem yöneticileri, SOC analistleri, BT destek ekipleri ve AD'ye yeni başlayanlar için biçilmiş kaftandır.**


## 🧩 Desteklenen Grup Türleri

| Tür | Badge | Açıklama |
|------|-------|-----------|
| **User** | `USER` | Varsayılan kullanıcı hesapları (Administrator, Guest vb.) |
| **Domain Local** | `DOMAIN LOCAL` | Etki alanı içerisinde kaynaklara erişim için kullanılan gruplar |
| **Global** | `GLOBAL` | Orman genelinde kullanıcıları gruplandırmak için kullanılan gruplar |
| **Universal** | `UNIVERSAL` | Orman içindeki tüm etki alanlarında geçerli en geniş kapsamlı gruplar |

---

## ⚠️ Kritik Gruplar ve Güvenlik Uyarıları

Uygulama içerisinde aşağıdaki yüksek riskli gruplar için özel bir uyarı paneli bulunur. Bu grupların üyelikleri sıkı denetlenmelidir.

| Grup Adı | Risk Seviyesi | Öneri |
|----------|:------------:|-------|
| **Schema Admins** | 🔴 Kritik | Sadece şema değişikliği sırasında üye eklenmeli, hemen geri alınmalı |
| **Enterprise Admins** | 🔴 Kritik | Kalıcı üye bulundurulmamalı, gün bazlı erişim verilmeli |
| **Domain Admins** | 🔴 Kritik | Üye sayısı minimumda tutulmalı, geçici üyelik tercih edilmeli |
| **Guest** | 🟡 Uyarı | Devre dışı bırakılmalı, kullanılmamalı |
| **DefaultAccount** | 🟡 Uyarı | Normal koşullarda devre dışı bırakılmalı |
| **Pre-Windows 2000 Compatible Access** | 🟡 Uyarı | Modern ortamlarda boş bırakılmalı, anonim erişime izin vermemeli |

---

## 🚀 Hızlı Başlangıç

1. **Depoyu klonlayın** veya ZIP olarak indirin.
   ```bash
   git clone https://github.com/Osman-Yusupov/active-directory-group-guide.git
