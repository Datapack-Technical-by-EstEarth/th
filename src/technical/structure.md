# โครงสร้างไฟล์ดาต้าแพ็ค

## เกี่ยวกับ

สำหรับแสดงตัวอย่างหนึ่งในโครงสร้างไฟล์ดาต้าแพ็คที่สวยงาม เป็นระเบียบ จัดกลุ่มได้ง่าย ง่ายต่อการอ่าน พัฒนา และ ซ่อมบำรุง

## ตัวอย่างที่เป็นไปได้ในแต่ละกรณี

### ดาต้าแพ็คหลายชุด

```
data
 ├ <เนมสเปซ: ชื่อผู้สร้าง, ชื่อทีม>
 │    ├ advancements
 │    │   ├ <ชื่อดาต้าแพค>
 │    │   │   ├ <event>
 │    │   │   │   ╰ <player_hurt_entity>.json
 │    │   │   ╰ <place>
 │    │   │       ╰ <place_block>.json
 │    │   ╰ <ชื่อดาต้าแพค>.json
 │    ├ functions
 │    │   ├ <ชื่อดาต้าแพค>
 │    │   │   ├ <กลุ่มโฟลเดอร์ฟังก์ชั่น>
 │    │   │   ├ main.mcfunction (เริ่ม loop*3)
 │    │   │   ├ setup.mcfunction (รัน load*3)
 │    │   │   ╰ uninstall.function
 │    │   ╰ <database, random & อื่นๆ>
 │    ├ loot_tables
 │    │   ╰ <ชื่อดาต้าแพค>
 │    │       ╰ <กลุ่มโฟลเดอร์รูทเช่น item, block>
 │    │           ╰ <...>.json
 │    ├ predicates
 │    │   ╰ <ชื่อดาต้าแพค>
 │    │       ├ <กลุ่มโฟลเดอร์ predicate>
 │    │       ╰ <...>.json
 │    ├ recipes
 │    │   ╰ <ชื่อดาต้าแพค>
 │    │       ╰ <...>.json
 │    ╰ tags
 │        ├ <items>
 │        │   ╰ <ชื่อดาต้าแพค>
 │        │       ╰ <...>.json
 │        ╰ <functions>
 │            ╰ <ชื่อดาต้าแพค>
 │                ├ load.json*2
 │                ╰ loop.json*2
 ├ <โกลบอล>
 │    ╰ advancements
 │        ├ <เนมสเปซ>.json
 │        ╰ root.json
 ╰ <ไมน์คราฟต์>
      ╰ tags
          ╰ <functions>
              ├ load.json*1
              ╰ tick.json*1
```

### ดาต้าแพ็คชุดเดียว