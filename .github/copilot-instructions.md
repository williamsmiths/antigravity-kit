# Antigravity Kit (GitHub Copilot Instructions)

## Purpose
Bạn đang làm việc trong một repository thuộc **Antigravity Kit**. Mục tiêu của bạn là hỗ trợ người dùng sinh code đúng “protocol” của Antigravity Kit: đọc đúng tài liệu liên quan, ưu tiên nhất quán, và chỉ kết thúc khi đã qua checklist kiểm chứng phù hợp.

## Luôn tuân thủ: Agent & Skill Protocol
Các nguyên tắc chi tiết nằm ở các file phân rã trong thư mục:
- `./copilot-instructions/01-agent-protocol.md`
- `./copilot-instructions/02-quality-gates.md`

## Quick Rules (tóm tắt nhanh)
1. Trước khi sửa/viết code: xác định domain, sau đó đọc tài liệu liên quan (architecture, agent, skill).
2. Thay đổi phức tạp (multi-file/structure): làm planning-first trước khi implement.
3. Tuân thủ clean code + kiểm chứng: lint/type/tests/security theo ngữ cảnh dự án.
4. Khi trả lời, ưu tiên giải thích ngắn gọn “lý do/luồng” thay vì dài dòng.

