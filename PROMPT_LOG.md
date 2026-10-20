# NHẬT KÝ PROMPT ENGINEERING (VIBE CODING LOG)

- **Họ và tên:** Nguyễn Nhật Bảo Lâm
- **MSSV:** 125000777
- **Tên đề tài Website:** Liên Quân Mobile Showcase – Chiến Trường Huyền Thoại
- **Công cụ AI đã sử dụng:** ChatGPT, Google Gemini

## 1. Yêu cầu ban đầu (System/Initial Prompt)

**Prompt đã dùng với Google Gemini:**

> Tôi chọn chủ đề tạo website giới thiệu game Liên Quân Mobile có hợp lý không, dễ làm không. Lập kế hoạch và các bước thực hiện cho tôi. Chỉ dùng HTML và CSS, không được dính tới JavaScript.

**Mục tiêu:** Xác định tính phù hợp của đề tài, lập kế hoạch thực hiện và giới hạn công nghệ sử dụng cho website.

**Kết quả AI tạo ra:** Gemini đưa ra kế hoạch và các bước thực hiện website theo chủ đề Liên Quân Mobile.

**Quyết định của sinh viên:** Chọn chủ đề Liên Quân Mobile Showcase và triển khai giao diện bằng HTML5, CSS3. Các thư viện bên ngoài được sử dụng trong phạm vi giảng viên cho phép.

## 2. Quá trình tinh chỉnh & Giải quyết sự cố (Iteration Iterations)

### Lần 1: Dựng khung Semantic HTML & CSS Variables

**Prompt đã dùng với ChatGPT:**

> Hãy xây dựng mã HTML cho website giới thiệu game Liên Quân Mobile với bố cục rõ ràng, giao diện hiện đại. Website cần có Header, thanh điều hướng, Hero, danh sách tướng, phần giới thiệu tính năng, cộng đồng, khu vực tải game và Footer. Sử dụng HTML5 semantic, liên kết CSS bằng file External CSS và thiết kế theo chủ đề nền tối kết hợp màu vàng.

**Kết quả AI tạo ra:**

ChatGPT tạo khung HTML cho website gồm các phần Header, Hero, Champions, Features, Community, Download và Footer. Mã nguồn sử dụng các thẻ HTML5 như `header`, `nav`, `main`, `section`, `article` và `footer`.

**Nhận xét & Tinh chỉnh của SV:**

- Giữ các khu vực nội dung riêng biệt để dễ quản lý và chỉnh sửa.
- Sử dụng file `style.css` bên ngoài thay vì viết CSS trực tiếp trong HTML.
- Giữ các liên kết điều hướng đến từng phần của trang.
- Bổ sung hình ảnh thực tế để thay thế các phần minh họa ban đầu bằng CSS.

### Lần 2: Tích hợp thư viện Animate.css & AOS

**Prompt đã dùng với ChatGPT:**

> Hãy tích hợp Animate.css và AOS vào website Liên Quân Mobile Showcase. Sử dụng Animate.css cho hiệu ứng xuất hiện ban đầu và AOS cho hiệu ứng khi cuộn đến các phần nội dung. Giữ nguyên cấu trúc HTML, CSS External và không tự viết JavaScript cho các chức năng riêng của website.

**Kết quả AI tạo ra:**

ChatGPT bổ sung liên kết CDN của Animate.css và AOS, đồng thời thêm các lớp hiệu ứng như `animate__fadeInLeft`, `animate__fadeInRight`, `data-aos="fade-up"` và `data-aos="zoom-in"`.

AOS được khởi tạo bằng một đoạn JavaScript ngắn để hiệu ứng cuộn trang hoạt động.

**Thách thức gặp phải:**

AOS cần được khởi tạo thì các phần tử có thuộc tính `data-aos` mới được kích hoạt hiệu ứng khi cuộn trang.

**Cách sửa prompt (Debug prompt):**

> Hãy kiểm tra việc tích hợp AOS trong website. Đảm bảo đã liên kết thư viện AOS, các phần tử cần hiệu ứng có thuộc tính data-aos và thư viện được khởi tạo đúng cách. Chỉ sử dụng đoạn khởi tạo thư viện trong phạm vi giảng viên cho phép, không thêm JavaScript cho các chức năng riêng của website.

**Nhận xét & Tinh chỉnh của SV:**

- Kiểm tra việc tải thư viện từ CDN và kết nối Internet.
- Giữ các hiệu ứng ở mức vừa phải để giao diện không bị rối.
- Phân biệt JavaScript dùng để khởi tạo thư viện với JavaScript tự viết cho chức năng của website.

### Lần 3: Nhận xét cấu trúc và khả năng đáp ứng yêu cầu đề thi

**Prompt đã dùng với Google Gemini:**

> [Đính kèm mã nguồn do ChatGPT soạn]
>
> Thầy yêu cầu cấm JavaScript trong code, nhưng không cấm thư viện JavaScript. Bạn thấy cấu trúc trang web mà ChatGPT soạn đã đầy đủ, hợp lý chưa, có thể được điểm cao không?

**Kết quả AI tạo ra:**

Gemini nhận xét cấu trúc HTML do ChatGPT soạn là hoàn chỉnh, chuyên nghiệp và phù hợp với các tiêu chí của đề thi. Gemini đánh giá bộ khung có tiềm năng đạt điểm cao.

**Nhận xét & Tinh chỉnh của SV:**

Tôi sử dụng nhận xét của Gemini để tham khảo, nhưng vẫn cần tự kiểm tra mã nguồn, hiệu ứng, giao diện thực tế và các tiêu chí chấm điểm. Nhận xét của AI không thay thế kết quả chấm điểm của giảng viên.

### Lần 4: Tích hợp hình ảnh và sửa lỗi bố cục

**Prompt đã dùng với ChatGPT:**

> Tôi đã tải hình ảnh vào thư mục assets gồm banner.jpg, DauSi.jpg, PhapSu.jpg, SatThu.jpg, XaThu.jpg và logo.png. Hãy giúp tôi chỉnh sửa HTML để sử dụng các hình ảnh này thay thế phần minh họa CSS cũ.

Sau khi kiểm tra giao diện, tôi tiếp tục yêu cầu:

> Tốn quá nhiều thời gian, giúp tôi chỉnh luôn vào HTML và CSS, để tôi copy đưa thẳng vào file, giới hạn kích thước ảnh để không bị vỡ bố cục.

**Kết quả AI tạo ra:**

ChatGPT cung cấp lại hai file `index.html` và `style.css`, tích hợp logo, banner và bốn ảnh tướng. CSS sử dụng `max-width`, `width`, `height`, `object-fit`, Grid, Flexbox và Media Queries để kiểm soát kích thước ảnh và bố cục trên các kích thước màn hình.

**Thách thức gặp phải:**

Logo ban đầu hiển thị quá lớn, làm thanh điều hướng bị đẩy lệch. Các phần minh họa tướng vẫn sử dụng CSS cũ thay vì ảnh thật.

**Cách sửa prompt (Debug prompt):**

> Hãy chỉnh lại toàn bộ HTML và CSS để sử dụng đúng các ảnh trong thư mục assets. Giới hạn kích thước logo, banner và ảnh tướng; giữ bố cục cân đối, không để ảnh làm tràn khung hoặc phá vỡ giao diện trên màn hình nhỏ.

**Nhận xét & Tinh chỉnh của SV:**

- Kiểm tra tên tệp và đường dẫn ảnh trong HTML.
- Giới hạn kích thước logo và sử dụng `object-fit` cho ảnh.
- Kiểm tra giao diện trên trình duyệt sau khi thay đổi mã nguồn.
- Giữ CSS trong file `style.css` để dễ bảo trì.

### Lần 5: Kiểm tra thư mục hình ảnh

**Prompt đã dùng với Google Gemini:**

> [Đính kèm ảnh chụp thư mục assets]
>
> Tôi đã tải đủ file ảnh vào thư mục assets chưa?

**Kết quả AI tạo ra:**

Gemini xác nhận thư mục ảnh đã có các tệp cần thiết theo danh sách được cung cấp.

**Nhận xét & Tinh chỉnh của SV:**

Tôi kiểm tra lại các tệp `logo.png`, `banner.jpg`, `DauSi.jpg`, `PhapSu.jpg`, `SatThu.jpg` và `XaThu.jpg`, sau đó tích hợp chúng vào HTML.

## 3. Đánh giá cá nhân về quá trình Vibe Coding

### AI đã giúp bạn tiết kiệm thời gian ở phần nào nhất?

AI giúp tôi tiết kiệm thời gian nhiều nhất ở khâu tạo khung HTML, xây dựng CSS cho giao diện, thiết kế bố cục bằng Grid và Flexbox, tích hợp thư viện hiệu ứng và sửa đường dẫn hình ảnh. Thay vì phải tự viết toàn bộ mã từ đầu, tôi có thể cung cấp yêu cầu, nhận mã nguồn rồi kiểm tra và điều chỉnh theo giao diện mong muốn.

### Bài học rút ra khi đặt câu hỏi (Prompt) cho AI trong thiết kế web?

Tôi nhận thấy prompt càng cụ thể về cấu trúc HTML, cách nhúng CSS, giới hạn JavaScript, đường dẫn hình ảnh và kích thước giao diện thì kết quả AI tạo ra càng dễ sử dụng.

Ngoài ra, không nên chỉ dựa vào lời nhận xét của AI để kết luận website đã hoàn chỉnh hoặc chắc chắn đạt điểm cao. Cần chạy thử trên trình duyệt, kiểm tra các liên kết, hiệu ứng, hình ảnh và giao diện responsive.

Tôi cũng học được rằng khi phát hiện lỗi, nên mô tả rõ hiện tượng, nguyên nhân có thể xảy ra và kết quả mong muốn để AI tập trung sửa đúng vấn đề thay vì viết lại không cần thiết toàn bộ dự án.
