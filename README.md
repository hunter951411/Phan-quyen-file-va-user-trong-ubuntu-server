# Phan-quyen-file-va-user-trong-ubuntu-server
Phân quyền file và user trong ubuntu server

##1 Phân quyền kiểu CHMOD

- **Chmod**(change mode) là kiểu chỉ định quyền thực thi của file/ folder
- Gồm có 3 quyền chính:
<ul>
<li>Quyền đọc (r - 4)</li>
<li>Quyền ghi (w - 2)</li>
<li>Quyền xem/ truy cập (x - 1)</li>
</ul>

- Biểu diễn: [ user ] [ group] [ anybody]

- **chmod [tùy_chọn] [biểu_diễn_phân_quyền] [tên_file_hoặc_thư_mục]**

- Tùy chọn:
<ul>
<li>-v: hiển thị báo cáo sau khi chạy lệnh. Nếu bạn chmod nhiều file/folder cùng lúc thì cứ mỗi lần nó đổi quyền của 1 file/folder xong là sẽ hiện báo cáo.</li>
<li>-c: giống như trên, nhưng chỉ hiện khi nó đã làm xong tất cả.</li>
<li>-f: Hiểu ngắn gọn là kiểu “kệ mẹ nó”, nếu có lỗi xảy ra nó cũng không thông báo.</li>
<li>-R: nếu bạn CHMOD một folder thì kèm theo -R nghĩa là áp dụng luôn vào các file/folder nằm bên trong nó.</li>
<li>--help: hiển thị thông báo trợ giúp.</li>
</ul>

Ví dụ: rwxr--r-- (744)

Ở phần [biểu diễn phân quyền], ban có thể biểu diễn bằng 2 kiểu:
<ul>
<li>kiểu ký tự: giống như ở trên (rw-rw-x–).</li>
<li>kiểu số: cũng giống như ở trên (644).</li>
</ul>

##2 Phân quyền kiểu CHOWN

- **Chown**(change own) là kiểu chỉ định quyền user/ group sở hữu folder.
- Chỉ để định quyền sở hữu của một user hay nhóm user nào đó để sở hữu file/forlder.
- Mặc định user tạo file/folder sẽ sở hữu thư mục đó.
- Lệnh đổi:
**chown [ user ] : [ group ]   [ file/folder ]**


**Nguồn: Internet**
