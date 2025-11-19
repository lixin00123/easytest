# 1. Sprint Goal（冲刺目标）

EN: Sprint Goal: Implement and test a simple addition function that correctly returns the sum of two numbers.  
CN: 冲刺目标：实现并测试一个简单的加法函数，能够正确返回两个数字的和。

---

# 2. Mini-ADR（迷你架构决策记录）

Decision（决策）：  
EN: Use Python and pytest to test the addition function.  
CN: 使用 Python 和 pytest 来测试加法函数。

Reason（原因）：  
EN: They are simple, already configured in the project, and suitable for small exercises.  
CN: 它们简单易用，已经在项目中配置好，非常适合小型练习。

Consequence（结果）：  
EN: Enables quick feedback on whether the addition function works correctly.  
CN: 可以快速反馈加法函数是否工作正确。

---

# 3. Mini-API Description（迷你 API 描述）

Endpoint（接口）：  
EN: POST /add  
CN: POST /add（加法计算接口）

Request（请求）：  
EN: { "a": number, "b": number }  
CN: { "a": 数字, "b": 数字 }（两个需要相加的数字）

Success（成功响应）：  
EN: 200 OK, { "result": a + b }  
CN: 200 OK，返回 { "result": a + b }（结果为两数之和）

Fail（失败响应）：  
EN: 400 Bad Request (if parameters are missing or invalid)  
CN: 400 Bad Request（当参数缺失或无效时）

Description（说明）：  
EN: Calculates the sum of two numbers and returns the result.  
CN: 计算两个数字的和，并返回计算结果。
