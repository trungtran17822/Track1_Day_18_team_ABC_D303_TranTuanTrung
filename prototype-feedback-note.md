# Prototype Feedback Note — Trần Tuấn Trung (Option C)

Nguồn ghi chép: worksheet 18.CP6 Bản 3, phiên mình facilitate khi tester dùng prototype Option C (AI Notes report).

## Tester / context

- **Facilitator:** Trần Tuấn Trung
- **Option mình phụ trách và demo chính:** C — AI tự tổng hợp highlight/ghi chú thành report có cấu trúc; user xác nhận, sửa hoặc xóa.
- **Relevant context (18.CP5):** Hỏi ngắn liệu tester từng ghi chú/highlight rồi khi ôn không nhớ ngữ cảnh hoặc phải đọc lại nhiều slide.
- **Task đưa cho tester:** Xác định phần cần xem lại và khôi phục đủ ngữ cảnh để tiếp tục ôn tập mà không phải đọc lại toàn bộ slide. Không giải thích icon. Không hỏi “Bạn có thích không?”

## OBSERVED — Tester đã làm hoặc nói gì?

| Observation focus | Ghi chép |
| --- | --- |
| **First action** | Click phần Hộp Báo Cáo (reports box), scroll chuột giữa các slide và bấm các button trên giao diện. |
| **Chỗ dừng / do dự / hiểu sai** | Sau khi note xong, tester do dự không biết report sẽ lưu vào đâu. Sau khi ấn lưu, hộp report hiện ra; tester lại hỏi: khi ấn vào mục ghi chú trong report thì có dẫn lên slide chứa ghi chú đó hay không. |
| **Evidence đọc hay bỏ qua** | Tester kiểm tra khá kỹ từng chức năng trên giao diện và đọc lại nội dung trong report do AI Notes đưa ra. |
| **Cách sửa / lấy lại control** | Tester nêu mong muốn có đường dẫn từ mục trong report về slide chứa ghi chú. (Mong muốn “AI Notes hiện cạnh ghi chú” và “thêm agent tổng hợp slide + note” được ghi trong worksheet là nhu cầu sau trải nghiệm / có trộn với tester khác — không coi là hành vi đã thực hiện trên UI.) |
| **Option được chọn** | C |
| **Lý do và trade-off** | Tester chọn C vì cho rằng ngay khi ghi chú hoặc highlight, report sẽ được tạo ngay. Trade-off so với A: A bắt user tự gom ghi chú và tự sắp xếp theo cụm, chậm hơn. |
| **Evidence chống lại kỳ vọng nhóm** | Tester nhận xét bản raw hơi cơ bản, cần phát triển thêm mới tối ưu được. |

## INTERPRETED — Điều đó có thể nghĩa gì?

- Tester chưa biết button nào dùng để làm gì nên khám phá toàn bộ giao diện trước, không đọc hướng dẫn.
- Tester mong muốn mỗi phần ghi chú trong report chứa đường dẫn lên slide nguồn — provenance, không chỉ bản tóm tắt.
- Tester ưu tiên tốc độ và tự động hóa; chấp nhận ít thao tác thủ công hơn A.
- Flow “ghi chú → report sinh ra → lưu vào hộp” chưa tự giải thích: không rõ report sống ở đâu và note có nhảy về slide không.
- “Hài lòng” khi đọc report chưa phải evidence rằng C giảm thời gian ôn hay khôi phục đúng ngữ cảnh.

## DECIDED — NEXT CHANGE (từ phiên này)

Giữ cơ chế C (AI Act → user review) nhưng sửa hai interaction breakdown đã quan sát:

1. Mỗi highlight/ghi chú trong report (và trong Hộp Báo Cáo) có nút **[Slide n]** nhảy về đúng slide nguồn.
2. Sau khi lưu, hệ thống nói rõ report nằm ở nút **Hộp Báo Cáo Đã Lưu** trên thanh trên.

Đã gắn vào [UI/solution_C.html](UI/solution_C.html). Chưa đổi C thành A hoặc B: tester đã chọn C vì tốc độ, không vì map hay inbox.

## STILL UNPROVEN (một người)

- Tester khác có cũng chọn C, hay chỉ người ưu tiên automation?
- C có giúp hoàn thành task “không đọc lại toàn bộ slide” hay chỉ tạo cảm giác có report?
- User có phát hiện khi AI gom/tóm tắt sai không, hay chỉ đọc report rồi hài lòng?
- Bản “cơ bản” cần thêm gì mới đủ dùng sau buổi học thật — chưa đo.
