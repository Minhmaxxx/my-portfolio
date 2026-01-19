# Báo Cáo Phản Hồi (Reflection Report) - Nhóm 4 

## 1. Báo cáo về Xung đột (Conflict Report) 

**Mô tả tình huống:**  
Để thực hiện yêu cầu “Simulate Conflict”, cả 3 thành viên (Minh, Phương, Việt) đã cùng chỉnh sửa **dòng đầu tiên** của file `README.md` trên các nhánh riêng biệt và thực hiện commit gần như cùng thời điểm.

**Quá trình xử lý:**  
1. **Người merge đầu tiên:** Việt là thành viên merge Pull Request đầu tiên vào nhánh `main`. Do lúc này chưa có thay đổi trùng lặp, quá trình merge diễn ra thành công và không phát sinh lỗi.  
2. **Người merge thứ hai:** Minh tiến hành merge sau đó. Tuy nhiên, do nội dung dòng đầu tiên của `README.md` đã bị thay đổi bởi commit trước đó, GitHub bắt đầu phát sinh cảnh báo xung đột (conflict).  
3. **Người merge cuối cùng:** Phương là người merge sau cùng và cũng gặp tình trạng conflict tương tự do thay đổi trên cùng một dòng đã tồn tại trên nhánh `main`.

**Cách giải quyết:**  
Nhóm đã thống nhất sử dụng **Method 1: Local Merge Resolution** để xử lý xung đột:
- Tại máy cá nhân, các thành viên thực hiện lệnh `git pull origin main --no-rebase` để cập nhật phiên bản mới nhất của nhánh `main`.
- Sử dụng VS Code để xem chi tiết xung đột và lựa chọn phương án **Accept Both Changes**, đảm bảo giữ lại đầy đủ nội dung cần thiết.
- Sau khi xoá các conflict marker và hoàn thiện nội dung file, nhóm tiến hành `git add`, `git commit` và `git push` để cập nhật lại Pull Request.
- Cuối cùng, các Pull Request được merge thành công mà không làm ảnh hưởng đến lịch sử commit chung của dự án.

---

## 2. Giá trị của việc Review Code 

Việc thực hiện review code chéo giữa các thành viên mang lại nhiều giá trị thiết thực cho nhóm:
- **Phát hiện lỗi sớm:** Giúp nhận ra các lỗi nhỏ như sai cú pháp, thiếu thuộc tính HTML (ví dụ: `target="_blank"`) trước khi code được merge vào nhánh chính.
- **Học hỏi lẫn nhau:** Các thành viên có cơ hội tham khảo cách viết code, đặt tên commit và tổ chức cấu trúc file của nhau, từ đó cải thiện kỹ năng cá nhân.
- **Đảm bảo tính thống nhất:** Codebase được giữ sạch, rõ ràng và tuân thủ đúng quy ước chung của dự án, tránh tình trạng mỗi người viết theo một kiểu khác nhau.

---

## 3. Hoạt động Agile 

Nhóm đã áp dụng một số thực hành Agile để quản lý công việc hiệu quả hơn:
- **GitHub Projects:** Được sử dụng để theo dõi tiến độ công việc, phân chia nhiệm vụ rõ ràng và giúp các thành viên nắm được trạng thái hiện tại của từng task.
- **Mini-Standup (qua chat):** Các thành viên thường xuyên cập nhật nhanh tình trạng công việc như “đã nhận task”, “đang xử lý conflict Git” hoặc “gặp vấn đề về quyền truy cập repository”. Điều này giúp cả nhóm hỗ trợ kịp thời và đảm bảo tiến độ chung của dự án.
