# Làm quen với ứng dụng web động đơn giản sử dụng Flutter và Dart

Trong bài lab này tôi sẽ hướng dẫn phát triển ứng dụng full-stack đơn giản với Dart và Flutter bao gồm backend và frontend.

Việc sử dụng các frameworl hiện đại trong phát triển và dễ dàng quản lý dự án. Flutter là một công cụ phát triển ứng dụng đa nền tảng, cho phép chúng ta tạo ra các công cụ cho web, di động (android, ios) và desktop (window, macOS và Linux) từ cùng một dự án mã nguồn (codebase). Điền này giúp chúng ta tiếp kiệm thời gian và công sức khi chúng ta chỉ cần viết mã một lần mà có thể biên dịch để chạy trên nhiều nền tảng khác nhau.

Quá trình biên dịch và phát hành ứng dụng web từ Dart và Framework sẽ tự động sinh ra mã cho backend và mã cho frontend (HTML, CSS và Javascrip) mà chúng ta không cần phải viết chúng trực tiếp. Điều này giúp chúng ta tập trung vào logic ứng dụng và giảm thiểu thời gian viết mã lặp lại. Tương tự, khi biên dịch ra các nền tảng di động hay desktop, chúng cũng sinh ra ứng dụng native trên cùng một codebase.

## Mục tiêu
- Hiểu và áp dụng được các khái niệm cơ bản về ứng dụng web động, ứng dụng đa nể tảng.
- Sử dụng Dart và thư viện shelf, shelf_router để tạo ra server đơn giản xử lý các yêu cầu HTTP theo chuẩn RESTful API.
 - Sử dụng Flutter framework để tạo giao diện đơn giản xử lý các yêu cầu HTTP theo chuẩn RESTful API.
 - Tích hợp giao diện với logic xử lý phản hồi từ server, thực hiện thao tác gửi dữ liệu từ client lên server thông qua HTTP POST.
 - Kiểm thử đơn giản với Postman để kiểm tra phản hồi từ server đối với các yêu cầu GET và POST, bao gồm cả trường hợp hợp lệ và không hợp lệ.

 ## Cấu trúc thư mục
 Để tiện cho việc quản lý và có thể đẩy lên GitHub, chúng ta sẽ cài đặt backend và frontend trong cùng một dự án.
 ```plaintext
 simple_flutter_project\
 |-- frontend/ # thư mục chứa mã nguồn Dart và Flutter cho frontend
 |-- backend/ # thư mục chứa mã nguồn Dart cho backend
 ```

 ## Các bước thực hiện
 ### Bước 1: khởi tạo dự án
 1. Tạo thư mục gốc chứa dự án `simple_flutter_project`
 2. Tạo thư mục `backend` và `frontend` trong thư mục `simple_flutter_project` như cấu trúc ở trên
 