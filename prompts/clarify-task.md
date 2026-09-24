# Prompt Plan — Phát triển và làm rõ nội dung task

## Prompt khởi động

Copy prompt dưới đây và thay phần đầu vào bằng nội dung ticket hoặc mô tả tự do. Không cần chuẩn bị đủ mọi mục trước khi bắt đầu. Prompt dùng độc lập được; nếu có template riêng của đội, gửi kèm để AI áp dụng.

```text
Hãy cùng tôi phát triển và làm rõ nội dung task để đưa lên Redmine.

Đầu vào:
[Dán nội dung ticket hiện có hoặc mô tả công việc; kèm tài liệu sẵn có nếu có]

Cách làm:
- Bắt đầu bằng cách tóm tắt ngắn điều bạn hiểu. Nếu thiếu hoặc mâu thuẫn,
  hỏi tối đa 3 câu mỗi lượt, ưu tiên điểm cần làm rõ để tiếp tục.
- Làm rõ vấn đề, đối tượng sử dụng kết quả, kết quả mong muốn, sản phẩm
  bàn giao, phạm vi, ràng buộc và tiêu chí thành công. Điều chỉnh theo
  loại task: coding, nghiên cứu, điều tra lỗi, viết tài liệu, v.v.
- Dùng lại thông tin đã có, không hỏi lại chỉ để điền mẫu. Chỉ yêu cầu
  thêm project context khi cần giải quyết một điểm chưa rõ cụ thể.
- Ghi lại câu trả lời của tôi. Không tự suy đoán yêu cầu; phân biệt
  thông tin đã được khẳng định, đề xuất của bạn và điều còn chưa rõ.
- Nếu tôi chưa có câu trả lời hoặc muốn để sau, ghi câu hỏi mở hoặc
  placeholder và tiếp tục soạn nháp. Nêu ảnh hưởng nếu có để tôi quyết định.
- Giữ các yêu cầu kỹ thuật có sẵn; chưa đi vào thiết kế hay triển khai.

Khi đủ thông tin hoặc khi tôi yêu cầu, soạn bản nháp gồm:
1. Tiêu đề.
2. Mô tả: vấn đề, đối tượng, kết quả mong muốn và sản phẩm bàn giao.
3. Phạm vi.
4. Tiêu chí chấp nhận.
5. Ràng buộc, tài liệu tham chiếu và điểm cần làm rõ nếu có.

Viết ngắn gọn, có thể gộp mục nếu phù hợp. Kiểm tra bản nháp với đầu vào
để tránh mất thông tin hoặc tự thêm yêu cầu. Đánh dấu chưa duyệt để tôi
sửa và chốt. Sau khi chốt, xuất nội dung sẵn để đưa vào Redmine;
chỉ cập nhật trực tiếp lên Redmine khi tôi yêu cầu.
```

## Các lượt tiếp theo

Human trả lời và sửa bằng ngôn ngữ tự nhiên; không cần prompt riêng cho mỗi bước. Có thể dùng các câu sau khi phù hợp:

| Tình huống | Câu lệnh minh họa |
|---|---|
| Chưa có thông tin | “Phần này tôi chưa rõ, ghi câu hỏi mở và tiếp tục soạn nháp.” |
| Muốn xem bản nháp sớm | “Soạn bản nháp từ thông tin hiện có, đánh dấu phần còn thiếu.” |
| Sửa cách hiểu | “Ý đúng là […]. Cập nhật bản nháp và kiểm tra các mục liên quan.” |
| Rà soát trước khi chốt | “Đối chiếu bản nháp với đầu vào và các câu trả lời của tôi; chỉ ra thông tin bị mất, tự thêm hoặc mâu thuẫn.” |
| Chốt nội dung | “Tôi chốt bản này, giữ các câu hỏi mở như đã ghi. Xuất nội dung để tôi đưa vào Redmine.” |
