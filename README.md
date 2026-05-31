# License Tracker (GitHub Pages)

หน้าเว็บสถิตินี้โหลด UI จาก GitHub Pages และเรียก API ผ่าน Google Apps Script (GAS)

## URL

หลังเปิด GitHub Pages แล้วเข้าใช้งานที่:

`https://pongvitsam.github.io/License_Tracker_GAS/`

## ตั้งค่า

1. แก้ไข `config.js` — ใส่ URL `/exec` ของ Web App deploy ล่าสุดจาก GAS
2. ใน GAS ต้อง `clasp push` และ **Deploy → New deployment → Web app** (Anyone) หลังอัปเดต RpcDispatch
3. GitHub → Settings → Pages → Branch `main` / folder `/` (root)

## Build ใหม่จาก PK.2

```bash
cd C:\Users\User\Desktop\PK.2
npm run build:ghpages
git -C ..\License_Tracker_GAS add -A && git commit -m "Update gh-pages" && git push
```

Build stamp: 2026-05-31T16:00:00+07:00-tiered-load
