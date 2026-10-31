# Hải Âu Ladder Lab

Trình mô phỏng PLC Ladder miễn phí chạy ngay trên trình duyệt, do **Hải Âu Automation** phát triển phục vụ học tập.

🔗 **Dùng thử:** https://lab.haiauautomation.com

## Tính năng
- Bài thực hành băng tải: START, STOP, E-STOP, RESET, cảm biến quang, bộ đếm hộp
- Lệnh: `XIC` `XIO` `OTE` `TON` `CTU` `RES` và nhánh song song
- Ladder hiển thị trực tiếp, Force tag, Run / Pause / Quét 1 lần
- Xuất / nhập chương trình dạng JSON, giao diện Việt / Anh

## Cú pháp
```
XIC(tag) XIO(tag) OTE(tag) TON(tên,ms) CTU(tên,số) RES(tên)
[ a , b ]      nhánh song song
// ghi chú
```
Ví dụ Start/Stop tự giữ:
```
[XIC(START_PB),XIC(MOTOR_RUN)] XIC(STOP_PB_NC) XIC(ESTOP_OK) OTE(MOTOR_RUN)
```

## Lưu ý
Đây là công cụ mô phỏng học tập, **không thay thế** phần mềm hoặc PLC thật và không liên kết với Rockwell Automation.

## Học tiếp
Khóa học PLC Rockwell bài bản: https://haiauautomation.com

## Giấy phép
Bảo lưu mọi quyền, xem file LICENSE.
