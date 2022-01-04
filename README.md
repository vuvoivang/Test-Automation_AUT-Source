# Test-Automation_Source
URL AUT: http://localhost:8080/moodle

- Port Apache: 8080, 443
- Port MySQL: 3306
# Account Test
- Username: admin
- Password: PasswordTest123%
# Add 3 important folder
- moodle
- mysql
- htdocs/moodle
# Test Cases:

# For student
# Enroll:
- Enroll thành công (cho phép self-enr)
- Enroll thất bại (không cho phép)
- Enroll voi Key thanh cong
- Enroll voi Key that bai
# Nộp bài:
- Đúng hạn
- Trễ hạn (vẫn nộp dc)
- Trễ hạn (ko nộp được)
- Nộp bài quá 20MB
- Tích xác nhận
# Xem thông báo, event trên calendar:
- Click vào ngày rồi đi đến nộp bài
-  Xem thông báo bình thường
# Nhắn tin:
- Nhắn mess thường
- Nhắn lúc offline
- Nhắn có thêm icon
