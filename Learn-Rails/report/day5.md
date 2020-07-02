# Day5
### Mô hình MVC (Model-View-Controller) : phân bổ source thành 3 phần 
##### Model :  là nơi  tương tác với dữ liệu hoặc hệ quản trị cơ sở dữ liệu (mysql, mssql…)
##### View : là nới chứa những giao diện ( button, edit text, menu, ...)
##### controller: là nới tiếp nhận những yêu cầu xử lý được gửi từ người dùng
##### Ưu điểm : 
###### -Trình tự xử lý rất rõ ràng
##### -Quá trình phát triển – quản lý – vận hành – bảo trì web diễn ra thuận lợi hơn, tạo ra được các chức năng chuyên biệt hoá đồng thời kiểm soát được luồng xử lý
######  -Tạo mô hình chuẩn cho dự án, dễ tiếp cận
##### - đơn giản, dễ hiểu, xử lý những nghiệp vụ đơn giản,
#####  Sự tương tác giữa các thành phần
-   **Controller** tương tác với qua lại với **View**
-   **Controller** tương tác qua lại với **Model**
-   **Model** và **View** không có sự tương tác với nhau mà nó tương tác với nhau thông qua **Controller**



**Người dùng** -----(Request)----> **Brower** ---(Request)-----> **Router** -----(tìm đường dẫn)----> **Controller** (xử lý logic) -------> **Model** ( xử lí dữ liệu) ------(trả dữ liệu đã xử lí , data ...... ) -------->> **Controller**(cầm dữ liệu được lấy ra từ model)  ------(data)----------> **View** (nạp dữ liệu ) ----> controller ---(Reponse) ------ > View của **Người dùng**
