# Landing Page Referral Manus AI - สรุปโปรเจค

## ข้อมูลโปรเจค

**ชื่อโปรเจค:** Landing Page Referral Manus AI By Gemini  
**Domain:** manus-flow.com  
**วันที่สร้าง:** 9 มกราคม 2026  
**สถานะ:** ✅ Deploy สำเร็จและพร้อมใช้งาน  
**ภาษาปัจจุบัน:** 🇺🇸 English (อังกฤษ)

---

## URLs ที่เกี่ยวข้อง

### เว็บไซต์ที่ใช้งานได้

#### 🇺🇸 English (Default)
- 🌐 **https://manus-flow.com** (Primary Domain)
- 🌐 **https://www.manus-flow.com**

#### 🇹🇭 Thai (ไทย)
- 🌐 **https://manus-flow.com/th**
- 🌐 **https://www.manus-flow.com/th**

#### 🇻🇳 Vietnamese (Tiếng Việt)
- 🌐 **https://manus-flow.com/vn**
- 🌐 **https://www.manus-flow.com/vn**

#### Cloudflare Pages URL
- 🌐 **https://manus-flow-landing.pages.dev**

### Repository & Dashboard
- 📦 **GitHub Repository:** https://github.com/TuiNui39/Landing-Page-Referral-Manus-AI-By-Gemini
- ⚙️ **Cloudflare Pages Project:** manus-flow-landing
- 🔧 **Cloudflare Dashboard:** https://dash.cloudflare.com/abaa7d21c5de82c2900373a476560297/pages/view/manus-flow-landing

---

## โครงสร้างโปรเจค

```
Landing-Page-Referral-Manus-AI-By-Gemini/
├── index.html              # Landing page หลัก (ภาษาปัจจุบัน)
├── versions/               # โฟลเดอร์สำหรับเก็บ backup ทุกภาษา
│   ├── README.md          # คู่มือการใช้งานหลายภาษา
│   ├── th/                # 🇹🇭 Thai Version
│   │   └── index.html
│   ├── en/                # 🇺🇸 English Version (Active)
│   │   └── index.html
│   └── vi/                # 🇻🇳 Vietnamese Version
│       └── index.html
├── README.md               # คำอธิบายโปรเจค
├── wrangler.toml          # Cloudflare Wrangler configuration
├── .gitignore             # Git ignore rules
└── PROJECT_SUMMARY.md     # เอกสารสรุปนี้
```

---

## ภาษาที่รองรับ

### 🇹🇭 Thai (ไทย)
- **Path:** `versions/th/index.html`
- **Status:** ✅ Backed up
- **Last Updated:** 2026-01-09
- **Description:** เวอร์ชันภาษาไทยต้นฉบับ

### 🇺🇸 English (อังกฤษ)
- **Path:** `versions/en/index.html`
- **Status:** ✅ Active (Deployed)
- **Last Updated:** 2026-01-09
- **Description:** เวอร์ชันภาษาอังกฤษที่กำลังใช้งานอยู่

### 🇻🇳 Vietnamese (Tiếng Việt)
- **Path:** `versions/vi/index.html`
- **Status:** ✅ Backed up
- **Last Updated:** 2026-01-09
- **Description:** เวอร์ชันภาษาเวียดนาม

---

## การสลับภาษา

### วิธีเปลี่ยนเป็นภาษาไทย

```bash
cd /home/ubuntu/manus-flow-landing
cp versions/th/index.html index.html
git add index.html
git commit -m "Switch to Thai version"
git push origin main
wrangler pages deploy . --project-name=manus-flow-landing
```

### วิธีเปลี่ยนเป็นภาษาอังกฤษ

```bash
cd /home/ubuntu/manus-flow-landing
cp versions/en/index.html index.html
git add index.html
git commit -m "Switch to English version"
git push origin main
wrangler pages deploy . --project-name=manus-flow-landing
```

### วิธีเพิ่มภาษาใหม่

1. สร้างโฟลเดอร์ใหม่: `versions/{language_code}/`
2. คัดลอกและแปล `index.html`
3. บันทึกไฟล์: `versions/{language_code}/index.html`
4. Commit และ Push ขึ้น GitHub
5. Deploy เมื่อต้องการใช้งาน

**ตัวอย่าง Languag- `th` - Thai (ไทย)
- `en` - English (อังกฤษ)
- `vi` - Vietnamese (Tiếng Việt)
- `zh` - Chinese (中文)
- `ja` - Japanese (日本語)
- `ko` - Korean (한국어)
- `es` - Spanish (Español)
- `fr` - French (Français)
- `de` - German (Deutsch)โลジีที่ใช้

- **Frontend:** HTML5, Tailwind CSS (via CDN), JavaScript
- **Icons:** Lucide Icons
- **Fonts:** Google Fonts (Inter - for English, Inter + Noto Sans Thai - for Thai)
- **Hosting:** Cloudflare Pages
- **DNS:** Cloudflare DNS
- **SSL/TLS:** Cloudflare Universal SSL
- **Version Control:** GitHub

---

## ฟีเจอร์หลัก

### 1. Landing Page Design
- ✨ Modern Dark Theme ที่เหมาะกับ AI Products
- 📱 Responsive Design รองรับทุก Device
- 🎨 Glass Morphism UI Effects
- ⚡ Fast Loading (Static HTML)
- 🌍 Multi-language Support (Thai, English, และเพิ่มเติมได้)

### 2. Content Sections (English Version)
- **Hero Section:** CTA for claiming 1,000 free credits
- **Use Cases:** Examples (Deep Research, Coding, Data Analysis, Image Gen)
- **Benefits Grid:** Exclusive benefits (Welcome Bonus, Daily Refill, Full Access)
- **How to Claim:** 3 simple steps
- **FAQ Section:** Frequently asked questions
- **Footer:** Contact info and social links

### 3. Referral Integration
- 🔗 **Referral Link:** https://manus.im/invitation/U9VNR08GX2MX
- 🎯 CTA buttons open referral link in new tab
- 📋 Copy link functionality with modal confirmation

---

## DNS Configuration

### DNS Records (Cloudflare)

| Type | Name | Content | Proxy | Status |
|------|------|---------|-------|--------|
| CNAME | @ | manus-flow-landing.pages.dev | ☁️ Proxied | ✅ Active |
| CNAME | www | manus-flow-landing.pages.dev | ☁️ Proxied | ✅ Active |

### Nameservers
- emely.ns.cloudflare.com
- trace.ns.cloudflare.com

---

## Custom Domains Status

### manus-flow.com
- **Status:** ✅ Active
- **Verification:** ✅ Active
- **SSL Certificate:** ✅ Active (Google Trust Services)
- **Created:** 2026-01-09 08:38:11 UTC

### www.manus-flow.com
- **Status:** ✅ Active
- **Verification:** ✅ Active
- **SSL Certificate:** ✅ Active (Google Trust Services)
- **Created:** 2026-01-09 08:38:23 UTC

---

## การ Deploy

### ขั้นตอนที่ทำแล้ว

1. ✅ สร้าง GitHub Repository
2. ✅ Push โค้ดขึ้น GitHub
3. ✅ ติดตั้ง Wrangler CLI
4. ✅ สร้าง Cloudflare Pages Project
5. ✅ Deploy ไฟล์ไป Cloudflare Pages
6. ✅ เพิ่ม Custom Domain (manus-flow.com, www.manus-flow.com)
7. ✅ ตั้งค่า DNS Records
8. ✅ SSL Certificate Provisioning สำเร็จ
9. ✅ สร้างโครงสร้างไฟล์สำหรับหลายภาษา
10. ✅ Backup โค้ดภาษาไทย
11. ✅ Deploy โค้ดภาษาอังกฤษ

### คำสั่งที่ใช้

```bash
# Deploy to Cloudflare Pages
wrangler pages deploy . --project-name=manus-flow-landing

# Add Custom Domains (via API)
curl -X POST "https://api.cloudflare.com/client/v4/accounts/{account_id}/pages/projects/manus-flow-landing/domains" \
  -H "Authorization: Bearer {api_token}" \
  -H "Content-Type: application/json" \
  --data '{"name":"manus-flow.com"}'
```

---

## การอัปเดตในอนาคต

### วิธีอัปเดตเว็บไซต์

1. แก้ไขไฟล์ `index.html` ใน local (หรือแก้ไขใน `versions/{lang}/index.html`)
2. Commit และ Push ขึ้น GitHub:
   ```bash
   git add .
   git commit -m "Update landing page"
   git push origin main
   ```
3. Deploy ใหม่ด้วย Wrangler:
   ```bash
   wrangler pages deploy . --project-name=manus-flow-landing
   ```

หรือเชื่อม GitHub กับ Cloudflare Pages เพื่อ Auto-deploy:
- ไปที่ Cloudflare Pages Dashboard
- เลือก Settings > Builds & deployments
- เชื่อม GitHub Repository
- ทุกครั้งที่ Push จะ Deploy อัตโนมัติ

---

## ข้อมูล Account

### Cloudflare Account
- **Email:** tuinuiete39@gmail.com
- **Account ID:** abaa7d21c5de82c2900373a476560297
- **Zone ID:** 67db372602850b5d4b7b8a57392558c8
- **Plan:** Free Website

### GitHub Account
- **Username:** TuiNui39
- **Repository:** Landing-Page-Referral-Manus-AI-By-Gemini

---

## หมายเหตุสำคัญ

### Multi-language Management
- ไฟล์ภาษาทั้งหมดถูก backup ไว้ใน `versions/` directory
- เปลี่ยนภาษาได้โดยคัดลอกไฟล์จาก `versions/{lang}/index.html` มาเป็น `index.html`
- แนะนำให้แก้ไขไฟล์ใน `versions/` ก่อน แล้วค่อยคัดลอกมา deploy

### SSL Certificate
- SSL Certificate ทั้ง 2 domains พร้อมใช้งานแล้ว
- ตรวจสอบสถานะได้ที่ Cloudflare Pages > Custom domains

### API Token Security
- API Token ที่ใช้: `vmkwPrl0rGCBuN4iunBME5xDMblmY3-Is-DPW4vP`
- **แนะนำ:** ลบ Token นี้หลังจาก Deploy เสร็จแล้ว
- สร้าง Token ใหม่ได้ที่: https://dash.cloudflare.com/profile/api-tokens

### Backup
- โค้ดทั้งหมดถูก backup บน GitHub แล้ว
- โค้ดภาษาไทยถูก backup ไว้ที่ `versions/th/index.html`
- โค้ดภาษาอังกฤษถูก backup ไว้ที่ `versions/en/index.html`
- สามารถ Clone repository ได้ทุกเมื่อ:
  ```bash
  git clone https://github.com/TuiNui39/Landing-Page-Referral-Manus-AI-By-Gemini.git
  ```

---

## การแก้ปัญหา

### Error 522 (Connection Timed Out)
- **สาเหตุ:** Custom Domain ยังไม่ได้ verify หรือ SSL ยังไม่พร้อม
- **วิธีแก้:** รอ 5-15 นาที หรือตรวจสอบ DNS Records

### ไม่สามารถเข้าเว็บได้
1. ตรวจสอบ DNS Records ใน Cloudflare Dashboard
2. ตรวจสอบสถานะ Custom Domain ใน Pages Project
3. ลอง Clear DNS Cache: `ipconfig /flushdns` (Windows) หรือ `sudo dscacheutil -flushcache` (Mac)

### ต้องการเปลี่ยน Referral Link
- แก้ไขไฟล์ `index.html` ในส่วน JavaScript:
  ```javascript
  const referralLink = "https://manus.im/invitation/YOUR_NEW_CODE";
  ```
- หรือค้นหา `U9VNR08GX2MX` และแทนที่ด้วยรหัสใหม่

### ต้องการเปลี่ยนภาษา
- ดูคู่มือในส่วน "การสลับภาษา" ด้านบน
- หรืออ่านไฟล์ `versions/README.md`

---

## Version History

| Version | Date | Language | Changes |
|---------|------|----------|---------|
| 1.0.0 | 2026-01-09 | 🇹🇭 Thai | Initial Thai version |
| 1.1.0 | 2026-01-09 | 🇺🇸 English | Added English version, multi-language structure |
| 1.2.0 | 2026-01-09 | 🇻🇳 Vietnamese | Added Vietnamese version backup |
| 1.3.0 | 2026-01-09 | 🌐 Multi-lang | Added URL routing (/th, /vn) |

---

## ติดต่อ & Support

- **Cloudflare Support:** https://support.cloudflare.com
- **GitHub Issues:** https://github.com/TuiNui39/Landing-Page-Referral-Manus-AI-By-Gemini/issues
- **Manus AI:** https://manus.im

---

**สร้างโดย:** Manus AI Agent  
**วันที่อัปเดตล่าสุด:** 9 มกราคม 2026  
**เวอร์ชัน:** 1.3.0
