# Tìm hiểu và áp dụng AI Native SDLC vào quy trình hiện tại

**Trạng thái:** Đang thực hiện stage Plan — bản nháp chưa duyệt, chưa chuyển sang Design.

## Bối cảnh và mục đích

Dự án tìm hiểu và xây dựng cách áp dụng AI Native SDLC vào quy trình phát triển phần mềm hiện tại của công ty outsourcing. Người phụ trách development (Human) và AI cùng thực hiện dự án bằng chính phương pháp AI Native SDLC.

## Phạm vi

Chỉ tập trung vào ba stage, thực hiện lần lượt:

1. **Plan:** Làm rõ vấn đề, mục tiêu, phạm vi và tiêu chí thành công.
2. **Design:** Thiết kế quy trình cộng tác giữa Human và AI.
3. **Build:** Tạo và thử dùng bộ tài liệu hướng dẫn, template và prompt mẫu.

Kiểm tra chất lượng được thực hiện trong từng stage. Dự án chưa triển khai Test, Deploy và Maintain thành các stage riêng.

## Cách làm và đầu ra mong muốn

- Tìm hiểu từng stage, đối chiếu với thực tế công ty và thực hành ngay trên dự án này.
- Sau mỗi stage, đúc kết một guidelines/runbook đơn giản, dễ hiểu và có thể dùng ngay trong công việc.
- Phân biệt cách chúng ta thực hiện dự án với bộ tài liệu hướng dẫn được tạo ra để đội ngũ áp dụng.
- Mỗi stage có đầu ra cụ thể và được Human duyệt trước khi chuyển sang stage tiếp theo.

Trong dự án này, Build tập trung vào bộ tài liệu thực hành. Việc áp dụng cho Build phần mềm cần được kiểm chứng tiếp trên một thay đổi nhỏ của dự án thực tế.

## Quy ước cộng tác

- **Human:** Cung cấp bối cảnh công ty, điều chỉnh nội dung, quyết định và duyệt đầu ra.
- **AI:** Hỗ trợ đặt câu hỏi, phân tích, tổng hợp, soạn thảo và kiểm tra.
- Ưu tiên nội dung ngắn gọn, rõ ràng, ít thủ tục và dễ áp dụng.
- Các chi tiết chưa xác định sẽ được làm rõ trong stage tương ứng, không tự coi là đã thống nhất.

## Trạng thái tài liệu

README này ghi lại những thống nhất ban đầu, chưa thay thế cho đầu ra của stage Plan.

[intent.md](intent.md) là bản nháp đang trao đổi trong stage Plan; chưa được duyệt. Vấn đề cụ thể, người dùng runbook và tiêu chí thành công đang chờ làm rõ.

Các tài liệu `spec.md` và `plan.md` sẽ được tạo khi thực hiện đến bước tương ứng. Theo tài liệu tham khảo, `plan.md` là kế hoạch thực hiện thuộc Build, khác với stage Plan đang thực hiện ở đây.

## Tài liệu tham khảo

- [The AI-Native SDLC playbook — Anthropic](https://claude.com/blog/the-ai-native-sdlc-playbook)
