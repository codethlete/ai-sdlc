# Intent: Tìm hiểu và áp dụng AI Native SDLC vào quy trình hiện tại

**Trạng thái:** BẢN NHÁP — chưa được Human duyệt.
**Ngày khởi tạo:** 2026-09-14.
**Người soạn:** AI, dựa trên README và yêu cầu khởi động stage Plan của Human.
**Người quyết định và duyệt:** Human phụ trách development.

## Cơ sở tham khảo

Đã đọc phần tổng quan và Plan của [The AI-Native SDLC playbook — Anthropic](https://claude.com/blog/the-ai-native-sdlc-playbook) ngày 2026-09-14.

Bài viết đề xuất tích hợp AI xuyên suốt SDLC, giữ trách nhiệm quyết định ở Human. Trong Plan, Human mô tả vấn đề, AI hỏi để làm rõ rồi soạn `intent.md`; Human sửa và duyệt trước khi lưu vào quản lý phiên bản. Nội dung gồm vấn đề, kết quả mong muốn, đối tượng ảnh hưởng, ràng buộc và câu hỏi mở.

Đây là hướng dẫn tham khảo, không phải bằng chứng về thực trạng công ty.

## Những gì đã thống nhất

Các điểm dưới đây lấy từ README và yêu cầu của Human; không đồng nghĩa toàn bộ bản intent này đã được duyệt.

- Bối cảnh: công ty outsourcing; Human phụ trách development cùng AI thực hiện dự án.
- Mục đích: tìm hiểu và xây dựng cách áp dụng AI Native SDLC vào quy trình hiện tại, thực hành phương pháp trên chính dự án này.
- Phạm vi: lần lượt Plan, Design, Build; kiểm tra chất lượng trong từng stage. Chưa tách Test, Deploy, Maintain thành stage riêng.
- Sau mỗi stage, đúc kết guidelines/runbook đơn giản để đội ngũ áp dụng; phân biệt hoạt động thực hiện dự án với bộ hướng dẫn tạo ra.
- Build của dự án tập trung vào tài liệu hướng dẫn, template và prompt mẫu. Áp dụng vào Build phần mềm cần kiểm chứng tiếp trên thay đổi nhỏ của dự án thực tế.
- Human cung cấp bối cảnh, quyết định và duyệt. AI hỏi, phân tích, tổng hợp, soạn và kiểm tra.
- Chat hiện tại chỉ làm Plan; chỉ chuyển stage khi Human xác nhận.
- Human yêu cầu runbook không giới hạn ở Claude/Claude Code: học tinh thần và ý tưởng từ bài viết để áp dụng với các AI coding tool khác nhau.

## Vấn đề cần giải quyết

**Human đã xác nhận ngày 2026-09-14:** Việc phải xây dựng project context là một trở ngại lớn khi áp dụng AI Native SDLC vào dự án đang chạy. Mong muốn giảm công chuẩn bị ban đầu để việc thực hành đơn giản và dễ bắt đầu.

Chưa có ticket cụ thể hoặc số liệu về công chuẩn bị. Không mặc định công ty đang gặp các điểm nghẽn khác nêu trong bài viết.

## Kết quả mong muốn

Định hướng đã có: bộ hướng dẫn đơn giản, rõ ràng, ít thủ tục và dùng được trong công việc.

**Yêu cầu đã xác nhận:** Runbook cho phép bắt đầu mà không cần chuẩn bị sẵn bộ project context. Đã thống nhất hướng dùng ticket Redmine thực tế để thực hành Plan, hỏi bổ sung context cần thiết trong quá trình làm.

**Chưa xác định:** người dùng đầu tiên, ticket thử dùng và tiêu chí thành công có thể kiểm chứng. Chưa kiểm chứng khả năng đáp ứng yêu cầu này ở Plan hoặc các stage khác.

## Đối tượng và ràng buộc

- Đã biết: Human phụ trách development và AI cùng thực hiện; đội ngũ là đối tượng sử dụng ở mức khái quát.
- Ràng buộc đã xác nhận: hướng dẫn không phụ thuộc công cụ. Mô tả cách cộng tác và kết quả cần đạt bằng ngôn ngữ chung; các tính năng/lệnh riêng chỉ dùng làm ví dụ được ghi rõ, không coi là điều kiện bắt buộc. Chưa kiểm chứng trên nhiều công cụ và không mặc định chúng có khả năng tương đương.
- Chưa biết: vai trò sử dụng đầu tiên, quy trình hiện tại, mức sử dụng AI, công cụ, thời gian/nguồn lực và các giới hạn từ công ty hoặc khách hàng có liên quan.

## Cách tiếp tục — đề xuất của AI, chưa duyệt

1. Cùng tìm hiểu Plan từ bài viết: mục đích, các bước, output, quản trị, đo lường và lý do của từng nội dung.
2. Chọn một ticket Redmine có phạm vi nhỏ; bắt đầu bằng nội dung sẵn có và chỉ hỏi thêm context ảnh hưởng đến việc làm rõ intent.
3. Ghi nhận thông tin thiếu; không tự giả định hoặc kết luận intent đủ rõ khi thiếu thông tin quan trọng. Ghi lại phần cần xử lý ở stage sau.
4. Đúc kết runbook Plan từ thực hành; xem xét lượng context phải bổ sung và mức độ dễ bắt đầu. Tiêu chí đánh giá cụ thể chờ Human thống nhất.
5. Xin Human duyệt đầu ra và xác nhận trước khi chuyển sang học stage Design.

Đề xuất đầu ra của feature học Plan: ghi chú tìm hiểu, intent của ticket thực hành và runbook Plan ngắn gọn. File intent hiện tại ghi ý định của dự án xây dựng bộ hướng dẫn, không thay thế intent của ticket. Chưa chọn ticket nên chưa tạo intent thực hành riêng.

## Câu hỏi đang trao đổi

Bước trao đổi tiếp theo: tìm hiểu mục đích và đầu ra của Plan trước khi yêu cầu Human cung cấp ticket hoặc context dự án thực hành.

## Ghi nhận duyệt

Human đã xác nhận hướng thực hành bằng ticket, yêu cầu không phải chuẩn bị sẵn bộ project context và yêu cầu không phụ thuộc AI coding tool cụ thể. Cách tổ chức mỗi chat được Human làm rõ và đã ghi trong README. Chưa có quyết định duyệt toàn bộ intent, runbook Plan hoặc chuyển stage. Các đề xuất còn lại vẫn chưa được duyệt.
