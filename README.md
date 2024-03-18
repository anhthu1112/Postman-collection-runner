## 14/03 Postman collection runner

### 1. CI/CD là gì

CI là viết tắt của Continuous Integration (tích hợp liên tục), CD là viết tắt của Continuous Delivery (chuyển giao liên tục) hoặc Continuous Deployment (triển khai liên tục).

Khái niệm CI/CD thường đề cập đến việc tự động hóa trong quy trình phát triển phần mềm và chuyển giao sản phẩm, giúp cho việc tích hợp diễn ra nhanh hơn và sản phẩm hoàn thiện được chuyển đến người dùng trong thời gian ngắn nhất.

Phần mềm được tạo thành: Source code (Mã nguồn mà các developer phát triển) + Quá trình build code (Biến code từ ngôn ngữ lập trình thành ngôn ngữ mà máy có thể hiểu và chạy được - phần mềm)

#### CI : Continuous Integration: Tích hợp liên tục 

- Một dự án sẽ có 1 kho code chung và nhiều lập trình viên cùng nhau đóng góp code vào kho chung đó (VD : Github)
- Các dev sẽ liên tục đóng góp code vào repository
- CI khi code liên tục được tích hợp vào kho chung -> code sẽ tự động được built -> chạy unit test -> chạy integration test -> built docker image(Bản dựng phần mềm - có thể triển khai phần mềm từ cái này)
- CI : Built Softwware at Every Change 
- Lợi ích: Giảm thiểu rủi ro nhờ việc phát hiện lỗi và fix sớm, tăng chất lượng phần mềm nhờ việc tự động test và inspect. Giảm thiểu những quy trình thủ công lặp đi lặp lại. Sinh ra sản phẩm có thể deploy bất kỳ thời gian và địa ddirrm 

#### CD: Continuous Delivery 

- Khi quá trình CI hoàn thành, CD là việc liên tục triển khai các bản dựng thành phần mềm lên môi trường sit/uat/production
- CD: Phát hiện có bản dựng phần mềm mới -> Triển khai phần mềm lên môi trường sit/uat/production -> Chạy UI testing, load testing, integration testing, API testing 
- Lợi ích: Giảm thiểu những quy trình thủ công lặp đi lặp lại. Giảm thiểu rủi ro nhờ phát hiện lỗi và fix sớm, tăng chất lượng phần mềm nhờ việc tự động test và inspect 

