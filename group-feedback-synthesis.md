# Group Feedback Synthesis

Nguồn: bảng 18.CP6 trên [worksheet nhóm](https://docs.google.com/document/d/129sQqOwMWCGUrT8tdyrtXXI8F9G5mpC6OxVi69YBPcc/edit?tab=t.xwd4tgpjmx1d#heading=h.kn1r76tn3dm5). Không tuyên bố solution đã validated.

## Nguồn evidence

| Phiên | Facilitator | Feedback Note | Option tester chọn |
| --- | --- | --- | --- |
| Feedback 1 | Chu Thị Yến Khanh | [feedback/feedback-note-tester-001.md](feedback/feedback-note-tester-001.md) | B |
| Feedback 2 | Nguyễn Trọng Đức | [feedback/feedback-note-tester-002.md](feedback/feedback-note-tester-002.md) | A |
| Feedback 3 | Trần Tuấn Trung | [prototype-feedback-note.md](prototype-feedback-note.md) | C |

Mỗi thành viên test cả A/B/C với một tester ngoài nhóm. Cùng task 18.CP5.

## Pattern và khác biệt

| Nội dung | Feedback 1 (Khanh) | Feedback 2 (Đức) | Feedback 3 (Trung / Option C) | Pattern hoặc khác biệt |
| --- | --- | --- | --- | --- |
| First action | Ấn ngay nút Generate để xem AI tạo tài liệu. | Click thử các button và chức năng trên giao diện. | Click report box, scroll slide và thử các button. | Cả 3 khám phá bằng thao tác trực tiếp, không đọc hướng dẫn trước. Tester 1 tập trung sớm vào output AI; tester 2 và 3 khám phá nhiều chức năng hơn. |
| Breakdown chính | Không hiểu flow 3 bước: chọn note → AI tổng hợp/sửa → tạo bản cuối. | Do dự lần đầu dùng note; chưa hiểu cơ chế các bước. | Không rõ report lưu ở đâu; hỏi note trong report có nhảy về slide gốc không. | Flow chưa tự giải thích. Feedback 3 cho thấy nhu cầu liên kết output với nguồn note. |
| Cách lấy lại control | Chọn note đầu vào và chỉnh nội dung AI trước khi tạo bản cuối. | Tự bôi đen, ghi chú, đi từng luồng để hiểu cơ chế. | Muốn link về slide gốc; (worksheet còn ghi mong muốn AI cạnh note / agent — không gộp thành hành vi đã làm). | Cả ba muốn kiểm tra hoặc tác động quá trình tạo nội dung, nhưng hình thức khác nhau: sửa trực tiếp, thao tác thủ công, hoặc provenance. |
| Option được chọn | B | A | C | Không có option thắng tuyệt đối. Mỗi tester ưu tiên một mức tự động hóa khác nhau. |
| Trade-off | Nhiều bước hơn để giữ quyền chọn input và sửa output. | Đơn giản và kiểm soát nội dung, dù phải tự làm nhiều hơn. | Tốc độ và tự động hóa, ít thao tác thủ công. | Trục control ↔ automation: A control, C automation, B ở giữa. |

## Evidence chống lại kỳ vọng nhóm

Cả ba phiên cho thấy giả định “flow nhiều bước / UI tự giải thích được” không đúng. Tester của Option C còn nói bản raw quá cơ bản.

## Group Next Change

- **Thay đổi:** Giữ ba cơ chế A/B/C (không chọn một option thay tester). Sửa interaction của C: đường dẫn note/highlight → slide nguồn, và làm rõ chỗ lưu report. Song song, làm rõ progression các bước trên B (và A) vì cả ba tester đều lạc flow.
- **Evidence dẫn tới quyết định:** Feedback 3 hỏi thẳng “ấn ghi chú trong report có lên slide không” và do dự chỗ lưu; cả ba first-action là click dò UI; không ai cho một option thắng.
- **Không làm:** Không bỏ C vì “bản raw cơ bản”; không tuyên bố C tốt hơn vì tester của mình chọn C.

## Still Unproven sau ba feedback

- Ba tester có hoàn thành được *task ôn tập* (tìm đúng phần cần xem, khôi phục ngữ cảnh, không đọc lại cả deck) hay chỉ khám phá UI?
- Mức automation nào phù hợp ngoài ba người này.
- AI phân cụm/tóm tắt có đủ đúng trên nội dung học thật không.
- Link về slide (Next Change của C) có hết do dự hay không — chưa test lại.
- Pain Day 17 có giảm thời gian ôn hay không; chưa đo.
