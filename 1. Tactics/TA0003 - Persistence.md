---
title: Persistence
mitre_id: TA0003
tags:
  - mitre-attack
  - tactic
  - persistence
---
---
# Persistence
**Persistence** là kỹ thuật giúp kẻ tấn công duy trì quyền truy cập vào hệ thống, ngay cả sau khi bị khởi động lại hoặc thay đổi thông tin đăng nhập, các sự kiện khác có thể làm gián đoạn quyền truy cập. Các kỹ thuật persistence bao gồm thay thế hoặc chiếm quyền điều khiển mã hợp pháp, cấu hình lại hệ thống, hoặc thêm mã khởi động để hệ thống tự động thực thi mã độc mỗi khi hoạt động trở lại.

## Techniques

| Technique                                          | Description                                                                   |
| -------------------------------------------------- | ----------------------------------------------------------------------------- |
| [[T1078 - Valid Accounts]]                         | Sử dụng tài khoản hợp lệ để duy trì truy cập vào hệ thống.                    |
| [[T1136 - Create Account]]                         | Tạo tài khoản mới để tiếp tục truy cập vào hệ thống.                          |
| [[T1098 - Account Manipulation]]                   | Sửa đổi tài khoản để giữ hoặc nâng cao quyền truy cập.                        |
| [[T1543 - Create or Modify System Process]]        | Tạo hoặc thay đổi tiến trình hệ thống để thực thi mã độc.                     |
| [[T1546 - Event Triggered Execution]]              | Thực thi mã khi có sự kiện hệ thống cụ thể xảy ra.                            |
| [[T1037 - Boot or Logon Initialization Scripts]]   | Thêm mã độc vào script khởi động hoặc đăng nhập.                              |
| [[T1053 - Scheduled Task/Job]]                     | Tạo hoặc sửa đổi tác vụ định kỳ để thực thi mã.                               |
| [[T1505 - Server Software Component]]              | Thay đổi thành phần phần mềm máy chủ để thực thi mã độc.                      |
| [[T1547 - Boot or Logon Autostart Execution]]      | Tự động thực thi mã khi hệ thống khởi động hoặc người dùng đăng nhập.         |
| [[T1031 - Modify Existing Service]]                | Sửa đổi dịch vụ hợp pháp để chèn mã độc.                                      |
| [[T1050 - New Service]]                            | Tạo dịch vụ mới để thực thi mã độc.                                           |
| [[T1548 - Abuse Elevation Control Mechanism]]      | Lợi dụng cơ chế kiểm soát đặc quyền để thiết lập persistence.                 |
| [[T1055 - Process Injection]]                      | Chèn mã vào tiến trình hợp pháp để duy trì hiện diện.                         |
| [[T1205 - Traffic Signaling]]                      | Dùng lưu lượng mạng đặc biệt để kích hoạt hành vi persistence.                |
| [[T1003 - OS Credential Dumping]]                  | Trích xuất thông tin xác thực để tái sử dụng đăng nhập hệ thống.              |
| [[T1036 - Masquerading]]                           | Ngụy trang mã độc dưới dạng tiến trình hoặc tệp hợp lệ.                       |
| [[T1112 - Modify Registry]]                        | Thay đổi các khoá registry để thiết lập persistence.                          |
| [[T1015 - Accessibility Features]]                 | Lạm dụng tính năng trợ năng để kích hoạt truy cập hoặc thực thi mã.           |
| [[T1183 - Image File Execution Options Injection]] | Thay đổi tùy chọn thực thi ứng dụng để chèn mã độc.                           |
| [[T1542 - Pre-OS Boot]]                            | Cài mã độc trước khi hệ điều hành khởi động để duy trì hiện diện.             |
| [[T1554 - Compromise Client Software Binary]]      | Thay thế các tệp thực thi hợp pháp của phần mềm để thực thi mã độc.           |
| [[../2. Techniques/T1574 - Hijack Execution Flow]]                  | Chiếm quyền điều khiển luồng thực thi để thực thi mã không mong muốn.         |
| [[T1209 - Time Providers]]                         | Lạm dụng dịch vụ đồng bộ thời gian để duy trì hiện diện hoặc thực thi mã độc. |

