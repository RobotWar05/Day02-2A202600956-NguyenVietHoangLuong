# BÍ KÍP THỰC HÀNH DAY 02: TỪ VẤN ĐỀ ĐẾN GIẢI PHÁP AI

> 💡 **3 QUY TẮC SỐNG CÒN:**
> 1. **Problem first, not AI first:** Cấm bắt đầu bằng câu "Tôi muốn làm chatbot để...". Phải bắt đầu bằng "Tôi đang tốn 2 tiếng mỗi ngày để...".
> 2. **Không AI vẫn là kết luận tốt:** Điểm số nằm ở lập luận logic, không nằm ở việc cố nhét AI vào bài toán.
> 3. **Tự vắt óc trước, AI hỗ trợ sau:** Không quăng giấy trắng cho AI bắt nó tự nghĩ ra vấn đề. Trải nghiệm đau đớn thực tế phải đến từ chính bạn!

---

## 💎 VIÊN KIM CƯƠNG 1: TÌM ĐÚNG VẤN ĐỀ (Phân kỳ cá nhân)

### PHASE 1: INDIVIDUAL PROBLEM SCAN (Quét Vấn Đề)
**Mục tiêu:** Liệt kê ít nhất 5 "nỗi đau" (pain point) thực tế dựa trên 4 lăng kính.

**Cách thực hiện:**
1. **Tự nghĩ (Không AI):** Liệt kê nhanh các công việc lặp lại, tốn thời gian, hoặc những việc bạn hay bị người khác giục giã phàn nàn.
2. **Dùng AI mở rộng:** Nếu bí ý tưởng, hãy dùng prompt: *"Tôi làm công việc/ngành nghề [Tên nghề]. 3 nỗi đau thực tế tôi đang gặp là [A, B, C]. Dựa vào 4 lăng kính (Lặp lại, Tốn thời gian, AI tốt hơn, Pain từ người khác), hãy gợi ý thêm 2 vấn đề thực tế nữa sát với ngành của tôi. Cấm nói chung chung."*

---

## 💎 VIÊN KIM CƯƠNG 2: HỘI TỤ & LỰA CHỌN GIẢI PHÁP

### PHASE 2: TOP 3 PROBLEM CARDS & DRAFT WORKFLOW
**Mục tiêu:** Chọn ra 3 vấn đề đau nhất. Sau đó biến Vấn đề #1 thành Problem Statement (PS) 9 trường hoàn chỉnh và Vẽ Workflow.

#### Bước 2.1: Chốt Problem Statement 9 trường

1. **Bài toán (Problem):** Mỗi khi Server báo lỗi, Dev phải tải file log khổng lồ và mò mẫm tìm nguyên nhân bằng tay, kéo dài thời gian web sập.
2. **Actor:** Backend Developer.
3. **Current Workflow (Quy trình hiện tại):**
   *(1) Nhận Alert → (2) Tải Log → (3) Mở file tìm chữ ERROR → (4) Đọc ngữ cảnh 50 dòng → (5) Search Google cách sửa → (6) Sửa Code.*
4. **Bottleneck (Nút thắt):** Bước 3 & 4 (Dò bằng mắt trong đống text vô nghĩa tốn 40 phút).
5. **Impact (Tác động):** Hệ thống sập lâu, khách hàng phàn nàn, Dev stress nặng.
6. **Success Metric (Đo lường thành công):** Giảm thời gian chẩn đoán lỗi từ 60 phút xuống < 10 phút.
7. **Boundary (Ranh giới):** AI không được tự động chọc vào sửa code trên Production. AI chỉ được phép đọc và đề xuất.
8. **Điểm AI can thiệp (Intervention):** Xen vào giữa bước 2 và 5 (AI tự đọc file log và tóm tắt nguyên nhân).
9. **Mức chọn / Rủi ro & HITL:** Chọn **Workflow**. Rủi ro: AI bị ảo giác (hallucination) chỉ sai lỗi. HITL (Human-in-the-loop): Dev là người đọc kết quả cuối cùng và tự tay sửa code.

#### Bước 2.2: Vẽ Workflow (Trước và Sau AI)
**Prompt:** 
Vẽ luồng ASCII/mermaid minh hoa trực quan luồng sau:
Daily report tiến độ công việc cho team:
- Hàng ngày ... phải tổng hợp thông tin từ: 
- Tự động gom nhóm phân loại các vấn để theo mức độ cấp bách, ai là người chịu trách nhiệm xừ lý
- Tạo một report và gửi lại cho..

---

## 🛡️ BÍ KÍP LẤY ĐIỂM TỐI ĐA KHI THUYẾT TRÌNH (Từ file Tham Khảo)
Khi chốt giải pháp và biện luận với nhóm (Decision: Go/Not Yet/No-Go), hãy "vay mượn" các thuật ngữ chuyên ngành sau để bảo vệ bài làm:

1. **Nguyên tắc "AI is Boost, not Replace" (Case study Stripe AI):** Nhấn mạnh giải pháp của bạn không thay thế con người, chỉ giúp con người làm nhanh hơn (Ví dụ: Dev vẫn phải review code).
2. **Thiết kế UX "AI suggest, Human decide" (Case study GitHub Copilot):** Áp dụng ranh giới an toàn. AI chỉ đưa ra gợi ý, con người phải chịu trách nhiệm bấm "Approve".
3. **Quyết định "Not Yet" là sự chín chắn:** Nếu bạn thấy bài toán không có đủ dữ liệu (Data) để test, hoặc rủi ro sai sót quá lớn, hãy dõng dạc chọn **Not Yet** hoặc chọn giải pháp tĩnh **Rule-based**. Giảng viên chấm điểm cao cho tư duy quản trị rủi ro này hơn là vẽ ra một con Agent ảo tưởng!

