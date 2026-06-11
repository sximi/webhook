# 🔔 Webhook

> **Event-Driven HTTP Callback** · กลไกที่ทำให้ระบบพูดคุยกันได้แบบอัตโนมัติ

---

## 📖 Definition

### English — MDN Web Docs
> *"A webhook is a way for an app to provide other applications with real-time information. A webhook delivers data to other applications as it happens, meaning you get data immediately unlike typical APIs where you would need to poll for data very frequently."*

### English — Zapier
> *"Webhooks are automated messages sent from apps when something happens. They have a message — or payload — and are sent to a unique URL, essentially an app's phone number or address."*

### 🇹🇭 Thai — สรุปในสไตล์ของตัวเอง
Webhook คือ **"ระบบโทรบอกอัตโนมัติ"** — แทนที่เราจะต้องคอยถามซ้ำๆ ว่า "มีอะไรใหม่ไหม?" ระบบปลายทางจะโทรหาเราทันทีเมื่อมีเหตุการณ์เกิดขึ้น เช่น มีคนจ่ายเงิน → ระบบแจ้งเราเองเลย ไม่ต้องรอ 🎀

---

## 🔍 Explanation

Webhook ทำงานต่างจาก API แบบปกติ (Polling) ดังนี้

### 🔄 Polling vs Webhook

| รูปแบบ | วิธีการ | ข้อเสีย |
|---|---|---|
| **Polling** | ถามซ้ำทุก X วินาที | เปลืองทรัพยากร |
| **Webhook** | รอให้ระบบโทรมาหา | เร็ว ประหยัด |

### 🛠️ การทำงานของ Webhook

1. **Register** — บอก URL ปลายทางที่ต้องการรับข้อมูล
2. **Event เกิดขึ้น** — เช่น มีการชำระเงิน, มี commit ใหม่
3. **HTTP POST** — ระบบส่ง payload มาที่ URL ที่ลงทะเบียนไว้
4. **Process** — รับข้อมูลและทำงานต่อได้เลย

### 🌍 ตัวอย่างการใช้งานจริง

- **GitHub** — แจ้งเมื่อมี push / pull request
- **Stripe** — แจ้งเมื่อการชำระเงินสำเร็จหรือล้มเหลว
- **LINE Notify** — ส่งข้อความแจ้งเตือนอัตโนมัติ

---

## 🤖 GenAI Explanation

> *"Webhook เปรียบเหมือนการฝากเบอร์โทรไว้กับร้านค้า — แทนที่จะโทรถามซ้ำว่าของมาหรือยัง ร้านจะโทรหาเราเองเมื่อของพร้อม ทำให้ทั้งสองฝ่ายประหยัดเวลาและทรัพยากร"*
>
> — **ChatGPT** (OpenAI)

> *"Webhook คือรากฐานของระบบ event-driven architecture ที่ทันสมัย ช่วยให้ microservices และ third-party integrations สื่อสารกันได้แบบ real-time โดยไม่ต้องพึ่ง polling ที่สิ้นเปลือง"*
>
> — **Gemini** (Google)

---

## 📚 References

1. MDN Web Docs. (2024). [*What is a Webhook?*](https://developer.mozilla.org/en-US/docs/Glossary/Webhook)
2. Zapier. (2024). [*What are Webhooks?*](https://zapier.com/blog/what-are-webhooks/)
3. GitHub Docs. (2024). [*About Webhooks*](https://docs.github.com/en/webhooks/about-webhooks)

---

*🔗 กลับไปหน้าหลัก → [sximi.github.io](https://sximi.github.io)*
