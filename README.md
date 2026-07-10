# 🚀 Đấu Trường Tri Thức Lớp 8 - Ôn Luyện Học Tập Gamified

Chào mừng bạn đến với **Đấu Trường Tri Thức Lớp 8**! Đây là một ứng dụng web ôn tập kiến thức trực quan, sinh động và được thiết kế theo mô hình trò chơi hóa (Gamification) nhằm đồng hành cùng **Đức Bảo** trong quá trình ôn tập và chuẩn bị cho các kỳ thi lớp 8 ngay tại nhà một cách hứng thú và hiệu quả nhất.

---

## 🎯 Mục Tiêu Dự Án
Ứng dụng được xây dựng với mục tiêu biến những giờ ôn tập lý thuyết khô khan thành một cuộc phiêu lưu chinh phục tri thức:
- Giúp học sinh lớp 8 (đặc biệt là Đức Bảo) củng cố nhanh kiến thức trọng tâm của học kỳ 1 và học kỳ 2.
- Theo dõi tiến trình học tập cá nhân trực quan.
- Tăng cường động lực ôn luyện hàng ngày thông qua hệ thống tích điểm XP, tăng cấp độ (Level) và bảng danh hiệu (Badges).

---

## ✨ Các Tính Năng Nổi Bật

### 1. Hệ Thống Câu Hỏi Đa Dạng
- **Trắc Nghiệm (Multiple Choice):** Bộ câu hỏi trắc nghiệm phủ rộng 5 môn học chính (Toán, Văn, Anh, Khoa học Tự nhiên, Lịch sử & Địa lí). Mỗi câu hỏi đều đi kèm phần giải thích chi tiết đáp án giúp học sinh hiểu sâu bản chất.
- **Tự Luận (Essay):** Trải nghiệm làm bài tự luận thông minh nhờ công nghệ phát hiện từ khóa cốt lõi (Keywords Detector), đối chiếu trực tiếp bài làm với đáp án mẫu và cho phép học sinh tự đánh giá (Self-assessment) để nhận mức XP tương ứng.

### 2. Tự Tạo Câu Hỏi Mới (Custom Questions)
- Cho phép người dùng tự gõ thêm câu hỏi trắc nghiệm của riêng mình.
- Tích hợp lưu trữ nội bộ (**LocalStorage**) giúp các câu hỏi tự thêm không bị mất đi khi tải lại trang.
- Tự động đồng bộ số lượng câu hỏi và cập nhật tiến trình ôn tập hiển thị trên giao diện chính Dashboard.

### 3. Trải Nghiệm Trò Chơi Hóa (Gamification)
- **Hệ Thống XP & Level:** Tích lũy XP sau mỗi câu trả lời đúng để thăng cấp.
- **Hộp Huy Hiệu (Badges Cabinet):** Mở khóa các huy hiệu danh giá khi hoàn thành thử thách xuất sắc (ví dụ: *Tân Binh Tự Học*, *Chuỗi Siêu Cấp*, *Bút Thần Tự Luận*, *Nhà Thông Thái*).
- **Công Nghệ Âm Thanh & Hiệu Ứng:**
  - Bộ tổng hợp âm thanh ảo (**Web Audio API**) phát nhạc và giai điệu phản hồi sinh động khi trả lời hoặc thăng cấp.
  - Hiệu ứng pháo hoa (**Confetti**) và các hạt chuyển động lơ lửng (**Particle Engine**) tạo cảm giác hưng phấn như đang chơi game.

### 4. Tùy Biến Giao Diện Cao Cấp
- **Chế Độ Sáng/Tối (Light/Dark Mode):** Chuyển đổi nhanh chóng bằng nút bấm biểu tượng 🌙/☀️ ở góc trên màn hình giúp bảo vệ mắt khi học bài vào ban đêm.
- **Cấu Hình Cá Nhân Hóa:** Chọn linh vật Avatar, thay đổi tông màu chủ đạo trang web, chỉnh âm lượng và chọn kiểu nền ứng dụng (Gradient mượt mà hoặc nền hạt động lơ lửng).

---

## 🛠️ Hướng Dẫn Cách Chạy Ứng Dụng Trên Google Chrome

Vì ứng dụng được xây dựng hoàn toàn bằng công nghệ Web thuần túy (**HTML5, CSS3, JavaScript**), bạn có thể chạy ứng dụng cực kỳ nhanh chóng mà không cần cài đặt bất kỳ môi trường lập trình phức tạp nào.

### Cách 1: Mở trực tiếp file HTML (Khuyên dùng cho sự đơn giản)
1. Tải toàn bộ thư mục dự án về máy tính của bạn.
2. Tìm đến file `index.html` trong thư mục dự án.
3. Click chuột phải vào file `index.html`, chọn **Open With (Mở bằng)** -> **Google Chrome**.
4. Hoặc bạn chỉ cần kéo thả trực tiếp file `index.html` vào một tab trống của trình duyệt Google Chrome.

### Cách 2: Chạy qua Live Server (Nếu phát triển code thêm)
Nếu bạn có sử dụng Visual Studio Code:
1. Mở thư mục dự án bằng VS Code.
2. Cài đặt tiện ích mở rộng **Live Server** (tác giả *Ritwick Dey*).
3. Nhấn vào nút **Go Live** ở góc dưới bên phải cửa sổ VS Code để khởi chạy trang trên trình duyệt Google Chrome của bạn.

---

## 📝 Cơ Cấu Môn Học Ôn Tập
- **📐 Toán Học 8:** Hằng đẳng thức, tam giác vuông Pythagore, định lí Thalès, phương trình bậc nhất...
- **✍️ Ngữ Văn 8:** Tác phẩm Lão Hạc, Tôi đi học, Ông đồ, Nhớ rừng, Chiếu dời đô...
- **🇬🇧 Tiếng Anh 8:** Bài tập trọng âm, câu điều kiện (loại 1, 2), quá khứ tiếp diễn, câu gián tiếp, bị động...
- **🧪 Khoa Học Tự Nhiên:** Lý thuyết Acid-Base, tính toán Mol, áp suất cơ học, sinh lý cơ thể người...
- **🌍 Lịch Sử & Địa Lí:** Cách mạng Pháp, đặc điểm địa hình Việt Nam, khí hậu gió mùa feralit...

Qua dự án mình đã tự tạo được một app trắc nghiệm và tự luận để ôn thi, mình cũng đã add các chức năng giúp người dùng của app như setting chỉnh độ sáng và tự nhập câu hỏi của mình vào

Chúc **Đức Bảo** ôn thi thật tốt và đạt kết quả cao nhất trong các kỳ thi sắp tới với **Đấu Trường Tri Thức Lớp 8**! 🏆🌟
