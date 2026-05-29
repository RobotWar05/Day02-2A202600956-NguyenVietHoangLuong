*Case: Hỗ trợ Tân học viên tìm kiếm phòng trọ và tiện ích xung quanh trường.*

*Bối cảnh: Lương, học viên khóa học VIN AI thực chiến, đang ở xa và cần tìm chỗ ở gần khu vực trường học, tiện ích xung quanh trước ngày khai giảng.*

---

# 01 — Individual Problem Scan

## Scan rộng
Lương scan 5 problems từ trải nghiệm chuẩn bị đi học thực tế của mình:

| # | Lăng kính | Problem quan sát được | Ai đang đau? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | Tốn thời gian | Học viên phải lướt các hội nhóm Facebook để tìm phòng trọ trống, sau đó copy địa chỉ thủ công sang Google Maps để kiểm tra khoảng cách đến giảng đường. | Tân học viên | Mất trung bình 3-5 ngày lướt điện thoại liên tục, ghi chép hỗn loạn ra sổ tay để so sánh khoảng 10-15 phòng khác nhau. |
| 2 | AI có thể tốt hơn | Đọc file PDF "Handbook hướng dẫn tân học viên" dài 35 trang để tìm các mốc thời gian quan trọng, quy định học tập và hồ sơ cần nộp trước ngày khai giảng. | Tân học viên | Tốn khoảng 30-45 phút đọc dò từng trang, dễ bỏ sót các mốc quan trọng chẳng hạn ngày nộp hồ sơ gốc dẫn đến việc phải nhắn tin hỏi ban tổ chức. |
| 3 | Pain từ người khác | Ban tổ chức hoặc Admin chương trình tuyển sinh bị quá tải tin nhắn từ học viên mới với các câu hỏi trùng lặp về thủ tục nhập học và chỗ ở gần trường. | Ban tổ chức | Hơn 50+ tin nhắn đổ về mỗi ngày trong tuần đầu, Ban tổ chức phải liên tục copy-paste cùng một câu trả lời. |
| 4 | Lặp lại | So sánh thủ công các yếu tố phi cấu trúc của phòng trọ như số tiền đặt cọc, việc có chung chủ hay không, phòng có điều hòa hay không và giá điện nước để tìm ra phòng tối ưu chi phí. | Tân học viên | Phải tự lập bảng so sánh Excel với hơn 10 cột thông số khác nhau, tốn nhiều công sức phân loại và đắn đo. |
| 5 | Tốn thời gian | Phải đến tận nơi sớm trước 2 ngày để đi khảo sát thực tế xung quanh trường nhằm tìm các tiện ích cơ bản như quán cơm bình dân, siêu thị mini, cây rút tiền ATM và tiệm thuốc. | Tân học viên | Mất nguyên một buổi chiều đi bộ hoặc chạy xe máy quanh bán kính 2km dưới nắng nóng, rất mệt mỏi và tốn kém. |

## Top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Tìm hiểu về khóa học, tìm trọ và các tiện ích xung quanh | Đây là rào cản tâm lý lớn nhất của học viên ở xa. Việc tìm kiếm không chỉ tốn thời gian mà còn gây căng thẳng, trực tiếp ảnh hưởng đến quyết định nhập học hay từ bỏ khóa học. | Khả năng thu thập dữ liệu tự động từ các nhóm kín Facebook có thể bị hạn chế do thuật toán bảo mật của Meta; cần giải pháp thay thế là chuẩn bị cơ sở dữ liệu trọ thủ công trước. |
| 2 | Tóm tắt PDF, tài liệu hướng dẫn của khóa học | Dữ liệu đầu vào như file PDF của trường đã có sẵn và chuẩn xác từ ban tổ chức, tính khả thi về mặt kỹ thuật cực kỳ cao. | Học viên có thể lười tương tác với tài liệu hoặc quen với việc nhắn tin hỏi trực tiếp ban tổ chức hơn là tự chat với bot. |
| 3 | Tự động hóa giải đáp Q&A tuyển sinh | Giải phóng sức lao động cho ban tuyển sinh trong các đợt cao điểm và phản hồi tức thì cho học viên thắc mắc. | Rủi ro AI bị ảo giác rồi trả lời sai lệch về học phí hoặc chính sách, gây tranh chấp thông tin hoặc hiểu lầm nghiêm trọng. |

---

## Problem Card #1 — Tìm hiểu khóa học, tìm trọ và tiện ích xung quanh

**Bài toán 1 câu:**
Tân học viên từ tỉnh xa tốn nhiều ngày tự tổng hợp thông tin phòng trọ từ các hội nhóm Facebook lộn xộn rồi đối chiếu khoảng cách trên Google Maps, gây stress và trì hoãn quá trình chuẩn bị nhập học.

**Actor:**
Tân học viên khóa học, đặc biệt là các học viên đến từ tỉnh xa.

**Thời điểm / bối cảnh:**
Sau khi nhận thông báo trúng tuyển, trước ngày khai giảng 1-2 tuần.

**Current workflow:**

1. Nhận email thông báo trúng tuyển kèm hướng dẫn nhập học dạng PDF.
2. Đọc tài liệu PDF để nắm địa chỉ giảng đường và các mốc thời gian khai giảng.
3. Lên Facebook tìm kiếm các từ khóa ví dụ tìm trọ gần trường VinUni trong 3-4 hội nhóm khác nhau.
4. Inbox hỏi giá chủ nhà, tự lọc tin rác và ghi lại danh sách phòng tiềm năng.
5. Copy địa chỉ từng phòng trọ sang Google Maps để tính khoảng cách và kiểm tra xung quanh có tiện ích như chợ hoặc quán ăn hoặc cây xăng không.
6. Di chuyển đến thực tế để xem phòng và đặt cọc.

**Bottleneck:**
Bước 3 và Bước 4 — Việc tìm kiếm thủ công, đối chiếu thông tin phòng trọ trên Facebook và khoảng cách địa lý trên bản đồ mất nhiều ngày và rất dễ bị rối.

**Impact:**
Học viên mất 3 ngày mệt mỏi, stress trước khi nhập học; nhà trường có nguy cơ bị rơi rụng học viên do rào cản đi lại và chỗ ở.

**Success metric:**
Giảm thời gian tìm ra danh sách 3 phòng trọ tối ưu từ 3 ngày xuống dưới 15 phút.

**Non-AI alternative:**
Ban tổ chức cung cấp danh sách Excel tĩnh hoặc bản đồ tĩnh chứa danh sách nhà trọ và tiện ích cố định gần trường.

**AI hypothesis:**
Sử dụng trí tuệ nhân tạo trong một quy trình công việc: tự động thu thập dữ liệu phòng trọ từ Facebook, dùng API bản đồ tính khoảng cách, AI draft bảng đề xuất 3 phòng trọ tốt nhất theo ngân sách và tiện ích mong muốn.

**Quick gut:**
Workflow.

Draft current workflow
```text
CURRENT STATE — 3 ngày

┌──────────────┐     ┌──────────────┐     ┌──────────────┐
│ 1 Nhận thông │     │ 2 Đọc PDF    │     │ 3 Tìm trọ    │
│ báo          │ ──> │ tài liệu     │ ──> │ trên FB      │
│ ⏱ 1'         │     │ ⏱ 30'        │     │ ⏱ 2 ngày 🔴  │
└──────────────┘     └──────────────┘     └──────────────┘
                                                 │
                                                 ▼
┌──────────────┐                          ┌──────────────┐
│ 5 Đi xem     │                          │ 4 Tra Maps & │
│ thực tế      │ ──────────────────────── │ tiện ích     │
│ ⏱ 1 ngày     │                          │ ⏱ 4 tiếng 🔴 │
└──────────────┘                          └──────────────┘

🔴 = Bottleneck
```

Draft future workflow
```text
FUTURE STATE — 15 phút

┌──────────────┐     ┌──────────────┐     ┌──────────────┐
│ 1 Nhận thông │     │ 2 Nhập budget│     │ 3 Bot query  │
│ báo + link   │ ──> │ & nhu cầu    │ ──> │ DB & Map API │
│ ⏱ 1'         │     │ ⏱ 1'         │     │ ⏱ 2'         │
└──────────────┘     └──────────────┘     └──────────────┘
                                                 │
                                                 ▼
┌──────────────┐                          ┌──────────────┐
│ 5 Học viên   │                          │ 4 AI draft   │
│ tự liên hệ   │ ──────────────────────── │ bảng so sánh │
│ ⏱ 10'        │                          │ ⏱ 1' 🟢      │
└──────────────┘                          └──────────────┘

🟢 = Human boundary - Học viên review đề xuất và tự gọi chủ nhà cọc tiền
Fallback: AI đề xuất sai thông tin ──> Học viên bỏ qua và tự tìm kiếm thủ công.
```

---

## Problem Cards #2 và #3 — tóm tắt

| Card | Actor | Bottleneck | Metric | Quick gut | Vì sao chưa chọn làm #1 |
|---|---|---|---|---|---|
| Tóm tắt PDF tài liệu khóa học | Tân học viên | Đọc thủ công file PDF giới thiệu khóa học dài chục trang để tìm thông tin lịch học, nội dung chuẩn bị | 30 phút → 2 phút | Workflow | Nỗi đau chưa đủ lớn, học viên nếu cố gắng đọc thì vẫn có thể tự tìm kiếm thông tin được, ít ảnh hưởng trực tiếp đến quyết định đi học bằng việc tìm chỗ ở. |
| Chatbot trả lời Q&A học viên | Ban tổ chức hoặc Tân học viên | Phải liên tục gõ trả lời đi trả lời lại các câu hỏi giống nhau từ nhiều học viên | Phản hồi tức thì; giảm 70% số câu hỏi lặp lại gửi về ban tổ chức | Agent / Workflow | Mang lại lợi ích nhiều hơn cho Ban tổ chức tuyển sinh chứ không giải quyết trực tiếp nỗi đau lớn nhất của học viên là tìm phòng trọ. Ngoài ra AI có rủi ro ảo giác thông tin. |

---

*Bản nộp cá nhân — Nguyễn Việt Hoàng Lương*
