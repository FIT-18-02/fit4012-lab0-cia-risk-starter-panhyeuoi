# Lab 01 Answers
## CIA & Risk: Hệ thống lưu điểm

**Họ và tên:** Phạm Phương Anh

**MSSV:** 1871020062

**Lớp/Nhóm:** CNTT 18-02

---

## 1. Assets

- Asset 1:Dữ liệu khách hàng/người dùng (Thông tin cá nhân, mật khẩu, số điện thoại)
- Asset 2:Mã nguồn ứng dụng (Source code) (Các thuật toán, logic xử lý của phần mềm)
- Asset 3 (nếu có):Hệ thống máy chủ (Server) (Nơi vận hành và lưu trữ toàn bộ dịch vụ)
  
## 2. Mapping CIA

- Sự cố A -> Confidentiality (Tính bảo mật)
- Sự cố B -> Integrity (Tính toàn vẹn)
- Sự cố C -> Availability (Tính sẵn sàng)
  
## 3. Phân tích sự cố B

- Threat: Kẻ tấn công (Hacker) hoặc mã độc xâm nhập hệ thống
- Vulnerability: Thiếu cơ chế kiểm soát truy cập và xác thực người dùng
- Mitigation: Cài đặt xác thực đa yếu tố (MFA) và phân quyền chặt chẽ

## 4. Reflection
Qua bài phân tích này, em nhận thấy rằng việc bảo vệ hệ thống không chỉ phụ thuộc vào công nghệ mà còn phụ thuộc vào con người và quy trình. Một lỗi thao tác nhỏ cũng có thể ảnh hưởng nghiêm trọng đến tính toàn vẹn của dữ liệu. Em học được cách xác định rõ mối đe dọa, lỗ hổng và đề xuất các biện pháp giảm thiểu cụ thể. Ngoài ra, em hiểu rõ hơn vai trò quan trọng của phân quyền, logging và backup trong an toàn thông tin. Bài học này giúp em xây dựng tư duy phân tích sự cố một cách hệ thống và có cơ sở hơn.

## 5. Bonus Flag
A → Confidentiality (C)
B → Integrity (I)
C → Availability (A)
Flag của em: FIT4012{A-C-B-I-C-A}

