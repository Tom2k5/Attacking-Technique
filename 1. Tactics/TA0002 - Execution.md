---
title: Execution
mitre_id: TA0002
tags:
  - mitre-attack
  - tactic
  - execution
---
---
# Execution
Giai đoạn Execution cho phép kẻ tấn công **thực thi mã tùy ý** trên hệ thống mục tiêu nhằm thực hiện các bước tiếp theo như thiết lập chỗ đứng (persistence), tải công cụ phụ, hoặc điều khiển hệ thống từ xa.

## Techniques

| Kỹ thuật                                       | Mô tả                                                                |
| ---------------------------------------------- | -------------------------------------------------------------------- |
| [[T1608 - Cloud Administration Command]]       | Sử dụng công cụ hoặc API quản trị cloud để chạy mã                   |
| [[T1059 - Command and Scripting Interpreter]]  | Sử dụng shell như PowerShell, CMD, Bash để thực thi mã               |
| [[T1609 - Container Administration Command]]   | Sử dụng lệnh quản lý container (Docker, Kubernetes...) để chạy mã    |
| [[T1610 - Deploy Container]]                   | Triển khai container chứa mã độc trong môi trường mục tiêu           |
| [[T1053 - Scheduled Task/Job]]                 | Tạo hoặc lợi dụng cronjob/tác vụ định kỳ để chạy mã                  |
| [[T1216 - System Services]]                    | Tạo/sửa đổi dịch vụ hệ thống để thực thi payload                     |
| [[T1129 - Shared Modules]]                     | Tải mô-đun chia sẻ (DLL...) để thực thi mã qua ứng dụng hợp pháp     |
| [[T1203 - Exploitation for Client Execution]]  | Khai thác lỗ hổng ứng dụng client để thực thi mã                     |
| [[T1106 - Native API]]                         | Gọi trực tiếp API hệ điều hành để thực thi mã                        |
| [[T1047 - Windows Management Instrumentation]] | Sử dụng WMI để thực thi mã – hỗ trợ từ xa                            |
| [[T1569.002 - Service Execution]]              | Tạo/khởi chạy dịch vụ để thực thi mã                                 |
| [[T1204 - User Execution]]                     | Dụ người dùng thực hiện hành vi như mở file hoặc chạy script         |
| [[T1647 - Input Injection]]                    | Tiêm đầu vào vào ứng dụng để điều khiển hành vi thực thi             |
| [[T1559 - Inter-Process Communication]]        | Truyền dữ liệu/mã giữa các tiến trình để kích hoạt thực thi          |
| [[T1072 - Software Deployment Tools]]          | Dùng công cụ triển khai phần mềm (SCCM, Group Policy...) để chạy mã  |
| [[T1055 - Process Injection]]                  | Tiêm mã vào tiến trình hợp pháp để thực thi mã và tránh bị phát hiện |

## Mitigations
- [[M1038]] Application Isolation and Sandboxing
- [[M1035]] Limit Access to OS Features (tắt macro, WMI nếu không dùng)
- [[M1042]] Disable or Remove Feature or Program (gỡ bỏ ngôn ngữ scripting không cần thiết)
- [[M1031]] Least Privilege (hạn chế quyền chạy dịch vụ/tạo tiến trình)
