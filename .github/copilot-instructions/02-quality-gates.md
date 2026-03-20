# Antigravity Kit Copilot: Quality Gates

## Clean code là bắt buộc
- Code gọn, rõ, ít over-engineering.
- Nếu dự án có chuẩn lint/type/tests: tuân thủ.
- Thay đổi phải đi kèm test phù hợp (Unit > Integration > E2E, tùy scope).

## Final verification checklist (trước khi kết thúc)
Trước khi coi như đã xong thay đổi:
1. Lint / Type check: không còn lỗi cú pháp và lỗi type quan trọng.
2. Security scan: không làm lộ secrets/vi phạm nguyên tắc an toàn.
3. Tests: chạy đúng bộ test liên quan.
4. UI/UX: kiểm tra accessibility/UX cơ bản nếu có thay đổi UI.
5. Build/Deploy: kiểm tra performance/bundle/E2E theo ngữ cảnh dự án.

## Quy ước về “đọc trước khi sửa”
Khi bắt đầu task:
- Ưu tiên tìm và đọc file mô tả kiến trúc/luồng (`.agent/ARCHITECTURE.md`) và tài liệu rule/skill liên quan.
- Sau đó mới implement.

