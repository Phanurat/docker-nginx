# ใช้ภาพพื้นฐานที่ต้องการ
FROM alpine:latest

# ติดตั้ง curl
RUN apk --no-cache add curl

# คัดลอกสคริปต์อัปเดต DuckDNS ไปยังคอนเทนเนอร์
COPY update_duckdns.sh /update_duckdns.sh
RUN chmod +x /update_duckdns.sh

# ตั้งค่า cronjob (หรือคุณสามารถใช้คำสั่งนี้เมื่อเริ่มต้นคอนเทนเนอร์)
CMD ["/update_duckdns.sh"]
