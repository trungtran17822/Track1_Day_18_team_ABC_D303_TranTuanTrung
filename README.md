# Track1_Day18_2A202601769_TranTuanTrung

Repo nộp cá nhân. Tên đúng form: `Track1_Day18_MHV_HoVaTen` → **Track1_Day18_2A202601769_TranTuanTrung**.

Ba thành viên trỏ cùng Design Sheet, bộ prototype A/B/C và Group Feedback Synthesis. File Feedback Note và AI Support Log trong repo này là của **Trần Tuấn Trung** (phiên mình facilitate + Option C).

Worksheet nhóm: [Google Doc Day 18](https://docs.google.com/document/d/129sQqOwMWCGUrT8tdyrtXXI8F9G5mpC6OxVi69YBPcc/edit?tab=t.xwd4tgpjmx1d#heading=h.kn1r76tn3dm5).

## 1. Thông tin cá nhân và nhóm

- **MHV:** 2A202601769
- **Họ và tên:** Trần Tuấn Trung
- **Tên nhóm:** Nhóm Case 2
- **Ba thành viên:** Chu Thị Yến Khanh (Option B); Nguyễn Trọng Đức (Option A); Trần Tuấn Trung (Option C)
- **Case:** Case B – AI Notes: Personal Learning Notes

## 2. Hypothesis Problem

Khi ôn tập lại bài giảng, học sinh đọc các highlight/note trong slide, gặp khó khi tìm hiểu, hiểu lại và tổng hợp vì ghi chú nằm rải rác và khó lấy ngữ cảnh, dẫn đến phải đọc lại toàn bộ slide hoặc tìm trên nền tảng khác, làm tăng thời gian ôn tập.

Cấu trúc: Khi [ôn lại bài có highlight/note], [học viên] gặp khó trong việc [tìm, hiểu lại, tổng hợp dấu vết học tập] vì [rải rác / mất ngữ cảnh], dẫn đến [đọc lại toàn bộ slide hoặc dùng tool khác / tốn thời gian].

**Nối với observation Day 17** (không dùng Practice Notes như validation):

- Người tham gia 001: ghi chú phần chưa hiểu; lúc ôn mất ngữ cảnh, quên note, đọc slide từ đầu để tìm phần bỏ sót.
- Người tham gia 002: ghi chú trên lớp; khi đọc lại không rõ note thuộc nội dung nào hoặc dùng để làm gì.
- Người tham gia 003: highlight chỗ thú vị chứ không chỗ khó; khi ôn thường không quay lại highlight, đọc hết slide rồi nhờ AI tóm tắt/tạo câu hỏi.

**Điều chưa biết / chưa chứng minh:** tần suất và số học viên; thời gian/công sức cụ thể; pain nằm ở phân tán, thiếu ngữ cảnh, quên xem lại hay cách tạo ghi chú ban đầu; hậu quả với hiểu bài, nhớ bài, điểm số. Hypothesis này là điểm xuất phát để test A/B/C, chưa phải problem đã validated.

## 3. Three Solution Options

Cùng target user, situation, task, content fixture và desired outcome. Khác **mechanism** và **cách chia việc user–AI**, không khác màu/layout/wording. Chi tiết: [three-option-design-sheet.md](three-option-design-sheet.md). Hub test: [UI/abc.html](UI/abc.html).

**Task chung (18.CP5):** Trong tình huống này, hãy dùng từng phương án để xác định phần bạn cần xem lại và khôi phục đủ ngữ cảnh để tiếp tục ôn tập mà không phải đọc lại toàn bộ slide.

| Option | Mô tả ngắn | Prototype (mở được trong repo) |
| --- | --- | --- |
| **A – User tự tổ chức** | Gom note về một nơi. Học viên tự phân cụm và tự viết diễn giải. AI Don’t Act. |
| **B – User + AI đồng tạo** | User chọn note → AI đề xuất nhóm/context → user sửa, gộp, tách, reject rồi mới chốt bản ôn. |
| **C – AI gen report, user review** | Có highlight/note hoặc hết bài → AI tự phân cụm thành report có cấu trúc → user sửa, lưu, xóa. | [UI/solution_C.html](UI/solution_C.html) |

Link đủ A/B/C: [prototype-link.md](prototype-link.md).

## 4. Đóng góp của tôi trong nhóm

- **Option chịu trách nhiệm:** Option C — AI Notes report (AI Act, user review). Spec Human–AI trên Design Sheet; micro-prototype `UI/solution_C.html`; thuyết trình [option-c-thuyet-trinh.html](option-c-thuyet-trinh.html).
- **Shared context/content:** Dùng Hypothesis 18.CP1 của nhóm; cùng task 18.CP5; cùng bộ slide Day 18 và cùng 3 highlight + 2 ghi chú + 1 điểm chưa hiểu trên A/B/C.
- **Human–AI decisions (C):** Trước khi AI chạy, banner nói report là bản nháp, có thể gom sai. User làm highlight/note; AI phân cụm và tóm tắt; user sửa / lưu Hộp Báo Cáo / xóa. Evidence: cụm highlight, cụm note, số slide. Recovery: edit, xóa, mở hộp đã lưu. Sau phiên test, thêm nhảy **[Slide n]** về nguồn vì tester hỏi điều đó.
- **Facilitation / observation:** Test cả A/B/C với một tester ngoài nhóm. Ghi Feedback Note của **chính phiên mình facilitate** trong [prototype-feedback-note.md](prototype-feedback-note.md) (Bản 3 trên worksheet).
- **Tổng hợp feedback:** Đóng góp hàng Feedback 3 và Next Change/Still Unproven vào [group-feedback-synthesis.md](group-feedback-synthesis.md). Không chọn option thay tester.

## 5. Prototype Feedback

**Phiên mình facilitate** — [prototype-feedback-note.md](prototype-feedback-note.md)

- First action: click Hộp Báo Cáo, scroll slide, dò các nút.
- Do dự: sau khi note, không biết report lưu ở đâu; sau khi lưu, hỏi ấn mục ghi chú trong report có dẫn lên slide chứa ghi chú không.
- Evidence: kiểm tra kỹ chức năng và đọc nội dung report AI đưa ra.
- Option chọn: **C**, vì muốn report sinh ngay khi highlight/note. Trade-off với A: A phải tự gom và tự cụm.
- Chống kỳ vọng: bản raw còn cơ bản.

**Ba-feedback synthesis** — [group-feedback-synthesis.md](group-feedback-synthesis.md)

- Pattern: cả ba tester dò UI bằng thao tác, không đọc hướng dẫn; flow chưa tự giải thích.
- Khác biệt: Khanh’s tester chọn B (sửa được output, chấp nhận nhiều bước); Đức’s tester chọn A (sợ AI hiểu sai giảng viên); tester của mình chọn C (tốc độ).
- Không đếm “thích C”. Không tuyên bố solution đã validated.

**Next Change (nhóm, không nói quá evidence):** Giữ ba cơ chế. Sửa interaction C: link note/highlight → slide nguồn và làm rõ Hộp Báo Cáo là nơi lưu (đã gắn trên C). Làm rõ progression bước trên B/A vì cả ba lạc flow.

**Still Unproven:** Ba người có hoàn thành *task ôn tập* hay chỉ khám phá UI; C có giảm việc đọc lại cả deck không; user có bắt AI tóm tắt sai không; mức automation nào đúng ngoài ba tester; Next Change chưa test lại.

Hai note còn lại: [feedback/feedback-note-tester-001.md](feedback/feedback-note-tester-001.md) (Đức), [feedback/feedback-note-tester-002.md](feedback/feedback-note-tester-002.md) (Khanh).

## 6. AI Support Log

Xem [ai-support-log.md](ai-support-log.md).

Tóm tắt: AI giúp khung nộp bài, copy UI C, sắp lớp OBSERVED/INTERPRETED. AI sai khi gắn C thành Review Map (khác worksheet). Tôi tự chốt C = AI gen report; Next Change = provenance + chỗ lưu; không bịa quote; không chọn C thắng vì mình phụ trách C.

---

## Năm gate — tự kiểm

| Gate | Đạt khi | Trong repo này |
| --- | --- | --- |
| 1. Evidence Continuity | HP nối Day 17 + điều chưa biết | Mục 2: 001/002/003 + chưa đo tần suất/hậu quả. Practice Notes không coi là validation. |
| 2. Meaningful Options | Cùng problem/task, khác mechanism/role | A Don’t Act / B Ask / C Act. Distance check trên Design Sheet. |
| 3. Human Control | Expectation, agency, evidence, recovery | Từng option trên Design Sheet; banner trên A/B/C. |
| 4. Test-ready | Tester tự dùng A/B/C cùng task | [UI/abc.html](UI/abc.html); task trên đầu mỗi prototype. C đầy đủ slide viewer; A/B cùng fixture và cùng nhiệm vụ. |
| 5. Learning | 3 notes, pattern, Next Change, Still Unproven | Không “ba người thích B”; không tuyên bố validated. |

## Checklist trước khi nộp

- [x] Sáu file tối thiểu ở thư mục gốc.
- [x] README đủ sáu phần; có **Đóng góp của tôi trong nhóm**.
- [x] Design Sheet, A/B/C, Feedback Note cá nhân, Group Synthesis mở được từ README.
- [x] Ba prototype cùng user, situation, task, content, desired outcome.
- [x] Mỗi thành viên test A/B/C với một người khác; đủ ba Feedback Notes.
- [x] Synthesis tách pattern, Next Change, Still Unproven.
- [x] AI Support Log của người nộp.
- [ ] Đổi tên folder/GitHub thành `Track1_Day18_2A202601769_TranTuanTrung` nếu remote vẫn mang tên khác.
- [ ] Đặt repo public / cấp quyền giảng viên-TA.
