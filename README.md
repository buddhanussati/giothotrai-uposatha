# Giờ Thọ Trai & Lịch Uposatha

> **Công cụ hỗ trợ hành giả xác định giờ Ngọ và ngày Bố Tát**

Đây là một ứng dụng web đơn giản, được thiết kế đặc biệt cho các tu sĩ và cư sĩ Phật giáo (đặc biệt là truyền thống Nguyên Thủy/Theravada) để theo dõi thời gian được phép thọ thực trong ngày và các ngày Tụng Giới/Bát Quan Trai (Bố Tát/Uposatha).

[IMG_20251216_160214](https://github.com/user-attachments/assets/bf0e94eb-b3d6-4919-9511-6d7ed9983a46)

## ✨ Tính năng nổi bật!
### 1. Xác định chính xác giờ Ngọ (Solar Noon)
Không giống như giờ đồng hồ (12:00 trưa), giờ Ngọ trong luật nghi được tính là thời điểm mặt trời lên cao nhất (Đứng bóng). Ứng dụng sử dụng thuật toán thiên văn để:
* Tính toán thời gian **Rạng đông (Dawn)** và **Đứng bóng (Solar Noon)** dựa trên tọa độ địa lý.
* Hiển thị đồng hồ đếm ngược tới giờ chót được phép thọ thực.
* Thanh tiến trình trực quan giúp hành giả dễ dàng sắp xếp thời gian dùng bữa.

### 2. 🌕 Lịch Uposatha (Bố Tát) tự động
* Tích hợp thuật toán Âm lịch Việt Nam (dựa trên `amlich-hnd.js`).
* Tự động tính toán ngày Uposatha kế tiếp (Mùng 8, 15, 23, 30 hoặc 29 Âm lịch).
* Hiển thị hình ảnh pha mặt trời (Trăng tròn, Trăng khuyết, Trăng non) trực quan bằng SVG.

### 3. 📍 Hỗ trợ Đa Địa điểm & Múi giờ
* **Tự động định vị (GPS):** Lấy toạ độ chính xác nơi bạn đang đứng để tính giờ mặt trời chuẩn xác nhất.
* **Danh sách thành phố:** Tích hợp sẵn danh sách các thành phố lớn tại Việt Nam và các trung tâm Phật giáo quốc tế (Yangon, Mawlamyine - Pa-Auk, Bodhgaya, Bangkok, v.v.).
* **Hỗ trợ Múi giờ:** Tự động điều chỉnh giờ hiển thị theo múi giờ của địa điểm được chọn (hữu ích khi hành giả đang ở nước ngoài nhưng muốn tra cứu giờ).

### 4. 🎨 Giao diện & Kỹ thuật
* **Dark Mode:** Giao diện nền tối với tông màu vàng y (Saffron/Gold) dịu mắt, tiết kiệm pin.
* **Offline-first:** Toàn bộ mã nguồn (HTML, CSS, JS) nằm gọn trong **một file duy nhất**. Không cần kết nối internet sau khi tải file về.
* **Responsive:** Hiển thị tốt trên cả điện thoại di động và máy tính.

---

## 🚀 Cách sử dụng

Vì đây là ứng dụng dạng **Single HTML File**, bạn không cần cài đặt phức tạp.

### Chạy trực tiếp
1.  Tải file `index.html` hoặc apk về máy.
2.  Mở file bằng bất kỳ trình duyệt web nào (Chrome, Safari, Firefox, Edge).
3.  Cấp quyền truy cập vị trí (nếu muốn dùng GPS chính xác) hoặc chọn thành phố từ danh sách.

### Cài đặt như App (Trên điện thoại)
* **iOS (Safari):** Mở web -> Chọn nút Share -> "Add to Home Screen" (Thêm vào màn hình chính).
* **Android (Chrome):** Mở web -> Chọn menu (3 chấm) -> "Add to Home Screen".

---

## 🛠️ Công nghệ sử dụng

Ứng dụng được xây dựng hoàn toàn bằng **Vanilla JavaScript**, không phụ thuộc vào framework (như React/Vue) để đảm bảo tính nhẹ nhàng và dễ lưu trữ.

* **SunCalc:** Thư viện tính toán vị trí mặt trời/mặt trăng (Vladimir Agafonkin).
* **AmLich-HND:** Thuật toán chuyển đổi Dương-Âm lịch (Hồ Ngọc Đức).
* **HTML5/CSS3:** Flexbox, Grid layout và CSS Variables cho giao diện.

---

## 📸 Ảnh chụp màn hình (Mô tả)

* *Màn hình chính:* Hiển thị năm Dương lịch/Phật lịch và Giờ hiện tại.
* *Card Lịch Uposatha:* Hiển thị ngày Bố Tát sắp tới cùng biểu tượng mặt trăng tương ứng.
* *Card Đếm ngược:* Đồng hồ đếm ngược to rõ tới giờ Ngọ, kèm trạng thái (Đang thọ thực/Đã quá giờ).
* *Thông số chi tiết:* Bảng hiển thị giờ Rạng đông, Mặt trời mọc/lặn cụ thể.

---

## 📝 Lưu ý cho Hành giả

* **Giờ Ngọ:** Ứng dụng tính toán thời điểm mặt trời đi qua kinh tuyến (Transit/Solar Noon). Đây là mốc thời gian kỹ thuật chính xác nhất cho việc giữ giới không ăn phi thời.
* **Vị trí:** Để có kết quả chính xác nhất từng phút, hãy sử dụng tính năng **"Dùng GPS"** thay vì chọn thành phố, vì mỗi sự thay đổi nhỏ về kinh độ đều ảnh hưởng đến giờ mặt trời.

---

## 📄 License

Dự án này là mã nguồn mở. Bạn có thể tự do sửa đổi, phân phối phi thương mại để phục vụ cộng đồng tu tập.

* *SunCalc Library (c) 2011-2015, Vladimir Agafonkin*
* *AmLich Logic (c) Hồ Ngọc Đức*
