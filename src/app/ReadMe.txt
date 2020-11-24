Tạo project:
ng new TenProject

Từ phiên bản angular 9 trở lên cài thêm localize bằng lệnh sau:
ng add @angular/localize

Cài đặt file json


Thêm file ngôn ngữ bằng lệnh sau: 
ng xi18n --output-path src/i18n
nó sẽ tạo ra thư mục i18n và file messages.xlf ở bên trong


Giờ để tạo một bản ngôn ngữ cho tiếng việt
Ta copy file messages.xlf rồi đặt thêm tên local của ngôn ngữ
messages.vi.xlf
Với những ngôn ngữ khác ta cũng tạo ra file tương tự như trên



Ở local để chạy xem kết quả với ngôn ngữ nào ta chạy như sau:
ng serve --configuration=vi --open
Trong đó vi là tên của ngôn ngữ mà ta đã đặt ở bước trước



Note: 
Khi ta thêm i18n vào một thẻ, Thì khi chạy lệnh 
ng xi18n --output-path src/i18n

Thì nó sẽ tự tạo ra các target với id tự động cho chúng ta

Nếu như bạn buốn tạo ra các id như ta tự đặt thì trên thẻ ta thêm id với @@ ở đằng trước vào
Thì trong file xlf sẽ sinh ra id như tên ta đặt
