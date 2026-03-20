# Antigravity Kit Copilot: Agent & Skill Protocol

## Mục tiêu
Đảm bảo bạn luôn làm việc theo “protocol” của Antigravity Kit:
- Đọc đúng tài liệu liên quan trước khi viết/thiết kế
- Chọn đúng agent/skill theo domain
- Áp dụng quy tắc clean code và kiểm chứng phù hợp

## Đọc gì trước khi làm
Trước khi thực hiện bất kỳ thay đổi code/design nào:
1. Đọc `.agent/ARCHITECTURE.md` để nắm luồng agents/skills/scripts.
2. Xác định agent phù hợp với domain yêu cầu.
3. Đọc file agent tương ứng trong `.agent/agents/`.
4. Đọc skill `SKILL.md` (hoặc các phần liên quan) trong `.agent/skills/`.

## Request classification (phân loại yêu cầu)
- Question/Explain: tập trung vào giải thích tri thức, không sinh patch code.
- Small edit: bám checklist “context check” và chỉ đụng phần liên quan.
- Complex build/create/refactor: chuyển sang “planning-first”.

## Planning-first cho thay đổi phức tạp
Với yêu cầu nhiều phần (multi-domain, multi-file, hoặc ảnh hưởng cấu trúc):
1. Phân rã nhiệm vụ (what/why/constraints).
2. Tạo plan rõ ràng: mốc bước, output mong đợi.
3. Chỉ sau khi plan đủ rõ mới bắt đầu implement.

## Intelligent agent routing (xác định agent theo domain)
- Tự xác định domain: `frontend`, `backend`, `database`, `security`, `testing`, `devops`, `debugging`, `planning`.
- Nếu nhiều domain: ưu tiên phương án orchestrate (tách luồng rồi hợp nhất kết quả).

## Thông tin/đầu ra nên ưu tiên
- Trả lời ngắn gọn theo luồng “lý do/tiến trình”.
- Khi cần, chỉ ra agent/skill logic nào đang được áp dụng ở mức mô tả.

