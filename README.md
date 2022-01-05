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

# For teacher

## Tạo thông báo trong phần announcement

### Step to go

At course: Click Announcements -> Add a new topic

### Basic

- Điền đủ 2 field Subject và Message -> ấn post to forum
- Trong Message, chèn thêm options đặc biệt: ví dụ icon
- Không điền mà submit: required yêu cầu điền đủ 2 trường bắt buộc trên

### Advanced

<!-- - Attachment: upload file from local -->

- Display period: enable display start hoặc display end để chọn
- Tags:

--- Tạo 1 tags mới: nhập và enter
--- Tạo multiple tags

## Thêm assignment cho course

### Step to go

At course: Turn Editing On -> Add an activity or resource -> Assignment

### Basic

- Điền Assignment name, các trường khác để default -> save and return to course
- Không điền Asignment name mà submit -> báo error trong field name: You must supply a value here.
- Trong description, chèn thêm options đặc biệt: ví dụ icon
<!-- - Additional files: upload file from local -->
- Availability: due date\*, ...
- Submission types: accepted file types\*, ...

### Extra

- Feedback types: comment inline\*, ...
- Grade: maximum grade\*, ...

## Thêm tài liệu (file) cho course

### Step to go

At course: Turn Editing On -> Add an activity or resource -> File

### Basic

- Điền Name và Select files -> Save and return to course
- Không điền mà submit -> required 2 trường Name và Select files

### Extra

<!-- - Tags: Enter tags... (1 or many) -->

## Thêm quiz cho course

### Step to go

At course: Turn Editing On -> Add an activity or resource -> Quiz

### Basic

- Điền Name, các trường khác để default -> save and display -> go to Step \*
- Không điền Name mà submit -> báo error trong field name: You must supply a value here.

<!-- - Timing: Enable các trường và điền thông tin tương ứng: Close the quiz, Time limit*, ...
- Grade: Grade to pass, Attempts allowed*: (1 or unlimited), ... -->

### Step \*

Khi tạo thành công (bước khởi đầu) sẽ dẫn đến giao diện display quiz -> Edit quiz -> Add -> a new question

- Test case chung của các option:

--- Nhập đủ các trường required: Question name, Question text, Default mark
--- Không nhập đủ các trường required-> báo error: You must supply a value here.

- Option Multiple Choice:
  Trong mục Answer:

--- Không 1 answer nào có Grade = 100% -> báo error: One of the choices should be 100%, so that it is possible to get a full grade for this question.
--- Nhập Grade nhưng k nhập tên Choice -> báo error: Grade set, but the Answer is blank

- Option True/False, Description, ...

## Xem điểm của sinh viên

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
- Xem thông báo bình thường

# Nhắn tin:

- Nhắn mess thường
- Nhắn lúc offline
- Nhắn có thêm icon
