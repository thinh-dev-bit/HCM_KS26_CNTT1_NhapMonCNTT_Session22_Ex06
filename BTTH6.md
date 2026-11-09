# BÁO CÁO BÀI TẬP VỀ NHÀ: ỨNG DỤNG PROMPT AI VÀ BUG REPORTING (SESSION 22)

Dưới đây là báo cáo tổng hợp kỹ năng vận dụng Trợ lý AI và quy chuẩn báo cáo lỗi (Bug Reporting Framework) để xử lý sự cố từ chối quyền truy cập (Permission denied) khi đẩy mã nguồn lên GitHub.

---

## Phần 1: Sử dụng Công thức Prompt 3 Thành phần nhờ AI giải mã

Để nhờ Trợ lý AI (ChatGPT/Gemini) phân tích lỗi một cách an toàn và dễ hiểu nhất mà không bị hiện tượng ảo giác, tôi thiết kế câu lệnh theo cấu trúc 3 mảnh ghép sau:

> **[Context - Ngữ cảnh]**
> Tôi đang làm dự án lập trình và cần đẩy mã nguồn (push code) lên GitHub bằng Terminal trên máy tính. Tuy nhiên, hệ thống đột ngột văng lỗi từ chối quyền truy cập và chặn không cho tôi đẩy code lên. Tôi đã thử gõ lại lệnh nhưng vẫn thất bại.
> 
> **[Raw Error - Lỗi nguyên văn]**
> Dưới đây là thông báo lỗi nguyên văn trên Terminal:
> `error: open(".git/FETCH_HEAD"): Permission denied`
> 
> **[Instruction - Yêu cầu]**
> Hãy đóng vai một chuyên gia IT, giải thích nguyên nhân gốc rễ của lỗi này bằng tiếng Việt bình dân, dễ hiểu nhất cho người mới học. Sau đó, hãy hướng dẫn tôi từng bước để khắc phục sự cố này.

---

## Phần 2: Thực thi giải pháp và Tiêu chuẩn chụp ảnh minh họa

Giả sử Trợ lý AI giải thích nguyên nhân là do thư mục bị khóa quyền và đề xuất giải pháp: *"Đóng VS Code / Terminal hiện tại và mở lại bằng quyền Quản trị viên (Run as Administrator)"*.

**Thao tác thực thi:**
1. Đóng toàn bộ cửa sổ VS Code đang mở.
2. Mở Start Menu (Windows), gõ `VS Code`.
3. Nhấp chuột phải vào biểu tượng Visual Studio Code ➔ Chọn **Run as administrator**.
4. Mở lại Terminal trong VS Code và gõ lại lệnh Git.

**Tiêu chuẩn chụp ảnh màn hình chuyên nghiệp:**
> **[KHUNG DÁN ẢNH CHỤP MÀN HÌNH MINH HỌA]**
> *(Sinh viên thực hiện dán ảnh vào đây)*

**Quy tắc chụp ảnh đã áp dụng:**
*   **Công cụ:** Sử dụng phím tắt `Win + Shift + S` (Windows 11) để chụp chính xác vùng cửa sổ Terminal báo lỗi, không chụp toàn bộ màn hình desktop lộn xộn.
*   **Khoanh vùng:** Dùng công cụ cọ vẽ (màu đỏ hoặc vàng) khoanh viền rõ ràng dòng chữ `error: open(".git/FETCH_HEAD"): Permission denied`.
*   **Bảo mật thông tin (Che mờ):** Đã bôi đen tên người dùng máy tính (Windows Username) trong đường dẫn Terminal (ví dụ: `C:\Users\***\project>`) để tránh lộ thông tin cá nhân.

---

## Phần 3: Soạn thảo tin nhắn nhờ hỗ trợ (Bug Reporting Framework)

Trường hợp sau khi chạy quyền *Run as Administrator* như AI gợi ý nhưng lỗi vẫn không biến mất, tôi sẽ nhắn tin nhờ Giảng viên hỗ trợ theo đúng khung chuẩn 4 mảnh ghép để tiết kiệm thời gian cho cả hai bên:

**Mẫu tin nhắn gửi Giảng viên:**

```text
Dạ em chào thầy, em đang gặp sự cố về quyền truy cập khi dùng Git, thầy xem giúp em với ạ:

1. [CONTEXT - Bối cảnh]
Em đang dùng Windows 11 và sử dụng Terminal tích hợp trong VS Code để đẩy code bài tập lên GitHub.

2. [EXPECTED - Kỳ vọng]
Em mong muốn chạy lệnh Git thành công để hoàn tất việc đồng bộ mã nguồn lên kho chứa (Repository) trước giờ nộp bài.

3. [ACTUAL - Thực tế phát sinh]
Tuy nhiên, Terminal liên tục báo lỗi từ chối quyền truy cập vào file FETCH_HEAD. Em đã thử hỏi AI và làm theo cách đóng VS Code, mở lại bằng quyền "Run as Administrator" nhưng Terminal vẫn hiện dòng lỗi y hệt như cũ. 

4. [LOG & SCREENSHOT - Bằng chứng]
- Lỗi nguyên văn: `error: open(".git/FETCH_HEAD"): Permission denied`
- Em có đính kèm ảnh chụp màn hình cửa sổ Terminal đã khoanh đỏ dòng lỗi bên dưới ạ. Thầy xem hướng dẫn giúp em bước khắc phục tiếp theo với nhé!