# 1. Switch
- lưu lại bản ghi nhớ địa chỉ MAC của tất cả các thiết bị mà nó kết nối tới ( xác định được cổng hệ thống)- tăngtô
- tăng tối da thời gian phản ứng mạng,có khả năng lọc frame
- khi gặp frame broadcast thì switch sẽ đẩy frame tự sao chép và frame này ra tất cả các cổng trừ cổngnhậpvào
- switch không quan tâm số lượng PC phát dữ liệu, người dùng  luôn luôn sử được băng thông tối đa
- có thể đấu nối swicth theo kiểu chuyển mạch đối xứng, bất đối xứng (trộn lẫn nhiều loại băng thông)
- trong mạng doanh nghiệp người ta thường tổ chức hệ thống switch thành 3 tầng
  - access layer : cung cấp các nhóm truy nhập đến các end user
  - distribution layer : cung cấp sự tập trung các kết nối lên tầng distribution , thực hiện chính sách định tuyến , chính sách chuyển mạch ...
  - core layer : vận chuyển dữ liệu qa lại  khôngvận dụng chính sách nào,tốc độ chuyển mạch nhanh
- nếu đấu nối switch lặp vật lý sẽ tạo nên hiện tượng flood, hệ thống bị treo. dự vào giao thucứ spanning tree protocol để tránh hiện tượng này

# 2. Cấu hình cơ bản trên switch
- đặt địa chỉ ip quản lí trên sw : 

``````
sw(config)#interface vlan 1 
sw(config-if)#no shutdown
sw(config-if)# ip address [ip] []
``````````````````
 - kiểm tra bảng địa chỉ mac : SW#show mac-address-table
- 

