# 02 — Group Problem Statement

## PHASE 3: Group Convergence (Hội tụ và chọn 1 bài toán)

**1. Các nhóm ý tưởng ban đầu của các thành viên:**
Nhóm chúng tôi có 4 người, mỗi người đưa ra 3 ý tưởng, tổng cộng có 12 ý tưởng. Chúng tôi gom lại thành 4 nhóm chính như sau:
*   Nhóm báo cáo: Tự động gom thông tin để viết báo cáo tiến độ hàng tuần.
*   Nhóm tìm kiếm: Tìm nhanh tài liệu bị trôi trên tin nhắn hoặc hệ thống công ty.
*   Nhóm kiểm tra lỗi: Đọc lại các bản thảo tài liệu hoặc mã nguồn để tìm chỗ sai sót.
*   Nhóm nhắc việc: Tự động theo dõi và nhắc nhở thời hạn hoàn thành công việc.

**2. Đánh giá và chọn lọc:**
Chúng tôi cùng chấm điểm các ý tưởng dựa trên độ rõ ràng của quy trình, hậu quả có đo đếm được không, và mức độ hiểu biết của cả nhóm về công việc đó. 

**3. Quyết định cuối cùng (Deliverable):**
Nhóm thống nhất chọn bài toán **Viết báo cáo tiến độ hàng tuần**. 

Lý do chọn bài toán này:
*   Các bước làm việc cực kỳ rõ ràng, ai cũng hình dung được.
*   Thời gian hao phí đếm được chính xác bằng phút.
*   Có thể đem đi hỏi thăm đồng nghiệp xung quanh rất dễ dàng để xác nhận nỗi đau này là có thật.
*   Dễ dàng vẽ ra được sơ đồ quy trình trước và sau khi áp dụng máy móc vào hỗ trợ.

---

## PHASE 4: Validation + Research (Kiểm chứng và Nghiên cứu giải pháp)

**1. Tín hiệu kiểm chứng (Validation):**
Nhóm đã đem ý tưởng này đi hỏi nhanh 3 người quản lý dự án quen biết và làm 1 khảo sát nhỏ với 6 bạn trong lớp. 
*   Xác nhận: Đa số mọi người đều thừa nhận việc đi gom nhặt số liệu từ nhiều nơi rồi ngồi gõ lại thành một đoạn văn trơn tru là việc cực kỳ tốn thời gian và nhàm chán.
*   Phản bác: Một vài người cho rằng họ chỉ cần nhìn bảng số liệu (dashboard) là đủ, không cần thiết phải đọc chữ dài dòng.
*   Bài học rút ra: Vấn đề thật sự không phải là việc lấy số liệu, mà là việc phải chuyển đổi những con số khô khan đó thành một đoạn văn bản tóm tắt tình hình, có điểm nhấn để cấp trên đọc hiểu ngay.

**2. Nghiên cứu giải pháp đã có (Research):**
Chúng tôi tìm hiểu xem trên thị trường đã có công cụ nào làm được việc này chưa:
*   Các công cụ báo cáo có sẵn của hệ thống công ty: Chỉ xuất ra được con số khô khan, không tự động viết thành câu chữ phân tích tình hình được.
*   Các trợ lý đọc tin nhắn tự động: Chỉ tóm tắt được nội dung trong phần mềm nhắn tin, không gom được dữ liệu từ các phần mềm quản lý công việc khác.
*   Phần mềm đọc tài liệu tự động: Tóm tắt rất tốt nhưng dễ bịa thêm thông tin, bắt buộc phải có người ngồi đọc lại để kiểm tra.

Kết luận sau khi nghiên cứu: Chúng tôi không nên xây dựng một hệ thống hoàn toàn tự động tự chạy đi tìm số rồi tự gửi báo cáo đi. Cách an toàn và hợp lý nhất là tạo ra một quy trình: Tự động kéo dữ liệu về một chỗ -> Trí tuệ nhân tạo (AI) sẽ viết nháp đoạn văn -> Người thật đọc lại, chỉnh sửa rồi mới bấm nút gửi.

---

## PHASE 5: Workflow + Problem Statement v0

**1. Sơ đồ quy trình (Workflow trước và sau):**

Quy trình hiện tại làm thủ công (Tốn 90 phút)
*   Xuất dữ liệu từ phần mềm quản lý công việc (10 phút)
*   Lấy số liệu đo lường từ bảng tính Excel (10 phút)
*   Đọc tóm tắt tin nhắn trao đổi trong tuần (15 phút)
*   Gom tất cả thông tin vào một file tài liệu chung (15 phút)
*   Ngồi gõ thành văn bản báo cáo hoàn chỉnh (25 phút) -> Đây chính là khâu tắc nghẽn nhất.
*   Đọc lại và căn chỉnh cho đẹp (10 phút)
*   Gửi email cho cấp trên (5 phút)

Quy trình tương lai kỳ vọng (Tốn 21 phút)
*   Hệ thống tự động kéo tất cả dữ liệu về (2 phút)
*   AI gom nhóm dữ liệu theo cấu trúc (1 phút)
*   AI tự động viết bản nháp báo cáo (1 phút)
*   Người làm báo cáo đọc lại và chỉnh sửa (15 phút) -> Đây là chốt chặn an toàn bắt buộc.
*   Người làm báo cáo bấm nút gửi (2 phút)

**2. Problem Statement v0 (Phát biểu bài toán bước đầu):**

*   **Người thực hiện:** Nhân viên quản lý dự án phụ trách việc gửi báo cáo hàng tuần cho ban giám đốc.
*   **Quy trình:** Mỗi tuần phải đi xuất dữ liệu, lấy số liệu từ bảng tính, đọc tin nhắn, gom vào file tài liệu, ngồi gõ thành văn bản, đọc dò lại và gửi email.
*   **Khâu tắc nghẽn:** Khâu ngồi gõ từ những dữ liệu thô thành một văn bản hoàn chỉnh mất tới 25 phút vì người làm phải tự suy nghĩ xem nên viết gì cho hay.
*   **Hậu quả:** Tổng cả quá trình mất 90 phút mỗi tuần cho một người. Báo cáo làm lâu dễ bị trễ giờ họp, khiến cấp trên không nắm được tình hình kịp thời.
*   **Mục tiêu cải thiện:** Giảm tổng thời gian làm báo cáo từ 90 phút xuống dưới 30 phút. 
*   **Giới hạn của AI:** AI tuyệt đối không được tự động bấm gửi email, không được tự động bịa ra số liệu, và không được quyết định thay người làm báo cáo. Nó chỉ được dùng dữ liệu đã cung cấp để viết nháp.

---

## PHASE 6: Rule / Workflow / Agent + Decision

**1. Lựa chọn mức độ can thiệp:**

*   **Luật cứng (Rule):** Dùng biểu mẫu có sẵn và điền số liệu tự động. Cách này không giải quyết được việc mỗi tuần tình hình dự án diễn biến khác nhau, cần văn phong miêu tả khác nhau.
*   **Tác nhân tự chủ (Agent):** Cho AI tự chạy đi dò hỏi khắp các phần mềm, tự phân tích và tự gửi báo cáo luôn. Cách này quá rủi ro vì AI có thể gửi sai số liệu lên ban giám đốc và vượt quá tầm kiểm soát.
*   **Quy trình có AI hỗ trợ (Workflow):** Viết đoạn mã để tự gom dữ liệu, sau đó nhờ AI viết nháp đoạn văn, cuối cùng người thật đọc lại. Đây là cách giải quyết an toàn, hợp lý và tuyến tính nhất. 

Chúng tôi chọn mức **Workflow**.

**2. Problem Statement v1 (Bản hoàn chỉnh):**

*   **Người thực hiện:** Nhân viên quản lý dự án phụ trách báo cáo hàng tuần.
*   **Quy trình:** Xuất dữ liệu -> Lấy số liệu -> Đọc tin nhắn -> Gom dữ liệu -> Viết thành văn -> Kiểm tra lại -> Gửi.
*   **Khâu tắc nghẽn:** Việc suy nghĩ và gõ thành văn bản từ dữ liệu thô mất 25 phút và dễ gây trễ giờ.
*   **Hậu quả:** Tốn 90 phút mỗi tuần, làm báo cáo trễ khiến cuộc họp thiếu thông tin nền tảng.
*   **Mục tiêu cải thiện:** Giảm thời gian xuống dưới 30 phút, đảm bảo số lần sếp phải hỏi lại để làm rõ thông tin không bị tăng lên.
*   **Giới hạn của AI:** AI không tự gửi báo cáo, không bịa số, không quyết định thay con người.
*   **Điểm AI can thiệp:** Ngay sau khi dữ liệu thô được gom lại, AI sẽ nhảy vào để viết nháp trước khi người làm báo cáo bắt tay vào tự viết.
*   **Mức độ chọn:** Quy trình có AI hỗ trợ (Workflow).
*   **Rủi ro và chốt chặn con người:** Rủi ro lớn nhất là AI bịa chuyện hoặc viết văn quá nhạt nhẽo. Chốt chặn bắt buộc là người thật phải đọc kiểm tra kỹ từng con số và chỉnh sửa lại câu từ trước khi gửi.

**3. Quyết định cuối cùng (Decision):**

**Quyết định: GO (Thực hiện dự án này).**

Lý do:
*   Vấn đề rất thực tế, quy trình các bước cực kỳ rõ ràng, mục tiêu thời gian đo lường được bằng phút.
*   Hệ thống có sự kết hợp của việc làm tự động bằng máy (không dùng AI) ở bước kéo dữ liệu, và chỉ dùng AI ở đúng khâu viết nháp. AI không thâu tóm toàn bộ quy trình.
*   Có sự tham gia kiểm duyệt của con người rõ ràng ở bước cuối, triệt tiêu được rủi ro phát ngôn bậy bạ lên ban giám đốc.

Nếu dự án này mà chạy ra văn bản quá tệ khiến người làm báo cáo phải ngồi viết lại từ đầu hơn 70% nội dung liên tục trong 2 tuần, chúng tôi sẽ hủy dự án và quay về cách làm thủ công cũ.
