# HEARTBEAT.md - Periodic Tasks

## Memory Backup to GitHub
- อ่าน memory/heartbeat-state.json เช็คว่า backup ครั้งล่าสุดเมื่อไหร่
- ถ้าเกิน 1 ชั่วโมง → backup ขึ้น GitHub
- รันคำสั่ง:
  1. git add memory/ MEMORY.md AGENTS.md SOUL.md USER.md IDENTITY.md TOOLS.md
  2. git commit -m "auto: memory backup $(date)"
  3. git push origin master

ถ้าไม่มีอะไรต้องทำ → HEARTBEAT_OK
