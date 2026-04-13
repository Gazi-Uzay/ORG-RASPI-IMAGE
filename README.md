# 🚀 Raspberry Pi Remote Development (VS Code + SSH)

Bu doküman, Raspberry Pi (Ubuntu Server) üzerine **VS Code Remote-SSH** ile bağlanmayı anlatır.

---

## 📦 Image Bilgisi

**Repo:** ORG-2026-Raspi-Image  

---

## 📡 Bağlantı Bilgileri

- **User:** ubuntu  
- **Password:** gaziuzay  

> ⚠️ **ÖNEMLİ:** Raspberry Pi'nin IP adresi her zaman aynı olmayabilir.  
> Router yeniden başlatıldığında veya Wi-Fi değiştiğinde IP değişebilir.

---

## 🔍 IP Adresini Nasıl Öğrenirim?

Raspberry Pi üzerinde:

```bash
hostname -I
```

Örnek çıktı:
```bash
192.168.1.106
```

👉 Bu IP'yi kullanarak bağlanacaksın.

---

## 🌐 Alternatif: Router Üzerinden Bulma

- Modem arayüzüne gir (genelde `192.168.1.1`)
- "Bağlı Cihazlar" listesine bak
- `raspberrypi` veya `ubuntu` cihazını bul

---

## 🔧 IP Sabitleme (Önerilir)

### 1. Router üzerinden
- DHCP Reservation / Static IP ayarla

---

## 🔌 VS Code ile Bağlantı

1. VS Code aç  
2. `Ctrl + Shift + P`  
3. `Remote-SSH: Connect to Host`  
4. Şunu yaz:

```bash
ubuntu@<IP_ADRESI>
```

Örnek:
```bash
ubuntu@192.168.1.106
```

---

## ⚠️ Bağlantı Sorunu Çözümü

1. `Ctrl + Shift + P`  
2. `Remote-SSH: Kill VS Code Server on Host`  
3. Tekrar bağlan  

---

## 📶 Dahili Wi-Fi Ayarları (Image İçinde Hazır)

Bu image içerisinde aşağıdaki Wi-Fi ağları tanımlıdır:

```yaml
- SSID: GAZIUZAY
  PASSWORD: guzay123

- SSID: VEGA
  PASSWORD: dN3ebu7eU9Da
```

> ⚠️ Notlar:
> - Büyük/küçük harf duyarlıdır  
> - Raspberry Pi otomatik olarak uygun ağa bağlanır  
> - Bağlanamazsa diğer kayıtlı ağa geçer  

---

## 📜 Versiyonlar

### 🔹 v1.0.0

👉 Image indir:
```
[DRIVE LINK BURAYA]
```

**İçerik:**
- Ubuntu Server  
- ROS Noetic  
- MAVROS kurulu  
- SSH aktif  
- VS Code Remote hazır  
- Wi-Fi önceden tanımlı  

---

🔥 Hazırsın!
