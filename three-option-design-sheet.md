# Three-option Design Sheet

Nguồn: [Day 18 worksheet](https://docs.google.com/document/d/129sQqOwMWCGUrT8tdyrtXXI8F9G5mpC6OxVi69YBPcc/edit?tab=t.xwd4tgpjmx1d#heading=h.kn1r76tn3dm5) · 18.CP1–CP3. Option C do Trần Tuấn Trung phụ trách.

## Shared test context (18.CP2 — quyết định chung)

| Thành phần | Quyết định chung cho A/B/C |
| --- | --- |
| **Target user** | Học viên có ghi chú hoặc highlight trong lúc học và quay lại ôn tập sau buổi học. |
| **Situation** | Sau buổi học, học viên mở lại tài liệu để ôn và cần hiểu lại các ghi chú/highlight đã tạo trước đó. |
| **Task** | Xác định nhanh nội dung cần xem lại và khôi phục đủ ngữ cảnh của ghi chú/highlight để tiếp tục ôn tập. |
| **Desired outcome** | Học viên biết cần xem lại nội dung nào và hiểu ghi chú/highlight đang nói về phần nào mà không phải đọc lại toàn bộ slide. |
| **Content/data fixture** | Cùng một bộ slide mẫu và cùng các ghi chú/highlight đã được tạo trong quá trình học để dùng cho cả ba prototype A/B/C. |

**Hypothesis Problem (18.CP1):** Khi ôn tập lại bài giảng, học sinh đọc qua các highlight đã có note trong slide, gặp khó trong việc tìm hiểu, hiểu lại và tổng hợp các ghi chú/highlight vì chúng nằm rải rác, khó lấy lại ngữ cảnh, dẫn đến phải đọc lại toàn bộ slide hoặc tìm trên nền tảng khác và tăng thời gian ôn tập.

**Evidence Day 17 hỗ trợ:** Cả ba học viên đều dùng highlight. Học viên 1 và 2 không tìm hết ghi chú hoặc không hiểu ngữ cảnh khi về ôn. Học viên 3 highlight phần thú vị, không highlight chỗ khó, và khi ôn vẫn đọc lại toàn bộ slide.

**Chưa chứng minh:** Tần suất, quy mô học viên, thời gian/công sức cụ thể; pain nằm ở phân tán, thiếu ngữ cảnh, quên quay lại hay cách tạo ghi chú ban đầu; hậu quả với hiểu bài, nhớ bài, điểm số.

**Outcome task khi test (18.CP5):** “Trong tình huống này, hãy dùng từng phương án để xác định phần bạn cần xem lại và khôi phục đủ ngữ cảnh để tiếp tục ôn tập mà không phải đọc lại toàn bộ slide.”

## Option A — User tự tổ chức (USER CREATES)

- **Người phụ trách:** Nguyễn Trọng Đức
- **Prototype:** https://github.com/Ntduc112/Track1_Day_18_team_ABC_D303_NguyenTrongDuc
- **Core mechanism:** Hệ thống gom ghi chú về một nơi; học viên tự phân cụm và tự viết diễn giải. Không dùng AI.
- **User làm:** Tự phân loại, nhóm và tổng hợp diễn giải ghi chú.
- **AI làm:** Không.
- **Trigger:** Học viên chủ động chọn Tổng hợp ghi chú.
- **Trade-off:** Kiểm soát hoàn toàn nội dung; tốn công sức và thời gian.
- **Human–AI:** Don’t Act. Mỗi ghi chú giữ nguyên văn, tên bài, slide nguồn, thời gian tạo; không suy luận. Recovery: thêm/sửa/xóa, phân loại, gộp/tách, hoàn tác trước khi lưu.

## Option B — User + AI đồng tạo (CO-CREATE)

- **Người phụ trách:** Chu Thị Yến Khanh
- **Prototype:** https://github.com/Lsdfs/Track1_Day_18_2A202601739_ChuThiYenKhanh
- **Core mechanism:** User chọn note/highlight muốn ôn → AI đề xuất nhóm theo chủ đề và gợi ý context còn thiếu → user chỉnh, thêm/bỏ và xác nhận từng nhóm trước khi tạo bản ôn tập.
- **User làm:** Chọn dấu vết đưa vào ôn tập; xem nhóm AI đề xuất; sửa, gộp, tách, thêm hoặc bỏ trước khi xác nhận.
- **AI làm:** Phân nhóm, tìm context liên quan, đề xuất cấu trúc; không tự chốt bản cuối.
- **Trigger:** User chủ động bắt đầu phiên “Tạo nội dung ôn tập” và chọn dữ liệu.
- **Trade-off:** Giảm công sức nhưng vẫn giữ agency; nhiều thao tác xác nhận/chỉnh sửa hơn C.
- **Human–AI:** AI Ask/Recommend. Mỗi nhóm cho thấy note/highlight nào được dùng; chỗ không chắc đánh dấu cần xác nhận. Recovery: edit, merge, split, remove, reject từng đề xuất hoặc dừng.

## Option C — AI tạo report, user review (AI ACT)

- **Người phụ trách:** Trần Tuấn Trung
- **Prototype:** [UI/solution_C.html](UI/solution_C.html)
- **Core mechanism:** Học viên hoàn thành bài / ghi highlight và note trên slide → AI tự phân cụm, chọn lọc → report có cấu trúc → user xác nhận, sửa hoặc xóa.
- **User làm:** Highlight và ghi chú trên slide; bước cuối xác nhận, sửa hoặc xóa report.
- **AI làm:** Sau khi nhận highlight/ghi chú, tự phân cụm và gen report; hỏi user có lưu không.
- **Trigger:** Học viên hoàn thành bài học (kết thúc buổi / kết thúc slide). Report cập nhật khi có highlight/note mới.
- **Trade-off:** AI có thể phân cụm/tóm tắt sai ý học viên → cần User Control và tốn thời gian kiểm tra; có thể hallucinate.
- **Expectation:** Banner trên prototype nói rõ đây là bản nháp do AI tổng hợp, không phải outline chính thức; user phải sửa/lưu/xóa.
- **Agency:** Sửa report, lưu vào Hộp Báo Cáo, xóa và tạo bản mới. Highlight/note trong report có đường dẫn về slide nguồn (bổ sung sau phiên test).
- **Evidence & uncertainty:** Report tách cụm highlights và cụm ghi chú, có tóm tắt; vẫn hỏi user trước khi lưu. Số slide trên từng mục là căn cứ nguồn.
- **Recovery:** Edit trực tiếp rồi lưu; xóa report; mở Hộp Báo Cáo; bấm slide nguồn để quay lại task ôn tập trên nội dung gốc.

## Distance check

- **A khác B vì** A không dùng AI còn B dùng AI đề xuất nhóm nhưng user chọn input và chốt bản cuối.
- **B khác C vì** B do user khởi tạo phiên và xác nhận từng nhóm trước khi tạo bản; C do AI chạy khi có highlight/note và khi hết bài, user chủ yếu review report.
- **A khác C vì** A user tự tổ chức toàn bộ; C AI tổ chức trước rồi user sửa, lưu hoặc xóa.

Spectrum: USER CREATES (A) → USER + AI CO-CREATE (B) → AI CREATES / USER REVIEWS (C).
