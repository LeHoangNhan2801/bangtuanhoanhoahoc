# 🧪 Bảng Tuần Hoàn Nguyên Tố Hóa Học (Periodic Table Web App)

Một ứng dụng web hiện đại, trực quan và tương tác cao giúp khám phá 118 nguyên tố hóa học, được thiết kế với giao diện Dark Mode tối ưu, hiệu ứng chuyển động mượt mà và kho dữ liệu chi tiết cho từng nguyên tố.

---

## ✨ Tính năng nổi bật

* **Bảng tuần hoàn chuẩn xác:** Hiển thị toàn bộ 118 nguyên tố hóa học theo đúng cấu trúc lưới 18 nhóm và 7 chu kỳ[cite: 2].
* **Hiệu ứng chuyển động mượt mà (`Fade Up` / `Fade Down`):** Khi người dùng lọc theo nhóm danh mục (như Kim loại, Phi kim, Á kim, Khí hiếm...), các ô nguyên tố không thuộc nhóm sẽ tự động mờ đi (`fade-down`) và các ô phù hợp sẽ nổi bật lên (`fade-up`)[cite: 2, 4].
* **Tìm kiếm thông minh:** Hỗ trợ tìm kiếm thời gian thực (real-time search) theo tên nguyên tố, ký hiệu hóa học, số hiệu nguyên tử hoặc loại nhóm[cite: 2].
* **Modal thông tin chi tiết:** Khi bấm vào bất kỳ nguyên tố nào, bảng modal sẽ hiển thị đầy đủ:
  * Khối lượng nguyên tử, số hiệu, ký hiệu[cite: 2].
  * Cấu hình electron, trạng thái vật lý (rắn, lỏng, khí)[cite: 2].
  * Người phát hiện và tóm tắt thông tin nguyên tố[cite: 2].
  * Hình ảnh mô hình Bohr và ảnh chụp thực tế của nguyên tố (nếu có)[cite: 2].
* **Trắc nghiệm & Hướng dẫn:** Tích hợp trang trắc nghiệm kiến thức (`quiz.html`) và trang hướng dẫn khám phá (`getstarted.html`)[cite: 4].

---

## 📂 Cấu trúc dự án

Dự án được tổ chức gọn gàng với các tệp mã nguồn chính:
* **`index.html`**: Trang chủ chứa giao diện chính của bảng tuần hoàn và các bộ lọc.
* **`quiz.html`**: Trang luyện tập và thử thách hằng ngày qua các câu hỏi trắc nghiệm[cite: 4].
* **`getstarted.html`**: Trang giới thiệu chi tiết về lịch sử và cách sử dụng bảng tuần hoàn[cite: 4].
* **`index.js`**: Tệp JavaScript chính xử lý logic tải dữ liệu từ tệp JSON, render các ô nguyên tố, tìm kiếm, hiệu ứng lọc nhóm và quản lý modal chi tiết[cite: 2].
* **`base.css`**: Tệp CSS chứa cấu trúc bố cục gốc, biến màu giao diện (Dark theme) và responsive[cite: 3].
* **`main.css`**: Tệp CSS chứa giao diện chi tiết của bảng tuần hoàn, các hiệu ứng animation (`fade-up`, `fade-down`), style cho modal và trang quiz[cite: 4].
* **`elements.json`**: Cơ sở dữ liệu chứa thông tin chi tiết của 118 nguyên tố hóa học[cite: 2].

---

## 🛠️ Công nghệ sử dụng

* **HTML5 / CSS3**: Xây dựng giao diện hiện đại, sử dụng CSS Grid, Flexbox và `@keyframes` cho hiệu ứng mượt mà.
* **JavaScript (Vanilla ES6+)**: Xử lý DOM động, quản lý trạng thái bộ lọc và bất đồng bộ (`fetch API`)[cite: 2].
* **FontAwesome**: Hệ thống biểu tượng trực quan[cite: 4].

---

## 🚀 Hướng dẫn cài đặt và chạy thử

Vì đây là một ứng dụng web thuần (Vanilla Web App), bạn có thể chạy trực tiếp trên máy tính một cách dễ dàng:

1. **Clone hoặc tải mã nguồn** dự án về máy tính của bạn.
2. Mở thư mục dự án bằng trình soạn thảo mã nguồn (ví dụ: **VS Code**).
3. Sử dụng tiện ích mở rộng **Live Server** trên VS Code:
   * Nhấp chuột phải vào tệp `index.html`.
   * Chọn **"Open with Live Server"**.
4. Trình duyệt sẽ tự động mở ứng dụng tại địa chỉ `http://127.0.0.1:5501/index.html`[cite: 1].

---

## 💡 Hướng dẫn sử dụng tính năng lọc nhóm & hiệu ứng
* Nhấp vào các nút bộ lọc nhóm phía trên bảng (như **Kim loại**, **Phi kim**, **Á kim**, **Khí hiếm**...) để kích hoạt hiệu ứng tương tác:
  * **Fade Up**: Các nguyên tố thuộc nhóm được chọn sẽ nổi bật lên màn hình.
  * **Fade Down**: Các nguyên tố khác sẽ mờ đi và tạm khóa tương tác để làm nổi bật nhóm đang chọn[cite: 2, 4].
