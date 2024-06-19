# NT208.O21.ANTT-Group02-MidtermSeminar
Đề tài: tìm hiểu về framework NextJS (ReactJS / JavaScript)

Video trình bày: [NT208.O21.ANTT-Group02-MidtermSeminar](https://youtu.be/_sbfWFnXu84)

## Phần trả lời câu hỏi:

### 1. So sánh NextJS và Gatsby: Ưu điểm của NextJS và Khi nào nên dùng NextJS

**Ưu điểm của NextJS so với Gatsby:**

- **SSR (Server-Side Rendering) và SSG (Static Site Generation) Linh Hoạt:**
  - **NextJS:** Cung cấp cả SSR và SSG, cho phép render các trang trên server trước khi gửi đến client, cải thiện SEO và tốc độ tải trang. Nhà phát triển có thể chọn phương pháp render cho từng trang dựa trên nhu cầu cụ thể.
  - **Gatsby:** Chủ yếu là SSG, tất cả nội dung được render tĩnh trong quá trình build, phù hợp cho các trang web có nội dung ít thay đổi.
- **Routing Động:**
  - **NextJS:** Hỗ trợ routing động tự động dựa trên cấu trúc thư mục, giúp tạo các trang động dễ dàng mà không cần cấu hình phức tạp.
  - **Gatsby:** Cần cấu hình thủ công cho routing động, không thuận tiện bằng NextJS.
- **API Routes:**
  - **NextJS:** Cho phép tạo các API routes bên trong ứng dụng, giúp xây dựng các chức năng backend mà không cần một server riêng biệt.
  - **Gatsby:** Không hỗ trợ trực tiếp API routes, cần sử dụng các dịch vụ backend riêng.
- **Incremental Static Regeneration (ISR):**
  - **NextJS:** Hỗ trợ ISR, cho phép cập nhật nội dung tĩnh mà không cần build lại toàn bộ site, cải thiện hiệu suất và thời gian cập nhật nội dung.
  - **Gatsby:** Cần build lại toàn bộ site mỗi khi có thay đổi, tốn thời gian hơn.
- **Hỗ trợ CSS và Sass Tích Hợp:**
  - **NextJS:** Có hỗ trợ tích hợp cho CSS và Sass từ đầu, giúp dễ dàng quản lý styles trong dự án.
  - **Gatsby:** Cũng hỗ trợ nhưng cần cấu hình thêm, không thuận tiện bằng NextJS.

**Khi nào nên dùng NextJS:**

- **Ứng Dụng Phức Tạp:** Khi xây dựng các ứng dụng có nhiều chức năng phức tạp yêu cầu cả SSR và SSG.
- **Tối Ưu SEO:** Khi SEO là một yếu tố quan trọng, vì SSR giúp cải thiện SEO bằng cách cung cấp HTML hoàn chỉnh cho các công cụ tìm kiếm.
- **Nội Dung Động:** Cho các ứng dụng có nội dung thay đổi thường xuyên và yêu cầu cập nhật theo thời gian thực.
- **Tích Hợp APIs:** Khi dự án yêu cầu xây dựng và tích hợp các API backend trong cùng một mã nguồn.

### 2. Công cụ Testing và Debugging cho NextJS

**Công cụ Testing:**

- **Jest:**
  - Một framework testing JavaScript phổ biến, do Facebook duy trì, được sử dụng rộng rãi để kiểm tra đơn vị và tích hợp.
  - Hỗ trợ tính năng snapshot testing, giúp kiểm tra giao diện không thay đổi ngoài mong đợi.
- **React Testing Library:**
  - Tập trung vào việc kiểm tra các hành vi của người dùng hơn là chi tiết triển khai, giúp đảm bảo các thành phần hoạt động đúng theo mong đợi.
  - Dễ sử dụng và tích hợp tốt với Jest.
- **Cypress:**
  - Một công cụ kiểm tra end-to-end mạnh mẽ, cho phép kiểm tra toàn bộ ứng dụng từ góc nhìn của người dùng.
  - Hỗ trợ thời gian thực và tự động hoá các bài kiểm tra tương tác phức tạp.

**Công cụ Debugging:**

- **VSCode Debugger:**
  - Tích hợp trong Visual Studio Code, cho phép gỡ lỗi trực tiếp trong trình soạn thảo.
  - Hỗ trợ breakpoint, watch variables và call stack, giúp dễ dàng tìm ra lỗi.
- **Chrome DevTools:**
  - Công cụ phát triển tích hợp trong trình duyệt Chrome, hỗ trợ kiểm tra và gỡ lỗi ứng dụng web.
  - Bao gồm các tính năng như Elements, Console, Network và Performance.
- **React DevTools:**
  - Công cụ giúp kiểm tra và gỡ lỗi cấu trúc thành phần React trong trình duyệt Chrome và Firefox.
  - Cho phép xem và sửa đổi state và props của các thành phần React trực tiếp.
- **NextJS Debugging:**
  - Sử dụng lệnh `next dev` trong terminal để khởi động ứng dụng NextJS với chế độ gỡ lỗi, cung cấp thông tin chi tiết về lỗi và cảnh báo.

## 3. Ưu điểm của NextJS so với NodeJS

**Ưu điểm của NextJS:**

- **Khả năng Full-Stack:**
  - **NextJS:** Kết hợp cả phát triển frontend và backend trong cùng một framework, cho phép xây dựng các ứng dụng full-stack mà không cần phải tích hợp nhiều công cụ khác nhau.
  - **NodeJS:** Chủ yếu là runtime backend, cần tích hợp thêm các framework frontend như React hoặc Vue.js để xây dựng ứng dụng full-stack.
- **Dễ Sử Dụng:**
  - **NextJS:** Cung cấp cấu trúc và thiết lập sẵn cho việc xây dựng các ứng dụng web, giúp giảm bớt mã boilerplate và đơn giản hóa quy trình phát triển.
  - **NodeJS:** Đòi hỏi nhiều cấu hình và thiết lập ban đầu hơn, không có sẵn các tính năng như SSR và SSG.
- **Tính Năng Tích Hợp:**
  - **NextJS:** Bao gồm sẵn các tính năng như SSR, SSG, routing và API routes, giúp xây dựng ứng dụng nhanh chóng và hiệu quả.
  - **NodeJS:** Cần phải cài đặt và cấu hình các thư viện bổ sung để có các tính năng tương tự.
- **Tối Ưu Hiệu Suất:**
  - **NextJS:** Đi kèm với các tối ưu hóa hiệu suất như tự động tối ưu hóa tĩnh và ISR, giúp cải thiện hiệu suất ứng dụng ngay từ ban đầu.
  - **NodeJS:** Tối ưu hiệu suất phụ thuộc vào cách triển khai và cấu hình của nhà phát triển.

### 4. Kiến trúc Serverless

**Kiến trúc Serverless:**

**Định nghĩa:** Kiến trúc serverless là một mô hình thực thi điện toán đám mây, trong đó nhà cung cấp đám mây quản lý việc phân bổ và cung cấp tài nguyên máy chủ. Nhà phát triển chỉ cần viết mã và triển khai, không cần quan tâm đến việc quản lý máy chủ.

**Các thành phần chính:**

- **Function as a Service (FaaS):**
  - Cho phép triển khai các hàm riêng lẻ để thực thi theo sự kiện.
  - Ví dụ: AWS Lambda, Azure Functions và Google Cloud Functions.
  - Ưu điểm: Tự động mở rộng và tính phí dựa trên thời gian thực thi thực tế.
- **Backend as a Service (BaaS):**
  - Cung cấp các dịch vụ backend như cơ sở dữ liệu, xác thực, và lưu trữ mà nhà phát triển có thể sử dụng mà không cần quản lý máy chủ.
  - Ví dụ: Firebase và AWS Amplify.
  - Ưu điểm: Giảm bớt công việc quản lý cơ sở hạ tầng, tập trung vào phát triển ứng dụng.

**Lợi ích:**

- **Khả năng mở rộng:**
  - Tự động mở rộng theo tải công việc, đảm bảo hiệu suất tối ưu và chi phí hiệu quả.
  - Không cần cấu hình thủ công việc mở rộng.
- **Chi phí hiệu quả:**
  - Trả tiền cho thời gian thực thi thực tế, giúp tiết kiệm chi phí so với các mô hình truyền thống yêu cầu tài nguyên máy chủ luôn sẵn sàng.
  - Không tốn chi phí cho tài nguyên không sử dụng.
- **Tập trung vào mã nguồn:**
  - Nhà phát triển có thể tập trung vào việc viết mã và logic kinh doanh mà không cần lo lắng về quản lý máy chủ và cơ sở hạ tầng.
  - Tăng tốc độ phát triển và triển khai ứng dụng.

**Ứng dụng của kiến trúc serverless:**

- **Ứng dụng có tải công việc biến đổi:**
  - Phù hợp với các ứng dụng có tải công việc không đều hoặc biến đổi theo thời gian, như các dịch vụ web có lưu lượng truy cập biến đổi.
- **Hệ thống điều khiển sự kiện:**
  - Lý tưởng cho các hệ thống dựa trên sự kiện, như xử lý dữ liệu theo thời gian thực hoặc tự động hóa công việc.
- **Microservices:**
  - Giúp xây dựng các dịch vụ nhỏ, độc lập có thể triển khai và mở rộng riêng lẻ.
- **Chu kỳ phát triển nhanh:**
  - Thích hợp cho các dự án cần triển khai nhanh chóng và thay đổi linh hoạt theo yêu cầu kinh doanh.
