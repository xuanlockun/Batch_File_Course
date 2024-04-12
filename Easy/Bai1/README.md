<h1> Bài 1: Xuất ra màn hình</h1>

Lệnh echo để in ra màn hình. <br>
Ví dụ:
```cmd
    echo Xin chào
```

Tuy nhiên khi chạy thì nó chỉ hiện lên 1 chút xíu rồi tắt, vì vậy chúng ta cần thêm lệnh dừng lại để xem lâu hơn.
Ví dụ
```cmd
    echo Xin chào
    pause
```
Chúng ta lại thấy nó hiện khá nhiều thứ nên chúng ta thêm lệnh @echo off để dễ nhìn hơn.

```cmd
    @echo off
    echo Xin chào
    pause
```

Chúng ta lại thấy chương trình bị lỗi tiếng việt, vì vậy thêm chcp 65001 ở sau dòng @echo off.

```cmd
    @echo off
    chcp 65001
    echo Xin chào
    pause
```

Nếu bạn thấy dòng "Active code page: 65001" thì thêm lệnh cls để xóa nó<br>
Lệnh cls để xóa những gì đã in trước đó <br>
Ví dụ về lệnh cls

```cmd
    @echo off
    echo abc
    echo xyz
    cls
    echo rawr
    pause
```
Lệnh cls sẽ xóa việc in ra abc xyz mà chỉ in ra rawr<br>
Tiếp tục bài chúng ta

```cmd
    @echo off
    chcp 65001
    cls
    echo Xin chào
    pause
```


## Kết luận<br>
Lệnh echo để in ra.<br>
Cấu trúc chuẩn file tiếng việt

```cmd
    @echo off
    chcp 65001
    cls
    -------------------------
    Nội dung code của bạn
    -------------------------
    pause
```
