# 02 — Group Problem Statement

## PHASE 3: Group Convergence (Hội tụ và chọn 1 bài toán)

**1. Các nhóm ý tưởng ban đầu của các thành viên:**
Nhóm chúng tôi có 4 người, mỗi người đưa ra 3 ý tưởng, tổng cộng có 12 ý tưởng. Chúng tôi gom lại thành 5 nhóm chính như sau:
* Nhóm báo cáo: Tự động gom thông tin để viết báo cáo tiến độ tuần của lead dev hoặc tiến độ thí nghiệm.
* Nhóm tìm kiếm: Tìm trọ và tiện ích cho học viên, tra cứu tài liệu học tập, trích xuất tài liệu chương trình.
* Nhóm kiểm tra lỗi: Đọc lại bản thảo hoặc code để tìm chỗ sai sót.
* Nhóm nhắc việc: Tự động theo dõi và nhắc nhở thời hạn hoàn thành công việc.
* Nhóm lọc dữ liệu: Lọc nhiễu trajectory từ mô phỏng học tăng cường.

**2. Đánh giá và chọn lọc:**
Chúng tôi cùng chấm điểm các ý tưởng dựa trên độ rõ ràng của quy trình, hậu quả có đo đếm được không, và mức độ hiểu biết của cả nhóm về công việc đó.

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Tìm phòng trọ & tiện ích | 5 | 5 | 5 | 5 | 5 | 5 | 5 | 35 |
| Báo cáo tiến độ tuần | 4 | 5 | 4 | 4 | 4 | 4 | 4 | 29 |
| Lọc noise trajectory | 4 | 4 | 3 | 4 | 3 | 4 | 3 | 25 |

Lý do chọn bài toán này:
* Có quy trình các bước tương tác rõ ràng, đối chiếu vị trí trọ trên bản đồ và thông tin trên mạng xã hội.
* Thời gian hao phí đếm được chính xác bằng ngày và giờ thực tế, từ 3 ngày xuống dưới 15 phút.
* Có thể đem đi hỏi thăm các học viên khác cùng khóa ở tỉnh xa để xác nhận nỗi đau này là có thật.
* Dễ dàng vẽ ra được sơ đồ quy trình trước và sau khi áp dụng máy móc vào hỗ trợ.

Vì sao không chọn các candidate còn lại:
* Báo cáo tiến độ tuần: Dù quy trình rõ nhưng các thành viên trong nhóm không phải ai cũng có dữ liệu thực tế hoặc hiểu sâu về dự án để chạy thử trong buổi thực hành.
* Lọc noise trajectory: Học tăng cường có miền kiến thức quá hẹp, các thành viên khác trong nhóm khó lòng đóng góp và rất khó chứng minh hay demo nhanh trong buổi thực hành ngắn ngủi.

**3. Quyết định cuối cùng (Deliverable):**
Nhóm thống nhất chọn bài toán **Tìm phòng trọ và tiện ích xung quanh trường**.

---

## PHASE 4: Validation + Research (Kiểm chứng và Nghiên cứu giải pháp)

**1. Tín hiệu kiểm chứng (Validation):**
Nhóm đã đem ý tưởng này đi hỏi nhanh 5 học viên cùng khóa ở xa tới học và thực hiện một khảo sát nhỏ với 8 bạn trong lớp.
* Xác nhận: Đa số mọi người đều thừa nhận việc đi gom nhặt thông tin phòng trọ từ nhiều bài đăng Facebook rồi tra cứu khoảng cách trên bản đồ là việc cực kỳ tốn thời gian và gây stress.
* Phản bác: Một vài bạn cho biết họ đăng ký ở ký túc xá hoặc ăn uống tại canteen trường nên không gặp khó khăn nhiều về tiện ích.
* Bài học rút ra: Vấn đề thật sự không phải là việc thiếu phòng trọ để thuê, mà là việc dữ liệu bị phân mảnh dữ dội. Học viên phải tự đối chiếu thủ công giá cả trên Facebook với vị trí và khoảng cách trên Google Maps.

**2. Nghiên cứu giải pháp đã có (Research):**
Chúng tôi tìm hiểu xem trên thị trường đã có công cụ nào làm được việc này chưa:
* Google Maps API: Tìm vị trí và tính khoảng cách chính xác thực tế, nhưng dữ liệu phòng trọ cho thuê rất nghèo nàn và thiếu thông tin liên hệ hay giá cả.
* NotebookLM / RAG: Hỏi đáp rất tốt bám sát tài liệu Handbook của nhà trường, nhưng không thể truy xuất các dữ liệu động bên ngoài như tin tuyển phòng trên mạng xã hội.
* Facebook Groups: Nguồn cung cấp tin đăng dồi dào, cập nhật liên tục nhưng tin rác nhiều, thông tin phi cấu trúc, không có định vị chính xác.

Kết luận sau khi nghiên cứu: Chúng tôi không nên xây dựng một hệ thống hoàn toàn tự động tự đàm phán cọc tiền do rủi ro pháp lý và lừa đảo tài chính lớn. Cách an toàn và hợp lý nhất là tạo ra một quy trình: Tự động kéo dữ liệu về bằng script hoặc API -> Trí tuệ nhân tạo sẽ viết nháp bảng so sánh đề xuất -> Học viên tự xem xét rồi mới chủ động liên hệ.

---

## PHASE 5: Workflow + Problem Statement v0

**1. Sơ đồ quy trình (Workflow trước và sau):**

Quy trình hiện tại làm thủ công (Tốn 3 ngày)
* Học viên nhận thông báo trúng tuyển khóa học (1 phút)
* Đọc PDF tài liệu giới thiệu trường để nắm địa chỉ (30 phút)
* Lên Facebook tìm kiếm trọ, hỏi giá và lọc tin rác (2 ngày) -> Đây chính là khâu tắc nghẽn nhất.
* Lên Google Maps tra cứu khoảng cách địa lý và tiện ích xung quanh (4 tiếng) -> Đây cũng là khâu gây rối thông tin.
* Đến tận nơi khảo sát thực tế và đặt cọc phòng (1 ngày)

Quy trình tương lai kỳ vọng (Tốn 15 phút)
* Học viên nhận thông báo kèm link chatbot (1 phút)
* Nhập ngân sách và nhu cầu tiện ích lên hệ thống (1 phút)
* Hệ thống tự động truy vấn database trọ và gọi API bản đồ (2 phút)
* AI tự động viết nháp bảng so sánh đề xuất (1 phút) -> Đây là điểm AI can thiệp hỗ trợ.
* Học viên đọc bảng so sánh và tự liên hệ chủ nhà đặt cọc (10 phút) -> Đây là chốt chặn an toàn bắt buộc.

**2. Problem Statement v0 (Phát biểu bài toán bước đầu):**

* **Người thực hiện:** Tân học viên khóa học chuẩn bị nhập học từ tỉnh xa phải chuyển nhà và tự tìm phòng trọ mới gần giảng đường.
* **Quy trình:** Nhận thông báo trúng tuyển → Đọc PDF tài liệu trường → Tìm phòng trọ trên hội nhóm Facebook → Tra Google Maps khoảng cách → Đi xem thực tế và chốt phòng.
* **Khâu tắc nghẽn:** Bước đối chiếu thủ công thông tin phòng trọ trên Facebook với khoảng cách và tiện ích xung quanh trên Google Maps mất quá nhiều thời gian và công sức ghi chép.
* **Hậu quả:** Học viên mất 3 ngày mệt mỏi, stress trước khi nhập học; nhà trường có rủi ro bị rơi rụng học viên do rào cản đi lại và điều kiện chỗ ở lạ lẫm.
* **Mục tiêu cải thiện:** Giảm thời gian tìm ra danh sách 3 phòng trọ phù hợp nhu cầu và ngân sách từ 3 ngày xuống dưới 15 phút.
* **Giới hạn của AI:** AI tuyệt đối không được tự động cọc tiền hay nhắn tin chốt nhà thay cho học viên vì quyết định tài chính thuộc về người dùng. Nó chỉ được dùng dữ liệu đã cung cấp để viết nháp.

---

## PHASE 6: Rule / Workflow / Agent + Decision

**1. Lựa chọn mức độ can thiệp:**

* **Luật cứng (Rule):** Bản đồ tĩnh chứa danh sách nhà trọ cố định do trường cung cấp. Cách này không giải quyết được tính cá nhân hóa theo ngân sách và nhanh bị lỗi thời do hết phòng.
* **Tác nhân tự chủ (Agent):** Cho AI tự chạy đi chat với các chủ nhà trên Facebook để hỏi phòng trống, tự thương lượng giá và tự động đặt cọc. Cách này quá rủi ro về mặt pháp lý, lừa đảo tài chính và khó kiểm soát hành vi AI.
* **Quy trình có AI hỗ trợ (Workflow):** Viết script/API để tự gom dữ liệu và tính khoảng cách, sau đó nhờ AI viết nháp bảng đề xuất, cuối cùng học viên review. Đây là cách giải quyết an toàn, hợp lý và tuyến tính.

Chúng tôi chọn mức **Workflow**.

**2. Problem Statement v1 (Bản hoàn chỉnh):**

* **Người thực hiện:** Tân học viên khóa học chuẩn bị nhập học từ tỉnh xa.
* **Quy trình:** Nhận thông báo → Nhập nhu cầu lên Bot → AI Workflow xử lý database và Map API → Học viên review bảng đề xuất → Tự liên hệ chủ nhà.
* **Khâu tắc nghẽn:** Bước đối chiếu thông tin phòng trọ và khoảng cách địa lý mất quá nhiều thời gian và gây stress.
* **Hậu quả:** Tốn 3 ngày chuẩn bị; gây nản lòng cho học viên ở xa; ảnh hưởng đến tỷ lệ nhập học thực tế.
* **Mục tiêu cải thiện:** Giảm thời gian tìm ra 3 phòng trọ tối ưu xuống dưới 15 phút; giảm 70% câu hỏi lặp đi lặp lại gửi về ban tổ chức.
* **Giới hạn của AI:** AI không tự bịa thông tin phòng trọ; không tự động cọc tiền; học viên phải tự liên hệ xác nhận.
* **Điểm AI can thiệp:** Sau khi Bot nhận nhu cầu học viên và lấy dữ liệu thô kết hợp database và Map API, AI sẽ viết nháp narrative và đánh giá tiện ích.
* **Mức độ chọn:** Quy trình có AI hỗ trợ (Workflow).
* **Rủi ro và chốt chặn con người:** Rủi ro lớn nhất là AI bịa thông tin hoặc đề xuất phòng trọ đã đóng cửa. Chốt chặn bắt buộc là học viên phải tự gọi điện xác nhận lại với chủ trọ trước khi đến.

**3. Quyết định cuối cùng (Decision):**

**Quyết định: GO (Thực hiện dự án này).**

Lý do:
* Vấn đề rất thực tế, quy trình các bước cực kỳ rõ ràng, mục tiêu thời gian đo lường được bằng phút.
* Hệ thống có sự kết hợp của việc làm tự động bằng máy ở bước kéo dữ liệu, và chỉ dùng AI ở đúng khâu viết nháp. AI không thâu tóm toàn bộ quy trình.
* Có sự tham gia kiểm duyệt của con người rõ ràng ở bước cuối, triệt tiêu được rủi ro cọc tiền nhầm lẫn hoặc lừa đảo.

Nếu dự án này chạy ra thông tin sai lệch lớn hoặc học viên vẫn phải tự lên Facebook tìm kiếm lại từ đầu liên tục trong 2 tuần, chúng tôi sẽ dừng sử dụng AI và quay về cách làm thủ công cũ.
