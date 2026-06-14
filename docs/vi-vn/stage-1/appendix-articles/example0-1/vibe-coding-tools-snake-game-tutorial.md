# So sánh 7 công cụ lập trình AI

## Hướng dẫn chương này

Đối mặt với vô số công cụ lập trình AI, công cụ nào mới phù hợp với bạn nhất? Chương này thông qua một nhiệm vụ thực chiến thống nhất -- phát triển trò chơi "Rắn ăn mồi + AI làm thơ", đánh giá chéo 7 nền tảng Web Vibe Coding phổ biến như Lovable, Replit, Z.ai. Chúng ta sẽ so sánh đa chiều từ mức độ thân thiện với người mới, khả năng kiểm soát code, tính tiện lợi triển khai, giúp bạn nhanh chóng chọn ra công cụ hỗ trợ phát triển mạnh nhất.

---

# 1. Dùng Vibe Coding xây trò Snake: Hướng dẫn thực chiến hoàn chỉnh

Bài viết giới thiệu một phương pháp phát triển phần mềm mới nổi -- "Vibe Coding", sử dụng trí tuệ nhân tạo để tăng tốc quá trình xây dựng ứng dụng.

Tiếp theo chúng ta sẽ lần lượt giới thiệu khái niệm cốt lõi của Vibe Coding, giải thích AI Agent là gì, và cung cấp phương pháp viết prompt thực dụng. Cuối cùng, thông qua thực chiến hoàn chỉnh xây dựng trò "Snake (Rắn săn mồi)" từ đầu, và đánh giá so sánh chi tiết nhiều nền tảng Vibe Coding phổ biến, giúp bạn chọn bộ công cụ phù hợp nhất với mình.

## Bạn sẽ học được:

- **Vibe Coding là gì:** Hiểu định nghĩa, workflow và lợi thế chính của nó.
- **Vai trò của AI Agent:** Hiểu cách làm việc của AI Agent, và sự khác biệt với chương trình truyền thống.
- **Cách viết prompt tốt:** Nắm vững cách viết prompt rõ ràng, cụ thể, để nhận kết quả tốt hơn.
- **Công cụ Vibe Coding:** Làm quen với một loạt nền tảng lập trình và thiết kế AI phổ biến.
- **So sánh nền tảng:** Đánh giá và so sánh ưu nhược điểm của 7 nền tảng AI Agent khác nhau từ góc nhìn người mới bắt đầu.
- **Công cụ UI / UX:** Học cách tích hợp các công cụ UI/UX như Figma, Mastergo vào workflow tổng thể.

## 1. Giới thiệu

Trong các bài học trước, chúng ta luôn sử dụng mô hình phát triển fullstack của z.ai để hoàn thành nhiệm vụ lập trình.

Tuy nhiên, chúng ta có bao giờ nghĩ: cốt lõi của nó thực ra là "AI Agent" (khác với AI chat thông thường, và thông minh hơn nhiều)? Vì nó không chỉ trò chuyện với bạn, mà còn có thể suy nghĩ (khi bạn giao nhiệm vụ, nó sẽ trước lập kế hoạch), còn có thể chủ động hành động (ví dụ gọi tìm kiếm web, thực thi lệnh máy tính, mở trang web, v.v.). Chúng ta sẽ giới thiệu chi tiết hơn ở phần sau.

## 1. Vibe Coding là gì?

Vibe Coding là một phương pháp phát triển phần mềm kiểu mới sử dụng AI để tăng tốc quá trình phát triển ứng dụng. Nó không phải sản phẩm thay thế lập trình truyền thống, mà là một chế độ lập trình "hội thoại" hơn. Khái niệm này được nhà nghiên cứu AI Andrej Karpathy đề xuất: trong workflow này, nhà phát triển không còn tự viết code từng dòng, mà chủ yếu thông qua hướng dẫn AI Agent để tạo, tối ưu và debug ứng dụng.

Tư tưởng cốt lõi của Vibe Coding, là chuyển từ **"lấy code làm trung tâm (code-first)"** sang **"lấy ý định làm trung tâm (intent-first)"**. Bạn không cần suy nghĩ từ dòng code đầu tiên, mà dùng ngôn ngữ tự nhiên mô tả kết quả bạn muốn.

Workflow điển hình của Vibe Coding là một vòng lặp liên tục:

- **Mô tả mục tiêu:** Trước dùng một câu hoặc một đoạn mô tả chức năng bạn muốn triển khai, ví dụ: "Làm một trò Snake đơn giản có backend Python, có thể sinh thơ."
- **AI tạo code:** AI Agent phân tích nhu cầu của bạn, tạo code phiên bản đầu, bao gồm cấu trúc cơ bản, trang frontend và logic backend.
- **Chạy và quan sát:** Chạy code đã tạo, kiểm tra có hoạt động đúng như mong đợi không, đồng thời phát hiện bug hoặc điểm chưa tốt.
- **Phản hồi và lặp lại:** Nếu có lỗi hoặc hiệu quả không lý tưởng, tiếp tục ra lệnh trong hội thoại, ví dụ: "Rắn di chuyển quá chậm, tăng tốc độ lên", hoặc "Hiện file `.env` không đọc đúng API Key, xin sửa code backend."
- **Lặp lại các bước trên:** Liên tục lặp trong vòng "mô tả → tạo → chạy → phản hồi" cho đến khi ứng dụng đạt trạng thái hài lòng.

### Lợi thế chính của Vibe Coding:

- **Giảm rào cản:** Để nhà thiết kế, doanh nhân, sinh viên thiếu kinh nghiệm lập trình cũng có thể tham gia phát triển ứng dụng thông qua ngôn ngữ tự nhiên.
- **Prototype nhanh chóng:** Thời gian từ ý tưởng đến sản phẩm khả thi tối thiểu (MVP) giảm đáng kể.
- **Nâng cao hiệu quả:** Tự động xử lý lượng lớn công việc lập trình lặp đi lặp lại, cơ học (như code template), để nhà phát triển tập trung sức vào thiết kế kiến trúc và trừu tượng hóa vấn đề.
- **Thuận lợi thử nghiệm:** Khuyến khích cách sản xuất nhanh rồi hoàn thiện dần, tiện thử ý tưởng và chức năng mới hơn.

## 2. Nền tảng Vibe Coding trực tuyến (Web-based) là gì?

Trong lần thử nghiệm thực tế này, bạn sẽ phát hiện công cụ chúng ta đánh giá được chia thành hai loại: **Web-based (nền tảng trực tuyến)** và **IDE (môi trường phát triển cục bộ)**.

Dù cốt lõi đều là dùng AI giúp bạn viết code, nhưng trải nghiệm sử dụng và kịch bản áp dụng có sự khác biệt rất lớn:

### Nền tảng Vibe Coding trực tuyến (Web-based)

**Công cụ đại diện:** Lovable, Replit, Z.ai, v0

Giống như căn hộ dịch vụ "xách vali vào ở".

- **Không cần cấu hình môi trường:** Bạn không cần quan tâm Python là gì, phiên bản Node.js ra sao, cũng không cần lo cài đặt dependency. Mở trình duyệt, nhập URL, có thể bắt đầu viết code ngay.
- **Xem trước và triển khai một lần:** Sau khi code được tạo, nền tảng thường tự động hiển thị kết quả chạy ở cửa sổ bên phải. Làm xong, click một nút đã có thể tạo link chia sẻ cho bạn bè.
- **Kịch bản phù hợp:**
  - **Xác minh ý tưởng nhanh chóng (MVP):** Trong đầu có ý tưởng, muốn mất nửa tiếng xem có thể làm ra hay không.
  - **Người mới bắt đầu:** Hoàn toàn không muốn bị lỗi môi trường phức tạp làm nản, chỉ muốn trải nghiệm niềm vui lập trình AI.
  - **Ứng dụng nhẹ:** Làm một trang công cụ đơn giản, game nhỏ hoặc trang cá nhân.

### AI IDE (Môi trường phát triển cục bộ)

**Công cụ đại diện:** Cursor, Trae, VS Code + AI plugin

Giống như nhà ở "trang trí đầy đủ" tự sở hữu.

- **Khả năng cục bộ mạnh mẽ:** Nó chạy trên máy của bạn, có thể trực tiếp truy cập tất cả file cục bộ, tận dụng sức mạnh tính toán máy của bạn.
- **Kết nối liền mạch workflow chuyên nghiệp:** Phù hợp dự án lớn, có thể tự do cài đặt plugin, kết nối database cục bộ, debug phức tạp.
- **Kịch bản phù hợp:**
  - **Phát triển dự án chuyên nghiệp:** Cần bảo trì dài hạn, dự án thương mại có cấu trúc phức tạp.
  - **Tùy chỉnh sâu:** Cần kiểm soát chi tiết code đến mức cực đoan, hoặc cần kết hợp sâu với workflow cục bộ hiện có (như Git, Docker).
  - **Quyền riêng tư dữ liệu:** Code hoàn toàn ở cục bộ, phù hợp hơn với quy định an toàn của một số doanh nghiệp.

**Tóm lại:** Nếu bạn mới tiếp xúc lập trình AI, hoặc chỉ muốn nhanh làm một thứ nhỏ để vui, **nền tảng trực tuyến** là điểm khởi đầu tuyệt vời. Nếu bạn là nhà phát triển chuyên nghiệp, hoặc dự án ngày càng phức tạp, **IDE cục bộ** sẽ cung cấp giới hạn trên cao hơn.

---

## 3. AI Agent là gì?

### AI Agent là gì?

AI Agent là một hệ thống phần mềm, có khả năng nhận thức môi trường, ra quyết định, và tự chủ hành động để đạt mục tiêu cụ thể. So với phần mềm truyền thống tuân theo chỉ thị cố định, quy trình đơn lẻ, AI Agent linh hoạt và tự thích nghi hơn.

Dưới đây là một số đặc điểm chính phân biệt AI Agent với chương trình truyền thống:

- **Tự chủ (Autonomy):** AI Agent có tính độc lập cao. Chương trình truyền thống thường cần người kích hoạt từng bước, còn Agent có thể tự quyết định bước tiếp theo làm gì dựa trên mục tiêu.
- **Nhận thức và trí nhớ (Perception & Memory):** Agent thu thập dữ liệu từ môi trường (ví dụ phản hồi API, dữ liệu cảm biến, đầu vào người dùng, v.v.), và giữ lại ngữ cảnh thông qua "trí nhớ", từ đó tái sử dụng kinh nghiệm và cải thiện hiệu quả liên tục trong hành động sau.
- **Lý tính và hướng mục tiêu (Rationality & Goal-Orientation):** Agent sẽ phân tích và lập kế hoạch xoay quanh mục tiêu đã cho, chọn chuỗi hành động phù hợp nhất để theo đuổi "chỉ số hiệu suất" cao hơn.
- **Sử dụng công cụ (Tool Use):** Đặc điểm lớn của AI Agent hiện đại là có thể gọi công cụ bên ngoài, không còn giới hạn ở "tạo văn bản". Ví dụ, nó có thể duyệt web, chạy code, truy vấn database, gửi email, là một bộ não "điều độ công cụ".

Có thể hiểu theo phép loại suy:

- Một **chương trình truyền thống** giống như máy tính. Bạn cho nó nhập số và toán tử, nó chỉ thực hiện tính toán khi bạn bấm nút.
- Một **trợ lý AI** giống như trợ lý con người. Bạn bảo "giúp tôi tìm nhà hàng gần đây", nó sẽ cho bạn kết quả tìm kiếm và liệt kê lựa chọn, nhưng cuối cùng vẫn là bạn ra quyết định.
- Một **AI Agent** giống hơn như một đội nghiên cứu tự động. Bạn chỉ cần đưa ra mục tiêu cấp cao (ví dụ "giúp tôi lên kế hoạch một chuyến đi Nhật"), nó sẽ phân tách nhiệm vụ, tra cứu mạng, đặt vé máy bay khách sạn (qua API), sắp xếp lịch trình, cuối cùng giao kết quả cho bạn, gần như không cần bạn can thiệp chi tiết.

---

# 2. Về viết prompt

## 1. Prompt viết xong ngay tốt, hay chia thành nhiều bước tốt hơn?

Rất nhiều người sẽ không nhịn được muốn trực tiếp trong một prompt, nói rõ "làm một ứng dụng fullstack hoàn chỉnh" cùng lúc. Thực tế, công cụ hiện tại đã đủ mạnh, xác thực có cơ hội cho kết quả trông khá ổn ngay lần đầu. Nhưng xét về trải nghiệm tổng thể và tỷ lệ thành công, chia công việc thành các bước nhỏ, lặp theo giai đoạn, kết quả thường tốt hơn, cũng ít dễ rơi vào ngõ cụt "sửa không được" hơn.

> **Mẹo nhỏ:** Thay vì kỳ vọng "làm đúng ngay một lần", tốt hơn chia mục tiêu lớn thành các todo nhỏ có thể thực hiện.  
> Ví dụ, đừng trực tiếp nói "build me a Snake game", mà chia thành:  
> "1. Trước làm frontend của trò Snake",  
> "2. Rồi triển khai một backend ghi điểm",  
> "3. Cuối cùng nối frontend và backend lại".  
> Như vậy có thể khiến AI hiểu chính xác nhu cầu của bạn hơn và cho output đáng tin cậy hơn.

## 2. Càng rõ ràng, càng tốt

- Trong Vibe Coding, prompt bạn viết quan trọng không kém code bạn viết. Prompt càng rõ ràng, càng cụ thể, kết quả càng gần với ý bạn nghĩ.
- Nói rõ mục tiêu và ràng buộc ngay từ đầu, có thể giảm số lần sửa đổi sau, không chỉ tiết kiệm thời gian, cũng tiết kiệm quota sử dụng và chi phí.

---

# 3. Tổng quan công cụ (Vibe Coding / UIUX)

## 1. Nền tảng AI Agent

| **Name**                                   | **Platform** |
| ------------------------------------------ | ------------ |
| **[Lovable](https://lovable.dev/)**        | Web-based    |
| **[Cursor](https://cursor.com/cn/agents)** | PC           |
| **[Z.ai](https://chat.z.ai/)**             | Web-based    |
| **[Replit](https://replit.com/~)**         | Web-based    |
| **[Minimax](https://agent.minimaxi.com/)** | Web-based    |
| **[Trae](https://www.trae.ai/)**           | PC           |
| **[V0](https://v0.app/)**                  | Web-based    |

## 2. Nền tảng AI UIUX

| **Name**                              | **Platform**         |
| ------------------------------------- | -------------------- |
| **[Mastergo](https://mastergo.com/)** | Web-based            |
| **[FIgma](https://www.figma.com/)**   | Web-based, PC Plugin |

---

# 4. Hướng dẫn thực chiến (Vibe Coding + UI kết hợp)

1. Trong cửa sổ chat của nền tảng Vibe Coding bạn chuẩn bị sử dụng, nhập mô tả chương trình bạn muốn.
   Ví dụ:

   > Xin xây dựng một ứng dụng web Snake đơn giản với frontend và backend.
   >
   > 1. Frontend
   >
   > - Trang 1: Trang game
   >   - Dùng phím điều khiển di chuyển của rắn.
   >   - Rắn ăn không phải thức ăn, mà là từ tiếng Anh.
   >   - Thanh bên trang hiển thị từ đã thu thập và số lượng.
   >   - Sau khi game over, từ đã thu thập vẫn được giữ lại, tiếp tục trong ván mới.
   > - Trang 2: Trang làm thơ (Make Poem)
   >   - Hiển thị cùng danh sách từ như trang game (dữ liệu đồng nhất).
   >   - Cung cấp nút, gửi từ hiện thu thập cho backend để tạo một bài thơ.
   >   - Sau khi sinh thơ, từ đã sử dụng bị xóa khỏi danh sách hoặc giảm số đếm.
   >
   > * Thêm điều hướng đơn giản, chuyển đổi giữa hai trang Game và Make Poem.
   > * Đảm bảo từ thu thập được nhìn thấy ở cả hai trang.
   >
   > 2. Backend
   >
   > - Cung cấp một API backend, nhận từ đã thu thập và trả về một bài thơ.
   > - Dùng DeepSeek API để tạo thơ.
   > - Lưu API Key trong file `.env`, và ignore file này trong `.gitignore`.

2. Nhập DeepSeek API Key của bạn. (Có thể lấy tại [https://platform.deepseek.com/](https://platform.deepseek.com/))
   1. API Key của LLM dùng để gọi mô hình lớn trong dự án của bạn. Vì đây là thông tin nhạy cảm, không thể công khai, nên cần viết riêng trong file cấu hình.
      **Tại sao phải dùng file `.env`, và không upload nó lên GitHub?**
   - File `.env` chuyên dùng để lưu **khóa hoặc mật khẩu** (ví dụ DeepSeek API Key).
   - Nếu file này bị upload lên GitHub, tất cả mọi người trên thế giới đều thấy được khóa của bạn và sử dụng trái phép.
   - Vì lý do an toàn, chúng ta cần khai báo ignore `.env` trong file `.gitignore`, để Git không theo dõi nó.
   - Như vậy, dự án của bạn vẫn có thể sử dụng các khóa này bình thường trên máy cục bộ, mà sẽ không bị rò rỉ trong repository.

3. Sau khi xem kết quả tạo, nếu phát hiện lỗi hoặc cần sửa, có thể trực tiếp nhập yêu cầu sửa trong cửa sổ chat.
4. Nếu bạn không hài lòng với thiết kế trang, cũng có thể chọn thiết kế lại giao diện trong Figma hoặc Mastergo, rồi phản hồi ý thiết kế cho Agent.

- **Ví dụ**

> Xin thiết kế một **ứng dụng web hai trang** tên _Word-Snake_.
>
> - **Trang Game:**
> - Rắn điều khiển di chuyển bằng phím.
> - Rắn ăn là từ tiếng Anh, không phải thức ăn thông thường.
> - Panel bên phải hiển thị từ đã thu thập và số lượng.
> - Sau khi game over, kho từ không bị xóa, tiếp tục sử dụng ở ván mới.
> - **Trang Make Poem:**
> - Hiển thị cùng kho từ chia sẻ.
> - Người dùng chọn một phần từ và click nút **Generate Poem**.
> - Gửi các từ này cho backend, dùng DeepSeek API tạo thơ.
> - Sau khi sinh thơ, xóa hoặc giảm số lượng từ đã sử dụng trong kho.
> - **Điều hướng:** Chuyển đổi giữa hai trang qua Tab đơn giản hoặc menu trên cùng.
> - **Trạng thái chia sẻ:** Đảm bảo từ thu thập luôn đồng bộ và hiển thị ở cả hai trang.

- **Ví dụ kết quả**

![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image1.png)![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image2.png)

---

# 5. So sánh nền tảng AI Agent (Cách chọn tổ hợp tốt nhất cho dự án đơn giản)

Các nền tảng Vibe Coding khác nhau có đặc điểm và workflow khác nhau. Chúng ta sử dụng cùng một bộ yêu cầu "trò Snake với DeepSeek API" để thử nghiệm thực tế trên nhiều nền tảng, đánh giá ưu nhược điểm từ góc nhìn người mới bắt đầu. Dưới đây là tóm tắt.

## 1. Tiêu chuẩn so sánh

1. **Mục tiêu (Goal)**
   Xây dựng một ứng dụng web Snake kết nối DeepSeek API.
2. **Chi tiết game (Game Details)**
   1. Game tạo thơ thông qua DeepSeek LLM API.
   2. Rắn ăn từ tiếng Anh, từ thu thập được giữ lại sau game over, tiếp tục sử dụng ở ván mới. Cùng một từ có thể thu thập nhiều lần, tính riêng.
   3. Khi tạo một bài thơ, từ đã sử dụng bị xóa khỏi kho.

3. **Chức năng bắt buộc (Must-Haves)**
   1. Một trang frontend có thể chạy, bao gồm trò Snake (điều khiển phím, render Canvas).
   2. Cơ chế thu thập từ (từ xuất hiện trên bàn cờ, rắn ăn từ, danh sách sidebar cập nhật).
   3. Lưu trữ kho từ liên tục giữa nhiều ván game.
   4. Backend sử dụng DeepSeek API (nếu không có API Key, có thể trước trả về thơ mô phỏng).
   5. Nút "sinh thơ": Sau khi click gọi backend, hiển thị thơ, và cập nhật kho từ theo sử dụng.
   6. Hỗ trợ API Key qua `.env`, và tránh rò rỉ khóa thông qua `.gitignore`.

4. **Điểm cộng (Nice-to-Haves)**
   1. Người dùng có thể chọn từ nào để sinh thơ.
   2. Trải nghiệm người dùng thân thiện (ví dụ sidebar hiển thị rõ ràng danh sách từ, layout khu vực hiển thị thơ hợp lý).
   3. Thêm comment trong code cho người mới bắt đầu, giải thích logic chính.

## 2. So sánh output code

### 1. Lovable (Web-based)

- **Loại nền tảng:** Web
- **Đặc điểm chính và workflow:** Lovable làm tốt trong tích hợp và phối hợp, nó tự động hoàn thành các khởi tạo như kết nối database Supabase, khiến quá trình xây dựng dự án rất thuận lợi. Bạn chỉ cần mô tả nhu cầu dự án, Agent sẽ giúp bạn kết nối các loại dịch vụ, xây dựng cấu trúc cơ bản.
- **Người dùng phù hợp:** Đối với người mới lần đầu thử Vibe Coding, Lovable là lựa chọn rất thân thiện. Nó đơn giản hóa độ phức tạp của liên kết đa dịch vụ, để bạn tập trung sự chú ý vào prompt và lặp lại, thay vì cấu hình môi trường. Nhờ tự động hóa cao, bạn có thể nhanh chóng nhận được prototype chạy được.
- **Quá trình prompt:**
  ![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image3.png)
- **Hiệu quả trò Snake:**

![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image4.png)![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image5.png)

- **Giá:** Tương đối cao, nhưng nếu bạn có email trường, có thể xác minh sinh viên để dùng với giá nửa.
  ![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image6.png)

### 2. Cursor (IDE)

- **Loại nền tảng:** Ứng dụng desktop (PC)
- **Đặc điểm chính và workflow:** Cursor là một IDE chuyên biệt tích hợp khả năng AI, hỗ trợ Windows, macOS và Linux. Nó nhúng trực tiếp tạo code, viết lại thông minh, truy vấn codebase vào môi trường phát triển. So với công cụ Web, nó gần với trải nghiệm phát triển cục bộ truyền thống hơn. Vì là môi trường cục bộ, cấu hình máy khác nhau sẽ thỉnh thoảng gặp vấn đề liên quan đến môi trường. Điểm tốt là dự án nằm ngay trên máy, không cần tải thêm hay cấu hình môi trường chạy, Cursor sẽ giúp bạn xử lý nhiều bước phức tạp.
- **Người dùng phù hợp:** Đối với người dùng đã có nền tảng lập trình nhất định, Cursor là một môi trường rất mạnh mẽ và quen thuộc. Nhưng đối với người mới hoàn toàn không có nền tảng, cần tự hiểu cấu trúc dự án, quản lý dependency và tổ chức file, đường cong học sẽ dốc hơn. Phù hợp hơn cho nhà phát triển muốn thêm trợ lý AI vào quy trình lập trình truyền thống.
- **Quá trình prompt:**
  ![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image7.png)
- **Hiệu quả trò Snake:**

![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image8.png)![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image9.png)

- **Giá:**
  ![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image10.png)

### 3. Z.ai (Web-based)

- **Loại nền tảng:** Web
- **Đặc điểm chính và workflow:** Cách sử dụng Z.ai khá trực tiếp, nhưng một thách thức rõ ràng là: bạn cần **thủ công copy paste code đã tạo**. Bản thân nền tảng thiếu cửa sổ xem trước thời gian thực, nên rất khó thấy ngay hiệu quả chạy code.
- **Người dùng phù hợp:** Nền tảng này yêu cầu cách sử dụng "động tay" hơn. Thiếu tự động hóa nghĩa là bạn phải trực tiếp đối mặt với code, điều này đối với người muốn hiểu sâu nội dung AI output lại là một dạng rèn luyện. Nhưng copy paste thường xuyên sẽ mang lại vấn đề hiệu quả và nguy cơ sai sót. Phù hợp hơn cho người muốn xem "raw AI output code", chứ không phải người theo đuổi trải nghiệm một lần click.
- **Quá trình prompt:**
  ![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image11.png)
- **Hiệu quả trò Snake:**

![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image12.png)![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image13.png)

- **Giá:**
  ![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image14.png)

### 4. Replit (Web-based)

- **Loại nền tảng:** Web
- **Đặc điểm chính và workflow:** Replit là môi trường phát triển và triển khai trực tuyến tất cả trong một, trong trình duyệt đã có thể viết code, chạy chương trình, tạo địa chỉ truy cập online. Trước khi bắt đầu code, nó sẽ đưa ra kế hoạch hành động rõ ràng; đồng thời cung cấp editor trực quan, bạn có thể sửa UI trực tiếp trong cửa sổ xem trước, source code tự động đồng bộ cập nhật. Như vậy có thể bạn luôn xác nhận output của AI có đúng kỳ vọng không, giảm đáng kể số lần sửa đổi qua lại.

  ![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image15.png)

- **Người dùng phù hợp:** Replit rất thân thiện với người mới. Nó đơn giản hóa vòng khép kín hoàn chỉnh từ code đến triển khai, không cần tự cấu hình server hay hosting thêm. Chức năng phối hợp cũng rất mạnh, phù hợp bạn học cùng làm dự án hoặc nhờ người khác hỗ trợ xem code từ xa.
- **Quá trình prompt:** Trong quá trình xây dựng, AI không phải ngay từ đầu đã hiểu hoàn toàn nhu cầu, trải qua khoảng 3 vòng lặp, output cuối cùng mới đạt hiệu quả lý tưởng.
  ![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image16.png)
- **Hiệu quả trò Snake:**

![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image17.png)![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image18.png)

- **Giá:**
  ![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image19.png)

### 5. Minimax (Web-based)

- **Loại nền tảng:** Web
- **Đặc điểm chính và workflow:** Minimax thường mất nhiều thời gian hơn khi thực thi nhiệm vụ. Quy trình thường bao gồm: AI tự động phát hiện và sửa lỗi, vì vậy toàn bộ quá trình có thể chậm hơn, thậm chí hơi rắc rối. Lấy dự án này làm ví dụ, Agent thường trước tạo một kế hoạch chi tiết, rồi từng bước xây dựng backend, database và logic frontend.
- **Người dùng phù hợp:** Vì nó sẽ tự động chạy test và sửa lỗi, thời gian và tiêu thụ Token đều khá lớn, nhưng bạn có thể rõ ràng thấy AI định vị và giải quyết vấn đề thế nào, từ góc độ học tập rất có giá trị.
- **Quá trình prompt:**

![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image20.png)![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image21.png)![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image22.png)![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image23.png)

- **Hiệu quả trò Snake:**

![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image24.png)![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image25.png)

- **Giá:** Phiên bản miễn phí trong dự án phức tạp rất có thể không chạy từ đầu đến cuối suôn sẻ, nên khuyến nghị nâng cấp trả phí, để đảm bảo dự án có thể xây dựng hoàn chỉnh.
  ![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image26.png)

### 6. Trae (IDE)

- **Loại nền tảng:** Ứng dụng desktop (PC)
- **Đặc điểm chính và workflow:** Là ứng dụng desktop, Trae so với công cụ Web thường có ưu thế hơn về hiệu năng và tốc độ phản hồi. Nhưng nó cần tải và cài đặt, đối với một số người dùng rào cản ban đầu hơi cao. Tương tự, vì là môi trường cục bộ, sự khác biệt về cấu hình máy và môi trường dependency sẽ mang lại một số không chắc chắn. Ưu điểm là Trae sẽ giúp bạn hoàn thành tạo dự án và cấu hình chạy ở cục bộ, bạn có thể trực tiếp phát triển và debug trên máy.
- **Người dùng phù hợp:** Phù hợp hơn cho người dùng kế hoạch tiến hành dự án Vibe Coding dài hạn, và muốn sử dụng tổ hợp công cụ desktop chuyên dụng. Đối với người chỉ muốn "thỉnh thoảng chơi thử", có thể không phải lựa chọn nhẹ nhất.
- **Quá trình prompt:**
  ![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image27.png)
- **Hiệu quả trò Snake:**

![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image28.png)![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image29.png)

- **Giá:** Giá tương đối hợp lý, kể cả phiên bản miễn phí cũng đủ để hoàn thành dự án nhỏ chất lượng khá.
  ![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image30.png)

### 7. V0 (Web-based)

- **Loại nền tảng:** Web
- **Đặc điểm chính và workflow:** V0 là một công cụ tập trung vào tạo component UI React, do Vercel cung cấp. Nó thể hiện xuất sắc trong việc tạo giao diện chất lượng cao, có thể dùng cho môi trường production. Nhưng trong sử dụng thực tế, sẽ gặp những vấn đề như "khó tìm code view", "không nói rõ API Key nên cấu hình ở đâu".
- **Người dùng phù hợp:** V0 rất phù hợp cho sinh viên hoặc nhà thiết kế tập trung vào frontend và UI/UX. Nhưng nó không phải giải pháp fullstack hoàn chỉnh, bạn vẫn cần sử dụng nền tảng khác để triển khai logic backend và tích hợp API, vì vậy nếu mục tiêu của bạn là "xây ứng dụng hoàn chỉnh tại chỗ", nó có thể không phải lựa chọn hàng đầu.
- **Quá trình prompt:**
  ![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image31.png)

  ![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image32.png)

- **Hiệu quả trò Snake:**
  ![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image33.png)![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image34.png)
- **Giá:** Người dùng miễn phí khoảng có thể xây dựng 4-5 dự án đơn giản.
  ![](../../../../vi-vn/stage-1/appendix-articles/example0-1/images/image35.png)

## 3. Bảng so sánh tổng kết nền tảng

| **Nền tảng**                                   | **Đánh giá**                                                                     | **Platform** | **Ghi chú**                                                                      |
| ------------------------------------------ | ------------------------------------------------------------------------------ | ------------ | ------------------------------------------------------------------------------ |
| **[Lovable](https://lovable.dev/)**        | Rất thân thiện với người mới lập trình AI, dễ bắt đầu, trải nghiệm mượt mà, là lựa chọn khởi đầu lý tưởng.                 | Web-based    | Tự động hoàn tất kết nối Supabase, giảm chi phí cấu hình.                                   |
| **[Cursor](https://cursor.com/cn/agents)** | Phù hợp người dùng đã có kinh nghiệm phát triển, nâng cao năng suất và chất lượng code đáng kể.                             | PC           | Cần nền tảng lập trình nhất định, cần tự hiểu cấu trúc dự án và dependency trong môi trường cục bộ.                         |
| **[Z.ai](https://chat.z.ai/)**             | Phù hợp hơn cho người có nền tảng lập trình, muốn trực tiếp nghiên cứu chi tiết code AI output.                           | Web-based    | Không có cửa sổ xem trước, kiểm tra kết quả khá phiền; cần thủ công paste code, tạo thư mục và file và chạy service thủ công. |
| **[Replit](https://replit.com/~)**         | Khuyến nghị cho người muốn nhanh biến ý tưởng thành dịch vụ online có thể truy cập.                                   | Web-based    | Phát triển và triển khai trực tuyến tất cả trong một, hỗ trợ phối hợp và cung cấp editor trực quan.                             |
| **[Minimax](https://agent.minimaxi.com/)** | Phù hợp người muốn xem toàn bộ quá trình AI tự động tìm và sửa lỗi, và học từ đó, nhưng tổng thể khá chậm và tốn Token. | Web-based    | Toàn bộ quá trình khá dài, AI sẽ nhiều lần tự động chạy test và sửa lỗi.                                |
| **[Trae](https://www.trae.ai/)**           | Dành cho người có kinh nghiệm lập trình, muốn sử dụng tổ hợp desktop IDE + AI Agent, là công cụ nâng cao hiệu quả mạnh mẽ. | PC           | Cần cài đặt cục bộ và cấu hình môi trường, nhưng hiệu năng tốt hơn, phù hợp tiến hành dự án Vibe Coding dài hạn.              |
| **[V0](https://v0.app/)**                  | Tối ưu cho người phi nhà phát triển muốn nhanh tạo hiệu ứng UI React, phù hợp sinh viên hướng frontend / thiết kế.  | Web-based    | Tập trung tạo UI React, cần phối hợp với nền tảng khác hoàn thành backend và xây dựng ứng dụng hoàn chỉnh.                  |
