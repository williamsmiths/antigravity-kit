# Antigravity Kit (Cursor Rules)

## Mục tiêu
- Giúp bạn tạo và chỉnh sửa code theo đúng “protocol” của Antigravity Kit.
- Ưu tiên tính nhất quán, chất lượng, và khả năng kiểm chứng trước khi viết code trên nhiều file.

## Bắt buộc đọc tài liệu liên quan trước khi làm
Trước khi tạo/đổi code hoặc thiết kế:
1. Đọc `.agent/ARCHITECTURE.md` để nắm luồng agents/skills/scripts.
2. Xác định agent phù hợp với domain yêu cầu.
3. Đọc agent `.md` tương ứng trong `.agent/agents/`.
4. Đọc skill `SKILL.md`/các phần có liên quan trong `.agent/skills/`.

## Request classification (phân loại yêu cầu)
- If là câu hỏi/giải thích: trả lời theo hướng mô tả kiến thức, không sinh patch code.
- If là sửa lỗi / thêm một thay đổi nhỏ: chỉ cần tập trung vào file liên quan, bám checklist “context check”.
- If là build/create/refactor hoặc thay đổi có nhiều phần: chuyển sang “planning-first”.

## Planning-first cho thay đổi phức tạp
Với yêu cầu “complex” (multi-domain, nhiều file, hoặc ảnh hưởng cấu trúc):
1. Phân rã nhiệm vụ (what/why/constraints).
2. Tạo một plan/timeline theo cấu trúc rõ ràng (mốc bước, output mong đợi).
3. Chỉ sau khi plan đủ rõ mới bắt đầu implementation.

## Intelligent agent routing (tự chọn hướng làm)
- Tự xác định domain: `frontend`, `backend`, `database`, `security`, `testing`, `devops`, `debugging`, `planning`.
- Nếu cần nhiều domain: ưu tiên cách làm “orchestrate” (tách luồng, sau đó hợp nhất kết quả).

## Clean code rules (bắt buộc)
- Viết code gọn, rõ ràng, hạn chế over-engineering.
- Mọi thay đổi nên kèm test phù hợp (Unit > Integration > E2E nếu dự án có).
- Không thêm giải pháp tạm bợ cho vấn đề cốt lõi.

## Final verification checklist (bắt buộc trước khi kết thúc)
Trước khi coi như xong thay đổi:
1. Lint/Type check: không còn lỗi cú pháp và lỗi type quan trọng.
2. Security scan: không để lộ secrets/vi phạm nguyên tắc an toàn.
3. Tests: chạy đúng bộ test liên quan (ít nhất unit/integration, tùy scope).
4. Nếu là UI/UX: kiểm tra accessibility/UX cơ bản.
5. Nếu là build/deploy: kiểm tra thêm performance/bundle/E2E theo ngữ cảnh dự án.

## Quy ước thông tin khi bạn là “assistant” của Antigravity Kit
- Khi bắt đầu trả lời theo hướng “thực thi dự án”, hãy nêu rõ agent/skills logic nào đang được dùng (ở dạng mô tả ngắn).

