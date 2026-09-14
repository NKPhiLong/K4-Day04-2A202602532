# Danh sách thành viên nhóm & Phân công nhiệm vụ

- **Tên nhóm / Repository:** K4-Day04-2A202602532
- **Đề tài:** IT Helpdesk Agent (Prompt Engineering & Tool Calling)

| STT | Họ và tên | Mã sinh viên | GitHub Username | Vai trò chính |
|:---:|---|:---:|---|---|
| 1 | Nguyễn Khắc Phi Long | 2A202602532 | `NKPhiLong` | Nhóm trưởng, Tool Implementation & Tích hợp hệ thống |
| 2 | Nguyễn Văn Sơn | 2A202602744 | `nvs` (`Nos Kaiser`) | Prompt Engineer (Tối ưu System Prompt, Behavior Boundaries & Versioning) |
| 3 | Lê Đức Tùng | 2A202603005 | `tungld` | QA / Eval Designer (Thiết kế bộ dữ liệu kiểm thử nhóm `eval_group.json`) |
| 4 | Trần Thị Thuý | 2A202602960 | `thuyannie2310` | Security & Adversarial Evaluator (Bảo mật ranh giới & Đánh giá tấn công) |

---

## Phân công nhiệm vụ chi tiết

### 1. Nguyễn Khắc Phi Long (Nhóm trưởng)
- Quản lý repository chung, phân chia nhánh và merge pull request của các thành viên.
- Rà soát tool implementations, đảm bảo các tool helpdesk hoạt động ổn định.
- Hoàn thiện checkout cuối cùng trước khi nộp bài trên VLearn.

### 2. Nguyễn Văn Sơn (Prompt Engineer)
- Chịu trách nhiệm chính về artifact `starter_v0/artifacts/system_prompt.md`.
- Tối ưu hóa prompt từ `v0` đến `v12`: ép native tool call, chuẩn hóa `clarify`, chống role spoofing và fake confirmation, ngăn chặn rò rỉ credential, xử lý multi-turn carry-over & cancellation, sửa regression (H17, H19).
- Quản lý nhật ký thí nghiệm `starter_v0/artifacts/version_log.csv`.
- Đóng góp nội dung B1 (Version evidence), B2 (Failure analysis), B7 (Technical reflection) và C2 (Self-reflection) trong `REPORT.md`.

### 3. Lê Đức Tùng (QA / Eval Designer)
- Thiết kế đúng 10 test cases nguyên bản (5 single-turn, 5 multi-turn) trong `starter_v0/data/eval_group.json`.
- Chạy đánh giá và ghi nhận metric cho bộ group eval suite.

### 4. Trần Thị Thuý (Security Evaluator)
- Đánh giá bộ adversarial suite (12 cases), rà soát thủ công tool execution results và thư mục `tickets/`.
- Xử lý retry 429 cho model provider trong `gemini_provider.py`.
- Hoàn thiện mục B4a (Adversarial evidence) và B6 (Safety review) trong `REPORT.md`.
