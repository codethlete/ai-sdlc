# Prompt khởi động stage Plan

Chúng ta cùng thực hiện dự án “Tìm hiểu và áp dụng AI Native SDLC vào quy trình hiện tại”.

Hãy đọc `README.md` trong thư mục dự án để nắm bối cảnh và các quy ước đã thống nhất.

Mỗi stage được tìm hiểu trong một chat riêng. Chat này chỉ tìm hiểu và thực hành stage **Plan**. Việc “Tìm hiểu và áp dụng stage Plan” là một feature của dự án xây dựng bộ hướng dẫn AI Native SDLC.

Lấy nguồn từ mục **Tài liệu tham khảo** trong `README.md`; tài liệu này có thông tin về tất cả các stages.

Hãy mở link trong mục đó, đọc phần tổng quan và phần liên quan đến stage Plan trước khi trao đổi. Dùng nội dung đó làm cơ sở, đồng thời điều chỉnh theo bối cảnh và các quyết định của dự án. Phân biệt rõ hướng dẫn từ bài viết với đề xuất của bạn. Nếu không truy cập được, hãy báo để tôi cung cấp nội dung.

Chúng ta học tinh thần và ý tưởng của bài viết, không giới hạn ở Claude hay Claude Code. Runbook cần mô tả mục đích, vai trò Human/AI, đầu vào, đầu ra và cách kiểm tra bằng ngôn ngữ không phụ thuộc công cụ. Lệnh hoặc tính năng riêng, nếu cần, chỉ là ví dụ được ghi rõ; không mặc định mọi AI coding tool có cùng khả năng.

Thực hiện lần lượt:

1. **Tìm hiểu:** Cùng đọc và giải thích mục đích của Plan, các bước làm, output, cách quản trị và đo lường. Với mỗi nội dung, làm rõ vì sao cần có nó, không chỉ liệt kê thao tác. Trao đổi từng phần, không trình bày toàn bộ runbook ngay từ đầu.
2. **Thực hành:** Khi đã hiểu đủ để bắt đầu, dùng một ticket Redmine của dự án đang chạy do Human cung cấp. Bắt đầu từ nội dung ticket sẵn có, không yêu cầu chuẩn bị trước bộ project context/knowledge. AI xác định thông tin còn thiếu và hỏi từng bước, ưu tiên thông tin ảnh hưởng đến vấn đề, kết quả mong muốn, phạm vi và ràng buộc. Ghi lại câu trả lời để dùng tiếp; không tự suy đoán. Nếu thiếu thông tin quan trọng, giữ rõ trạng thái chưa xác định. Nếu ticket cần quá nhiều kiến thức nền, cùng Human cân nhắc thu hẹp hoặc chọn ticket khác. Chi tiết chỉ cần cho Design/Build được ghi lại để xử lý sau.
3. **Đúc kết:** Từ phần học và thực hành, cùng tạo runbook Plan ngắn gọn, ít thủ tục, dễ áp dụng. Kiểm tra cả chất lượng đầu ra và công sức bổ sung context. Phân biệt điều đã kiểm chứng trên ticket với đề xuất chưa thử; không kết luận đã áp dụng được cho mọi công cụ hoặc dự án.

Phân biệt ba loại nội dung: tài liệu về dự án xây dựng bộ hướng dẫn, intent của ticket thực hành, và runbook hướng dẫn đội ngũ thực hiện Plan. Không dùng intent của dự án xây dựng bộ hướng dẫn thay cho intent của ticket. Trước khi tạo artifact, giải thích ngắn mục đích và phạm vi của nó. Không nhầm stage Plan với kế hoạch triển khai `plan.md` thuộc Build trong bài viết.

Trước tiên, chỉ tóm tắt cách bạn hiểu mục tiêu và cách học/thực hành đã thống nhất; phân biệt những gì đã thống nhất và những gì cần làm rõ. Sau đó dừng lại, chờ Human xác nhận hoặc điều chỉnh. Chỉ khi Human xác nhận cách hiểu này mới chuyển sang bước tìm hiểu mục đích và đầu ra của Plan từ tài liệu tham khảo; chưa yêu cầu ticket hay context dự án thực hành ngay. Trao đổi từng bước, ưu tiên một câu hỏi quan trọng nhất mỗi lần; không tự giả định bối cảnh công ty.

Lưu bản nháp và kết quả vào tài liệu dự án, phân biệt rõ nội dung chưa duyệt và đã duyệt. Chỉ chuyển sang stage tiếp theo khi tôi xác nhận.
