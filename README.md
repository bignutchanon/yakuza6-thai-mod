# Yakuza 6: The Song of Life — Thai Translation (ม็อดแปลไทย)

แปลไทย Yakuza 6: The Song of Life (Steam): เนื้อเรื่องหลักทุกบท · ซับคัตซีน · บทสนทนาทั้งเกม (NPC / ซับสตอรี่ / โทรศัพท์ / SNS) · เมนู / UI / ไอเทม / สกิล / แผนที่ · มินิเกม (คาบาเรต์, Clan Creator, ตกปลา, เบสบอล, คาราโอเกะ, ดาร์ท, มาจอง, โชกิ, เกมตู้ ฯลฯ) · ข้อความระบบ talk · รูป UI ที่มีตัวหนังสือ + โลโก้หน้าแรก + ป้ายในคัตซีนเป็นไทย · ฟอนต์ไทยฝังในตัว (สระซ้อน/วรรณยุกต์ครบ) · ช่องไฟตัวอักษรไทยแบบสัดส่วน

Thai localization for Yakuza 6: The Song of Life (Steam): full main story, cutscene subtitles, every dialogue script (NPC, substories, phone, SNS), menus/UI/items/skills/map, minigames, the talk system, Thai UI images / title logo / cutscene captions, an embedded Thai font with proper vowel/tone stacking, and proportional Thai glyph spacing. The game executable is never modified.

## ดาวน์โหลด / Download

ไปที่หน้า [Releases](../../releases/latest) → `Yakuza6-Thai-v1.5.zip` (ไฟล์เดียว มีตัวติดตั้ง + ตัวถอน)

## ภาษาเกมใน Steam: English หรือ 日本語 ก็ได้ (ตั้งแต่ v1.5)

ม็อดใช้ชุดข้อมูลญี่ปุ่นของเกม (โหมดอังกฤษวาดตัวหนังสือจากรูปภาพที่ใส่ไทยไม่ได้) — `dinput8.dll` บอกเกมให้โหลดชุดนั้นเองไม่ว่า Steam จะตั้งภาษาอะไร และรูป UI ถูกเปลี่ยนเป็นไทย/อังกฤษ ในเกมไม่มีญี่ปุ่นโผล่
ถ้าลบ `dinput8.dll` ออก ต้องตั้ง Steam → คลิกขวาเกม → Properties → Language → **Japanese / 日本語** เอง ไม่งั้นเกมจะไม่ขึ้นภาษาไทย

**English:** any Steam language works — `dinput8.dll` makes the game load its Japanese data set, which carries the Thai text. Without `dinput8.dll`, set the game language to **Japanese** yourself.

## การติดตั้ง / Installation

1. ปิดเกมให้สนิท แล้วแตก zip ออกมาก่อน (คลิกขวา → Extract All) อย่าเปิดไฟล์ข้างในตอนยังอยู่ใน zip
2. ดับเบิลคลิก `ติดตั้ง.bat` — หาโฟลเดอร์เกมเอง สำรองไฟล์เดิม แล้วติดตั้ง 7 ขั้น
   ขั้นประกอบรูป UI (~800 MB), talk (~360 MB) และคัตซีน (~530 MB) ใช้เวลารวม ~10 นาที **อย่าปิดหน้าต่าง** · ต้องมีที่ว่างในไดรฟ์เกม ~4 GB
3. เปิดเกม

ถ้า Windows เตือน "Windows protected your PC" ให้กด More info → Run anyway (ไฟล์ .bat ไม่ได้เซ็นชื่อ)

**แบบวางทับเอง (ไม่รัน .bat):** ก๊อปโฟลเดอร์ `data` และไฟล์ `dinput8.dll` ไปวางทับในโฟลเดอร์เกม (`...\steamapps\common\Yakuza 6 - The Song of Life\`) → Replace
ได้ข้อความไทยส่วนหลัก + ช่องไฟ แต่รูป UI (เมนูมือถือ, ป้ายมินิเกม ฯลฯ) จะยังเป็นญี่ปุ่น และข้อความระบบ talk (ตัวเลือกสนทนา/prompt มินิเกม/บาร์สแน็ค) กับป้ายในคัตซีนยังไม่เป็นไทย — สามส่วนนี้ต้องติดตั้งผ่าน `ติดตั้ง.bat`

**English:** extract the zip and run `ติดตั้ง.bat` (install) — it finds the game, backs up every file it touches, and verifies the copy. Manual alternative: drop the `data` folder and `dinput8.dll` onto the game folder (main text + spacing only; UI images, cutscene captions and the talk system need the installer).

## การถอน / Uninstall

- `ถอนการติดตั้ง.bat` — คืนไฟล์ที่สำรองไว้ตอนติดตั้ง + ลบ `dinput8.dll`
- หรือ Steam → Properties → Installed Files → Verify integrity แล้วลบ `dinput8.dll` ในโฟลเดอร์เกมเอง (Steam ไม่ลบให้ เพราะไม่ใช่ไฟล์ของเกม)
- อยากปิดเฉพาะตัวแก้ช่องไฟ: ลบ `dinput8.dll` อย่างเดียว ข้อความไทยยังอยู่

## ตัวแก้ช่องไฟ (`dinput8.dll`)

เกมจัดตัวอักษรทุกตัวที่ไม่ใช่อังกฤษให้กว้างเท่าคันจิ ตัวไทยเลยห่างเป็นช่องๆ และบางเมนูล้น/ทับกัน `dinput8.dll` แก้ค่าช่องไฟในหน่วยความจำเฉพาะตอนเกมเปิด ให้ตัวไทยแต่ละตัวกินที่ตามความกว้างจริง ไม่แก้ไฟล์ exe หรือไฟล์เกม อังกฤษ/ตัวเลข/ญี่ปุ่นไม่ถูกแตะ

ระหว่างเล่น: **F3** เปิด/ปิดเทียบดู · **F1 / F2** แน่น/หลวมทีละ 5% · **F4** คืนค่าเริ่มต้น

## ส่วนที่ยังเป็นอังกฤษ — ตั้งใจ ไม่ใช่ติดตั้งไม่ครบ

- หน้าเครดิต · ข้อตกลงลิขสิทธิ์ (EULA)
- ภาพหน้าจอสอนเล่น · เนื้อเพลง/ชื่อเพลงคาราโอเกะ · โลโก้แบรนด์
- ป้ายร้าน/ป้ายจราจรในฉาก 3D (ตามต้นฉบับ)
- ข้อความบางจุดที่เกมไม่มีช่องให้แทน เช่น ป้ายบางอันบนโต๊ะรูเล็ต

## หมายเหตุ / Notes

- ใช้กับ Yakuza 6: The Song of Life ของ Steam เท่านั้น
- `dinput8.dll` และ `ParTool.exe` (ตัวประกอบไฟล์ UI/talk/คัตซีนในตัวติดตั้ง) อาจโดนแอนตี้ไวรัสเตือน = false positive · ถ้าไม่สบายใจใช้วิธีวางทับเองได้ (ไม่ต้องรัน .exe/.bat)
- Steam อัปเดตเกม / Verify integrity = ไฟล์แปลหาย ต้องลงใหม่
- ม็อดทำโดยแฟนเกม ไม่เกี่ยวข้องกับ SEGA / Ryu Ga Gotoku Studio · ต้องมีเกมแท้ · แจกฟรี ห้ามนำไปขาย ห้ามอัปโหลดต่อที่อื่น
- แจ้งคำแปลผิด/บั๊กที่ [Issues](../../issues)

## มีอะไรในซิป

| ไฟล์ | คือ |
|---|---|
| `ติดตั้ง.bat` / `ถอนการติดตั้ง.bat` | ตัวติดตั้ง/ตัวถอน (เรียก `_install.ps1` / `_uninstall.ps1`) |
| `data\font.par` | ฟอนต์ไทย |
| `data\db\ja\*.bin` (210 ไฟล์) | ข้อความแปลทั้งเกม |
| `dinput8.dll` | ตัวแก้ช่องไฟตัวอักษรไทย + ให้เกมโหลดชุดข้อความไทย (เกมโหลดเอง) |
| `_ui_en\` | รูป UI 819 รูป (ไทย 225 · อังกฤษแทนญี่ปุ่น 594) + `ParTool.exe` สำหรับประกอบเข้า `ui.par` ของคุณเอง |
| `_talk_th\` | ข้อความไทยระบบ talk 595 ไฟล์ย่อย สำหรับประกอบเข้า `talk.par` |
| `_auth_th\` | ป้ายไทยในคัตซีน 21 ฉาก สำหรับประกอบเข้าไฟล์คัตซีนภาษาอังกฤษของเกม |

## เครดิต

เครื่องมือ: ParTool (Kaplas) · ฟอนต์ไทย: Sarabun (Cadson Demak) · ฟอนต์ในรูป UI/โลโก้/ป้าย: Kanit, Sriracha, Pattaya, Noto Sans Thai, Taviraj — SIL Open Font License
