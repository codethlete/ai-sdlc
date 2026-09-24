# Runbook Plan — Phát triển và làm rõ nội dung task

**Trạng thái: Bản nháp chờ Human duyệt.**  
Ngày cập nhật: 2026-09-24.

## 1. Mục đích và đầu ra

**Trong stage Plan, AI cùng Human phát triển và làm rõ nội dung task để thống nhất công việc cần làm và kết quả cần đạt.**

Áp dụng cho phát triển phần mềm, nghiên cứu solution, điều tra lỗi, viết tài liệu và các công việc tương tự. Giữ trọng tâm ở vấn đề, đối tượng sử dụng kết quả, phạm vi, ràng buộc và tiêu chí thành công. Yêu cầu kỹ thuật có sẵn trong đầu vào được giữ lại; chi tiết thiết kế và kế hoạch triển khai được dành cho bước sau.

- **Đầu vào:** nội dung ticket hiện có hoặc mô tả tự do của Human, kèm tài liệu sẵn có nếu liên quan. Không yêu cầu chuẩn bị toàn bộ project context.
- **Đầu ra làm việc:** bản nháp nội dung task để Human sửa và chốt. Có thể lưu thành `task-draft.md` nếu cần review bằng file.
- **Đầu ra chính thức:** nội dung đã chốt được đưa vào ticket Redmine mới hoặc cập nhật ticket hiện có. Redmine là nguồn chính thức sau khi cập nhật.

## 2. Lợi ích kỳ vọng

| Lợi ích | Giá trị |
|---|---|
| Đồng nhất cấu trúc ticket | Đầu vào có thể khác nhau theo người viết hoặc PM; đầu ra có bộ nội dung cốt lõi chung. |
| Cải thiện độ rõ và đầy đủ | AI hỏi phần thiếu, phát hiện mâu thuẫn và ghi lại điều chưa biết. |
| Giảm công soạn thảo | Human cung cấp thực tế; AI tổ chức và diễn đạt thành nội dung dễ review. |
| Dễ bàn giao và đánh giá hoàn thành | Người đọc hiểu cần làm gì, vì sao và dựa vào đâu để xác nhận kết quả. |
| Giữ một nguồn chính thức | Bản nháp phục vụ soạn thảo; ticket quản lý yêu cầu và công việc sau khi chốt. |
| Dùng chung cho code và non-code | Điều chỉnh sản phẩm bàn giao và tiêu chí thành công theo loại task. |

Các lợi ích về thời gian, công sức và bàn giao cần được đo qua sử dụng thực tế; chưa coi là kết quả đã chứng minh.

## 3. Vai trò

- **Human (thường là người nhận ticket):** cung cấp thực tế, chủ động tìm hiểu, trả lời hoặc trao đổi với người tạo ticket/PM, sửa bản nháp và tự đánh giá nội dung đã đủ để bắt đầu chưa.
- **AI:** tổng hợp thông tin, hỏi phần cần thiết, phát hiện thiếu/mâu thuẫn, soạn và kiểm tra bản nháp. Không tự biến suy đoán thành yêu cầu đã chốt.
- **Người tạo ticket/PM:** làm rõ những điểm cần xác nhận. Với ticket khó hoặc phức tạp, PM có thể yêu cầu bước confirm bổ sung; không mặc định thêm bước này cho mọi ticket.

## 4. Các bước thực hiện

### Bước 1 — Đưa thông tin sẵn có

Human cung cấp ticket hoặc mô tả công việc bằng lời của mình. AI đọc và tóm tắt cách hiểu, chỉ ra thông tin đã rõ và phần còn thiếu. Nếu không truy cập được tài liệu, báo lại để Human cung cấp nội dung cần thiết.

Ticket đã đầy đủ có thể đi thẳng đến bản nháp; không hỏi lại chỉ để điền mẫu.

### Bước 2 — Cùng làm rõ

AI kiểm tra: vấn đề, đối tượng, kết quả, sản phẩm bàn giao, phạm vi, ràng buộc và tiêu chí thành công. Mỗi lượt hỏi tối đa 3 câu, ưu tiên điểm ảnh hưởng đến cách hiểu công việc.

- Human trả lời điều mình biết; điều cần xác nhận thì trao đổi với người tạo ticket hoặc PM.
- AI ghi lại câu trả lời, phân biệt thông tin được khẳng định với giả thuyết/câu hỏi mở.
- Thiếu link hoặc ví dụ có thể dùng placeholder và ghi rõ chưa đối chiếu. Không suy ra nội dung của tài liệu chưa đọc.
- Câu hỏi mở không tự động chặn việc tạo bản nháp. Human quyết định thời điểm làm rõ và ảnh hưởng đến việc bắt đầu công việc.
- Nếu cần quá nhiều kiến thức nền, cùng thu hẹp phạm vi hoặc chọn tình huống phù hợp hơn. Ghi lại chi tiết dành cho bước sau.

### Bước 3 — Soạn bản nháp nội dung task

AI nói ngắn mục đích và phạm vi trước khi tạo tài liệu, rồi soạn từ thông tin đã có theo mẫu ở mục 5. Đánh dấu bản nháp chưa duyệt và giữ rõ các điểm chưa xác nhận.

Với ticket có sẵn, đối chiếu để không làm mất yêu cầu, link hoặc chi tiết còn giá trị. Không thêm giải pháp, tiêu chí hay phạm vi chỉ vì AI thấy hợp lý; nếu cần đề xuất, tách rõ để Human quyết định.

### Bước 4 — Human review và chốt

AI kiểm tra trước; Human đọc và sửa theo các câu hỏi:

- Có đúng vấn đề và mục đích công việc không?
- Người đọc có hiểu ai sử dụng kết quả, cần bàn giao gì và phạm vi đến đâu không?
- Tiêu chí thành công có giúp đánh giá kết quả không?
- Có thông tin bị mất, tự thêm hoặc mâu thuẫn với yêu cầu gốc không?
- Các điểm chưa rõ có được ghi đúng, và đã rõ điểm nào cần trả lời trước khi làm tiếp chưa?

Human chốt nội dung theo thẩm quyền thông thường của dự án. Chấp nhận bản mô tả còn câu hỏi mở không đồng nghĩa câu hỏi đó đã được giải quyết hoặc kết quả đã được kiểm chứng.

### Bước 5 — Đưa nội dung đã chốt vào Redmine

Human hoặc AI theo phân công và quyền truy cập tạo ticket mới/cập nhật mô tả ticket hiện có.

1. Kiểm tra khả năng truy lại mô tả cũ; nếu chưa bảo đảm, lưu bản cũ trước khi thay thế.
2. Đưa nội dung đã chốt vào ticket, giữ link/tài liệu liên quan và câu hỏi mở. Bỏ ghi chú chỉ dành cho quá trình soạn thảo.
3. Đọc lại ticket để xác nhận nội dung và định dạng đã được cập nhật đúng.
4. Đánh dấu bản nháp đã chuyển vào ticket, kèm link và thời điểm. Bản lưu này không tiếp tục được duy trì như một nguồn yêu cầu song song.

Sau đó, thay đổi yêu cầu được cập nhật trên Redmine. Nếu tiếp tục dùng bản sao với AI, lấy lại nội dung ticket hiện hành. Chưa cập nhật ticket thì ghi đúng trạng thái “đã chốt bản nháp, chờ cập nhật”, không báo hoàn tất bước này.

## 5. Mẫu nội dung task

Mẫu dùng chung để hỗ trợ tính nhất quán; có thể gộp mục khi ngắn. “Bắt buộc” là cần có nội dung, không bắt buộc một heading riêng. Bản nháp vẫn có thể ghi phần còn thiếu.

| Nội dung | Mức cần thiết | Ý nghĩa |
|---|---|---|
| Vấn đề / nhu cầu | Bắt buộc | Vì sao cần làm công việc này? |
| Đối tượng sử dụng / bị ảnh hưởng | Bắt buộc | Ai dùng kết quả hoặc chịu tác động? |
| Kết quả mong muốn và sản phẩm bàn giao | Bắt buộc | Cần đạt điều gì và bàn giao thứ gì? |
| Phạm vi | Bắt buộc | Bao gồm những gì? Chỉ thêm ngoài phạm vi khi cần tránh hiểu nhầm. |
| Tiêu chí thành công / chấp nhận | Bắt buộc | Dấu hiệu hoặc bằng chứng nào đủ để đánh giá hoàn thành? |
| Ràng buộc | Không bắt buộc mục riêng | Có giới hạn liên quan đã biết thì phải ghi. |
| Tài liệu tham chiếu | Không bắt buộc nếu không có | Có nguồn cần thiết thì dẫn link; thiếu link thì ghi placeholder. |
| Điểm cần làm rõ | Không bắt buộc nếu không còn | Có điều chưa rõ ảnh hưởng đến công việc thì phải ghi, kèm người/bước làm rõ khi đã xác định. |

```markdown
# [Tiêu đề task]

## Mô tả
[Vấn đề/nhu cầu, đối tượng sử dụng và kết quả mong muốn]
[Sản phẩm bàn giao nếu cần nêu riêng]

## Phạm vi
- ...

## Tiêu chí chấp nhận
- ...

## Ràng buộc
- ...

## Tài liệu tham chiếu
- ...

## Điểm cần làm rõ
- [Câu hỏi — người/bước làm rõ nếu đã xác định]
```

Mã/link ticket đặt trong thông tin bản nháp để đối chiếu nếu đã có ticket; không cần lặp trong chính mô tả Redmine.

### Điều chỉnh cho công việc non-code

| Loại task | Sản phẩm bàn giao minh họa | Tiêu chí thành công minh họa |
|---|---|---|
| Nghiên cứu solution | So sánh phương án, đề xuất và bằng chứng thử nghiệm nếu cần | Đủ cơ sở chọn hướng tiếp theo, nêu rõ đánh đổi và hạn chế. Kết luận chưa có phương án phù hợp vẫn có thể đạt nếu đáp ứng mục tiêu nghiên cứu đã chốt. |
| Viết tài liệu | Hướng dẫn cho nhóm người đọc xác định | Người đọc mục tiêu có thể làm theo trong phạm vi đã thống nhất. |
| Điều tra lỗi | Kết quả điều tra, bằng chứng và bước tiếp theo | Đạt mức xác định nguyên nhân hoặc thu hẹp khả năng đã thống nhất; phân biệt bằng chứng với giả thuyết. |

Các ví dụ này là gợi ý, không tự trở thành yêu cầu của mọi task. Với nghiên cứu, nên làm rõ giới hạn thời gian/độ sâu nếu cần để xác định điểm dừng.

## 6. Prompt làm việc giữa Human và AI

Dùng [prompt phát triển và làm rõ nội dung task](../prompts/clarify-task.md). File gồm prompt khởi động và các câu lệnh minh họa cho những lượt tiếp theo.

Copy prompt, thay phần đầu vào bằng ticket hoặc mô tả công việc, rồi trao đổi với AI. Khi cần thay đổi prompt, cập nhật trực tiếp trong file đó.

## 7. Đánh giá sau khi áp dụng

Sau mỗi lần áp dụng, xem lại ba điểm:

- **Chất lượng:** nội dung task có đúng, đủ rõ và còn thông tin tự suy diễn không?
- **Công sức:** Human phải tìm thêm, giải thích và sửa thông tin cho AI đến mức nào?
- **Giá trị sử dụng:** nội dung đã làm rõ giúp thực hiện và bàn giao công việc tốt hơn ở đâu?

Sau khi thực hiện task, có thể xem lại những lần phải hỏi lại hoặc sửa yêu cầu do nội dung ban đầu chưa rõ để điều chỉnh cách làm Plan.
