# Website Tin học 11 – Bài 5

Website tĩnh để luyện tập nội dung **Bài 5: Kết nối máy tính với các thiết bị số** (Tin học 11, bộ Kết nối tri thức với cuộc sống).

## Chạy thử trên máy tính
1. Giải nén thư mục.
2. Mở `index.html` bằng Chrome, Edge hoặc Firefox.
3. Không cần cài thêm thư viện hay chạy máy chủ.

## Đưa lên GitHub Pages
1. Đăng nhập GitHub và tạo repository mới, ví dụ `tin-hoc-11-bai-5`.
2. Để repository ở chế độ **Public** nếu muốn dùng GitHub Pages miễn phí theo cách thông thường.
3. Tải lên file `index.html` (có thể tải cả `README.md`).
4. Vào **Settings → Pages**.
5. Trong phần **Build and deployment**, chọn **Deploy from a branch**.
6. Chọn branch `main`, thư mục `/(root)`, rồi bấm **Save**.
7. Chờ GitHub triển khai; đường dẫn thường có dạng:
   `https://TEN-TAI-KHOAN.github.io/tin-hoc-11-bai-5/`

## Chức năng có sẵn
- Giao diện responsive cho máy tính và điện thoại.
- 15 câu trắc nghiệm mẫu, mỗi câu có giải thích.
- Điều hướng câu hỏi, thanh tiến độ, xác nhận nộp bài.
- Chấm điểm và xem lại đáp án.
- Nhập họ tên và lớp; in kết quả.

## Giới hạn cần biết
- Đây là website tĩnh chạy hoàn toàn trên trình duyệt.
- Kết quả chưa được gửi về giáo viên, không có bảng điểm tập trung và không xác thực danh tính.
- Họ tên/lớp chỉ dùng để hiển thị trên màn hình kết quả, không được lưu lên máy chủ.
- Câu hỏi là bộ mẫu để khởi tạo website. Giáo viên nên rà soát và điều chỉnh theo đúng nội dung dạy học, đặc biệt nếu lớp dùng định hướng/chuyên đề khác nhau.

## Chỉnh sửa câu hỏi
Trong `index.html`, tìm `const questionBank = [` ở gần cuối file. Mỗi câu hỏi có cấu trúc:
- `q`: nội dung câu hỏi
- `a`: mảng 4 lựa chọn
- `c`: chỉ số đáp án đúng, bắt đầu từ 0 (0=A, 1=B, 2=C, 3=D)
- `e`: phần giải thích

Ví dụ:
```js
{q:"Câu hỏi?", a:["Đáp án A","Đáp án B","Đáp án C","Đáp án D"], c:1, e:"Giải thích đáp án."}
```
