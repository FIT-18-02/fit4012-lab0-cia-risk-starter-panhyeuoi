# Lab 01 Answers
## CIA & Risk: Hệ thống lưu điểm

**Họ và tên:** Phạm Phương Anh

**MSSV:** 1871020062

**Lớp/Nhóm:** CNTT 18-02

---

## 1. Assets
Liệt kê ít nhất 2 assets cần bảo vệ.
ví dụ 1: cho hệ thống website thương mại điện 
Asset 1: Dữ liệu khách hàng (tên, email, địa chỉ, thông tin thanh toán)
Asset 2: Server chứa mã nguồn website
Asset 3: Cơ sở dữ liệu đơn hàng

## 2. Mapping CIA
Ghép từng sự cố với CIA.
Sự cố A: Hacker xâm nhập và đánh cắp danh sách khách hàng
Sự cố B: Nhân viên vô tình sửa sai thông tin trong database
Sự cố C: Website bị DDoS dẫn đến tê liệt 3 giờ
 Mapping CIA:
Sự cố A → Confidentiality (bị lộ thông tin)
Sự cố B → Integrity (dữ liệu bị thay đổi sai)
Sự cố C → Availability (không truy cập được)

## 3. Phân tích sự cố B
Threat (Mối đe dọa):
Người dùng nội bộ hoặc kẻ tấn công có thể thay đổi dữ liệu quan trọng, làm sai lệch thông tin trong hệ thống.
Vulnerability (Lỗ hổng):
Hệ thống thiếu kiểm soát phân quyền (Access Control yếu).
Không có cơ chế kiểm tra thay đổi (change tracking).
Không bật xác nhận thao tác hoặc không có bản sao lưu dữ liệu.
Mitigation (Giảm thiểu):
Áp dụng phân quyền chặt chẽ (RBAC).
Sử dụng cơ chế kiểm tra toàn vẹn (hash, checksum, logging).
Thiết lập cơ chế versioning hoặc backup định kỳ để khôi phục dữ liệu.
Thêm bước xác nhận trước thao tác quan trọng (confirmation dialog).

## 4. Reflection
Qua bài phân tích này, em nhận thấy rằng việc bảo vệ hệ thống không chỉ phụ thuộc vào công nghệ mà còn phụ thuộc vào con người và quy trình. Một lỗi thao tác nhỏ cũng có thể ảnh hưởng nghiêm trọng đến tính toàn vẹn của dữ liệu. Em học được cách xác định rõ mối đe dọa, lỗ hổng và đề xuất các biện pháp giảm thiểu cụ thể. Ngoài ra, em hiểu rõ hơn vai trò quan trọng của phân quyền, logging và backup trong an toàn thông tin. Bài học này giúp em xây dựng tư duy phân tích sự cố một cách hệ thống và có cơ sở hơn.

## 5. Bonus Flag
A → Confidentiality (C)
B → Integrity (I)
C → Availability (A)
Flag của em: FIT4012{A-C-B-I-C-A}

