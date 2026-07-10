---
name: quiz
description: Tuân thủ quy chuẩn của dự án để tạo 3 câu hỏi trắc nghiệm lớp 8 mới về một môn học cụ thể và thêm trực tiếp vào mã nguồn ứng dụng. Kích hoạt khi người dùng nhập lệnh hoặc yêu cầu dưới dạng `/quiz [tên môn học]`.
---

# HƯỚNG DẪN KÍCH HOẠT VÀ THỰC THI SKILL /quiz

Mỗi khi người dùng gõ lệnh `/quiz [Tên môn học]` hoặc yêu cầu tạo câu hỏi tương đương, bạn hãy đóng vai trò là một chuyên gia soạn đề bài và thực hiện quy trình sau:

## Bước 1: Đọc tệp quy chuẩn dự án
Hãy mở và đọc kỹ tệp [Skill.md](file:///Users/shylvaorchid/Desktop/project/ducbao-App.quiz/Skill.md) tại thư mục gốc để tuân thủ mọi quy định:
- Mỗi câu hỏi trắc nghiệm phải có **đúng 4 đáp án** (A, B, C, D).
- Phần giải thích (`explanation`) viết bằng tiếng Việt và phải có câu phản hồi phù hợp với kết quả (ví dụ: *"Đúng rồi!..."* hoặc *"Sai rồi!..."*).
- Toàn bộ mã nguồn phải nằm gọn gàng trong một tệp duy nhất là [index.html](file:///Users/shylvaorchid/Desktop/project/ducbao-App.quiz/index.html).

## Bước 2: Xác định môn học và học kỳ
Phân tích `[Tên môn học]` từ lệnh của người dùng để ánh xạ sang mã môn học tương ứng trong hệ thống:
- **Toán Học / Toán** -> `toan`
- **Ngữ Văn / Văn** -> `van`
- **Tiếng Anh / Anh** -> `anh`
- **Khoa Học Tự Nhiên / KHTN** -> `khtn`
- **Lịch Sử & Địa Lí / Sử Địa** -> `sudia`

Nếu môn học không khớp với các lựa chọn trên, hãy thông báo và hỏi lại người dùng để ánh xạ chính xác. Mặc định hãy phân phối đều 3 câu hỏi mới vào Học kỳ 1 (`hk1`) và Học kỳ 2 (`hk2`) của môn học đó, hoặc bổ sung trực tiếp vào danh sách phù hợp với chủ đề câu hỏi.

## Bước 3: Soạn 3 câu hỏi trắc nghiệm mới tinh
Soạn 3 câu hỏi trắc nghiệm mới thuộc chương trình học lớp 8 của Việt Nam. Mỗi câu hỏi tuân thủ cấu trúc dữ liệu JavaScript:
```javascript
{
  type: 'mcq',
  question: 'Nội dung câu hỏi...',
  options: [
    'Đáp án A',
    'Đáp án B',
    'Đáp án C',
    'Đáp án D'
  ],
  correct: 0, // Chỉ mục đáp án đúng (0 = A, 1 = B, 2 = C, 3 = D)
  explanation: 'Đúng rồi! [Giải thích chi tiết lý do].' (hoặc 'Sai rồi! Đáp án đúng là... vì...')
}
```

## Bước 4: Cập nhật trực tiếp vào file index.html
1. Đọc và phân tích file [index.html](file:///Users/shylvaorchid/Desktop/project/ducbao-App.quiz/index.html), tìm đến phần định nghĩa đối tượng `quizDatabase` (khoảng dòng 2258).
2. Tìm đến đúng môn học (`toan`, `van`, `anh`, `khtn`, `sudia`) và học kỳ mong muốn.
3. Chèn 3 câu hỏi mới vừa soạn vào mảng câu hỏi thích hợp trong `quizDatabase`.
4. Lưu lại tệp [index.html](file:///Users/shylvaorchid/Desktop/project/ducbao-App.quiz/index.html) và đảm bảo không phá vỡ cú pháp JavaScript của ứng dụng.

## Bước 5: Phản hồi người dùng
Sau khi cập nhật thành công, hãy gửi phản hồi tóm tắt cho người dùng về 3 câu hỏi vừa được thêm vào (bao gồm: câu hỏi, các đáp án lựa chọn và lời giải thích) để họ theo dõi.
