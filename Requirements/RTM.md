# MATRIX TRACEABILITY REQUIREMENTS (RTM) - DỰ ÁN E-OFFICE HÒA PHÁT

Bảng dưới đây thể hiện sự truy vết từ Nhu cầu kinh doanh (Needs) -> Tính năng (Features) -> Yêu cầu chi tiết (UC/SUP) -> Kịch bản kiểm thử (Test Cases).

| Requirement ID | Requirement Description | Category | Trace to (Feature/UC) | Trace to (Test Case) | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **BR-01** | Quản lý công văn đến/đi | Functional | Fe-01, UC-01 | TC-01, TC-02 | Approved |
| **BR-02** | Phê duyệt điện tử nhiều cấp | Functional | Fe-02, UC-05 | TC-05 | Approved |
| **BR-06** | Hỗ trợ thông minh bằng AI | Functional | Fe-AI, UC-09 | TC-AI-01 | Approved |
| **UR-01** | Hiệu suất phản hồi < 3 giây | Non-Functional | SUP-3.3.12 | TC-PERF-01 | Approved |
| **UR-02** | Độ tin cậy (Uptime 99.5%) | Non-Functional | SUP-3.3.11 | TC-REL-01 | Approved |
| **UR-03** | Bảo mật HTTPS & RBAC | Non-Functional | SUP-3.3.11 | TC-SEC-01 | Approved |
| **UR-04** | Xác thực mạnh 2FA (Admin) | Non-Functional | SUP-3.3.11 | TC-SEC-02 | Approved |
| **UR-05** | Tương thích đa trình duyệt | Non-Functional | SUP-3.3.13 | TC-SUPP-01 | Approved |
| **UR-06** | Khả năng phục hồi (60 phút) | Non-Functional | SUP-3.3.11 | TC-REL-02 | Approved |

---

### Ghi chú mã hiệu:
* **BR:** Business Requirement (Nhu cầu kinh doanh)
* **UR:** Usability/Reliability/Security Requirement (Yêu cầu phi chức năng từ mục 3.3)
* **SUP:** Supplementary Reference (Tham chiếu đến tài liệu yêu cầu bổ sung)
* **TC:** Test Case (Kịch bản kiểm thử tương ứng)
