## **PHẦN 1: BÁO CÁO PHÂN TÍCH I/O (INPUT / OUTPUT)**

1.  **Dữ liệu đầu vào (Input - Văn bản thô & Ghi chú kỹ thuật):**
    
    -   Các đoạn chú thích kỹ thuật, tên biến (`pin_sensor`, `relay_pin`), và các ký tự đặc biệt (`#`, `*`) cần được hiển thị nguyên bản mà không bị hiểu lầm là cú pháp Markdown.
        
    -   Thông số thô về hai dòng cảm biến cũ và mới.
        
    -   Danh sách các công việc kiểm tra thiết bị phần cứng trước khi vận hành hệ thống tưới nước tự động.
        
2.  **Kết quả mong đợi (Output - Giao diện Render chuyên nghiệp):**
    
    -   Văn bản giải thích sử dụng Inline Code làm nổi bật các tên biến hoặc câu lệnh ngắn gọn.
        
    -   Đoạn mã Python điều khiển máy bơm được đóng gói trong Fenced Code Block (python) với màu sắc cú pháp trực quan (Syntax Highlighting).
        
    -   Bảng so sánh (`Markdown Table`) trình bày rõ ràng ưu/nhược điểm giữa cảm biến cũ và mới.
        
    -   Danh sách kiểm tra (`Task List`) hiển thị các hộp kiểm tương tác trực tiếp (`[x]` và `[ ]`).
        
    -   Sử dụng ký tự thoát (`\`) để hiển thị chính xác các ký tự đặc biệt như `\#1` trên giao diện người dùng.
        

## **PHẦN 2: SOURCE CODE TỆP `README.md` HOÀN CHỈNH
## 1. So sánh Cảm biến Độ ẩm (Loại Cũ vs. Loại Mới)

| Tiêu chuẩn so sánh | Cảm biến Điện dung Cũ (v1) | Cảm biến Điện trở Mới (v2) |
| :--- | :--- | :--- |
| **Độ bền vật liệu** | Dễ bị oxy hóa sau 3 tháng vận hành | Chống ăn mòn cao nhờ lớp phủ mạ vàng |
| **Độ chính xác** | Thấp ( 10\%$) | Cao ( 2\%$) |
| **Giao tiếp tín hiệu** | Tín hiệu Analog thuần túy | Hỗ trợ giao thức kỹ thuật số I2C |

---

## 3. Checklist Kiểm tra Thiết bị Trước Khi Vận Hành

-   Kiểm tra kết nối nguồn điện ổn định cho bo mạch vi điều khiển chính.
    
-    Xác thực biến `pin_sensor` trùng khớp với sơ đồ mạch phần cứng thực tế.
    
-    Tiến hành hiệu chuẩn độ ẩm thực tế tại khu vực nhà kính trồng lan #1.
    
-    Kiểm tra cơ chế tự ngắt an toàn của rơ-le máy bơm khi xảy ra sự cố điện áp.




