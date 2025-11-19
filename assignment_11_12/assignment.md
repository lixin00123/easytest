# Sprint Goal（冲刺目标）

EN: Sprint Goal: Implement core pet adoption request workflow, enabling users to submit adoption requests through the system.
CN: 冲刺目标：实现宠物领养请求的核心流程，使用户能够通过系统提交领养申请。

---

# Mini-ADR（迷你架构决策记录）

Decision（决策）:
EN: Use a REST-based API design.
CN: 使用基于 REST 的 API 设计。

Reason（原因）:
EN: It is simple, widely used, and easy to integrate with frontend applications.
CN: 它简单易用，应用广泛，并且易于与前端集成。

Consequence（结果）:
EN: Faster development speed and a consistent structure for future endpoints.
CN: 开发速度更快，并为未来的端点保持一致结构。

---

# Mini-API Description（迷你 API 描述）

Endpoint（接口）:
EN: POST /adoptions/request
CN: POST /adoptions/request（提交领养请求）

Request（请求格式）:
EN: { pet_id, user_id, message }
CN: { pet_id, user_id, message }（包含宠物 ID、用户 ID、留言）

Success（成功响应）:
EN: 201 Created
CN: 201 Created（创建成功）

Fail（失败响应）:
EN: 400 Bad Request
CN: 400 Bad Request（错误请求）

Description（说明）:
EN: Creates a new adoption request submitted by a registered user.
CN: 用于创建注册用户提交的新宠物领养申请。
