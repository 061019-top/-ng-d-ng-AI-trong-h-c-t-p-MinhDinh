PHÂN TÍCH PROMPT YÊU CẦU XỬ LÝ CHUỖI
1. Phân tích vì sao kết quả AI chưa hiệu quả
Thiếu Mục tiêu Xử lý Cụ thể (Missing Specific Goal): Xử lý chuỗi là khái niệm quá rộng (đảo ngược, tách, nối, tìm kiếm...). AI không biết chính xác người học muốn làm gì, nên chỉ trả về đoạn code đơn giản nhất (ví dụ: in chuỗi), không giúp rèn luyện kỹ năng.

Thiếu Ngữ cảnh và Ngôn ngữ Lập trình (Missing Context & Language): AI không được chỉ định ngôn ngữ lập trình (C, Python, Java...). Kết quả trả về có thể không phù hợp với môn học mà sinh viên đang theo đuổi (Ví dụ: Trả về code Python khi sinh viên đang học C).

2. Những yếu tố còn thiếu trong Prompt ban đầu
Vai trò AI: Không có (AI không biết nên đóng vai giáo viên, trợ giảng, hay chuyên gia).

Ngôn ngữ: Không chỉ định (C, C++, Java, Python...).

Mục tiêu: Không rõ ràng (Đảo ngược chuỗi? Loại bỏ ký tự?...).

Ngữ cảnh: Không rõ trình độ người học (Mới bắt đầu? Chuyên gia?).

Định dạng: Không yêu cầu giải thích logic hoặc định dạng code/giải thích cụ thể.

3. PROMPT MỚI ĐÃ TỐI ƯU (Mục tiêu: Kiểm tra Palindrome)
Prompt mới này sẽ giúp AI tạo ra một đoạn code C có tính ứng dụng cao, đồng thời kèm theo giải thích logic từng bước, phù hợp với mục tiêu học tập.

Prompt mới: "Bạn là một Trợ giảng Lập trình C kiêm Chuyên gia phân tích code. Mục tiêu của tôi là học cách xử lý vòng lặp. Hãy viết một đoạn code C để kiểm tra xem một chuỗi có phải là Palindrome (chuỗi đối xứng) hay không bằng cách thực hiện đảo ngược chuỗi đó. Code cần có hàm main để chạy thử, kèm theo giải thích logic từng bước dưới dạng danh sách gạch đầu dòng, phù hợp với trình độ sinh viên năm nhất."