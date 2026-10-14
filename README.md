Phần 1. Phân tích ngắn gọn1. Hai sai lầm của Nam:Nhầm lẫn bản chất file: Word (.docx) là file nhị phân nén (binary/zip), không phải văn bản thuần. Git không thể so sánh từng dòng (git diff) nên dù sửa một dấu phẩy, Git vẫn tính là đổi toàn bộ file $\rightarrow$ gây xung đột (conflict) và không xem trước được trên GitHub.Định kiến về Markdown: Markdown là chuẩn tài liệu ngành IT. Nó tách rời nội dung và cách hiển thị, giúp viết nhanh, mở được trên mọi máy/terminal và tự động dựng thành trang web đẹp mắt trên GitHub.2. Vì sao Markdown an toàn và nhẹ hơn?Dung lượng: Markdown chỉ lưu ký tự chữ thuần túy (vài KB), trong khi Word phải gánh thêm font, schema, metadata XML (hàng chục KB đến vài MB).Khả năng chống hỏng file (mất 1 byte):File Word: Bị mất 1 byte sẽ làm lỗi cấu trúc nén (ZIP) hoặc rách thẻ đóng XML $\rightarrow$ hỏng toàn bộ file, không mở được.Markdown: Mất 1 byte chỉ làm mất/lỗi đúng 1 ký tự đó, 99.9% nội dung còn lại vẫn đọc bình thường.Phần 2. Mẫu chuyển đổi Markdown (README.md)Thao tác nhanh trên StackEdit: Vào StackEdit.io $\rightarrow$ Dán nội dung và gắn thẻ (#, **, |) $\rightarrow$ Nhấn góc trên bên phải chọn Export to disk $\rightarrow$ Lưu tệp README.md.Markdown# Quản Lý Điểm Sinh Viên PTIT

Ứng dụng tra cứu điểm và tính điểm GPA tự động cho sinh viên PTIT.

## Tính năng chính

* Tra cứu điểm chi tiết từng học phần.
* 
* Tự động quy đổi và tính GPA theo thang điểm 4.
* 
* Cảnh báo học vụ tự động.


## Phân công nhóm

| MSSV | Họ tên | Vai trò |
| :--- | :--- | :--- |
| B23DCCN001 | Nguyễn Văn Nam | Quản lý dự án, viết tài liệu |
| B23DCCN002 | Trần Minh Đức | Backend API |
| B23DCCN003 | Lê Hoàng Long | Giao diện Frontend |

## Cài đặt

```bash
git clone [https://github.com/ptit-project/student-grade.git](https://github.com/ptit-project/student-grade.git)
cd student-grade
npm install
npm run dev
