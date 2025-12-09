1. Đặt câu hỏi cho AI (Prompt)Prompt: "Viết một hàm kiểm tra số nguyên tố bằng ngôn ngữ C. Code ngắn gọn, tối ưu và có hàm main để chạy thử."
2. Đoạn code AI tạo ra(Lưu ý: Đây là code do ChatGPT/Claude sinh ra)C#include <stdio.h>
#include <math.h>

// Hàm kiểm tra số nguyên tố
int isPrime(int n) {
    if (n <= 1) return 0; // 0 và 1 không phải số nguyên tố
    for (int i = 2; i <= sqrt(n); i++) {
        if (n % i == 0) {
            return 0; // Chia hết cho số khác -> không phải SNT
        }
    }
    return 1; // Là số nguyên tố
}

int main() {
    int num;
    printf("Nhập một số nguyên: ");
    scanf("%d", &num);

    if (isPrime(num))
        printf("%d là số nguyên tố.\n", num);
    else
        printf("%d KHÔNG phải là số nguyên tố.\n", num);

    return 0;
}
3. Quá trình chạy thử và Kiểm chứngCông cụ sử dụng: Visual Studio Code (VS Code) với trình biên dịch GCC.Phương pháp kiểm chứng (Test Cases): Tôi không chỉ chạy 1 lần mà thử nghiệm với các nhóm dữ liệu đặc biệt (Edge cases) để "bắt lỗi" AI.Kết quả chạy thực tế:Input (Số nhập vào)Dự đoán (Logic toán học)Output của Code AIĐánh giá7Là SNT"7 là số nguyên tố."ĐÚNG10Không phải SNT"10 KHÔNG phải là số nguyên tố."ĐÚNG1Không phải SNT"1 KHÔNG phải là số nguyên tố."ĐÚNG (AI đã xử lý tốt trường hợp n <= 1)-5Không phải SNT"-5 KHÔNG phải là số nguyên tố."ĐÚNG29Là SNT"29 là số nguyên tố."ĐÚNGMô tả kết quả: Code chạy đúng cú pháp, không báo lỗi biên dịch (Compile error). Logic thuật toán chính xác vì AI đã sử dụng vòng lặp chạy đến sqrt(n) (căn bậc 2) để tối ưu hiệu suất thay vì chạy đến n.4. Kết luậnBài học rút ra:AI viết code C cú pháp rất chuẩn và biết cách tối ưu thuật toán (dùng sqrt).Tuy nhiên, việc kiểm chứng bằng các trường hợp biên (số âm, số 0, số 1) là bắt buộc. Nếu không kiểm tra kỹ, rất dễ dính lỗi logic ở các trường hợp đặc biệt này.Cách để không bị lệ thuộc hoặc hiểu sai:Đọc hiểu trước khi chạy: Phải giải thích được dòng for (int i = 2; i <= sqrt(n); i++) nghĩa là gì trước khi copy. Nếu không hiểu, hãy hỏi ngược lại AI để nó giải thích.Không tin tưởng tuyệt đối: Luôn giả định code AI có lỗi tiềm ẩn và tìm cách "test cho sai" (break the code) thay vì chỉ mong nó chạy đúng.Tự gõ lại code: Thay vì Ctrl+C / Ctrl+V, hãy tự gõ lại code vào IDE. Việc này giúp não bộ ghi nhớ cú pháp và logic tốt hơn.