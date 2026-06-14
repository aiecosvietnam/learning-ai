# Dùng Agent thiết kế và lập trình thiết kế trang web

## Hướng dẫn chương này

Chương này sẽ trình bày thiết kế và phát triển có thể hợp tác hoàn hảo thông qua AI như thế nào. Bạn sẽ đóng vai trò product manager, chỉ huy "Agent thiết kế" hoàn thành thiết kế Logo, phối màu và bố cục trang, rồi phối hợp với "Agent lập trình" chuyển bản thiết kế thành code có thể chạy. Từ hình thành ý tưởng đến trang web lên mạng, trải nghiệm toàn bộ quy trình phát triển được AI nâng cao, khiến một người trở thành một đội ngũ.

---

# 1. Hướng dẫn bắt đầu

## 1. Giới thiệu hướng dẫn

Hãy sử dụng AI Design Agent và Coding Agent để xây dựng một trang web hoàn chỉnh từ đầu.

- **Agent thiết kế**: Chịu trách nhiệm tạo logo, bố cục trang web, phối màu và các yếu tố hình ảnh khác
- **Agent lập trình**: Viết code thực tế HTML/CSS/JS, v.v. dựa trên yêu cầu và bố cục bạn đưa ra trong prompt, xây dựng trang web có thể chạy

## 2. Agent thiết kế và Agent lập trình

- **Agent thiết kế**: AI tạo hình ảnh, mô hình trang hoặc phong cách thiết kế dựa trên prompt bạn cung cấp.
- Mastergo
- Lovart
- Figma MCP
- **Agent lập trình**: AI viết code thực tế (HTML/CSS/JS, v.v.) dựa trên chức năng và bố cục bạn yêu cầu trong prompt.
- Z.AI
- Trae
- Cursor
- Lovable

---

# 2. Sử dụng Agent thiết kế tạo Logo

## 1. Các yếu tố cần cân nhắc khi thiết kế Logo

Logo là một trong những yếu tố quyết định ấn tượng đầu tiên về trang web của bạn. Để nhận kết quả hài lòng từ Agent thiết kế AI, bạn cần mô tả rõ loại Logo bạn muốn trong prompt.

1. **Tên thương hiệu / Văn bản**

- Văn bản phải xuất hiện trong Logo (ví dụ: tiêu đề trang web, tên thương hiệu, v.v.).

2. **Phong cách (tâm trạng / bầu không khí)**

- Cảm giác hoặc bầu không khí tổng thể mà Logo muốn truyền tải.
- _Ví dụ: Tối giản, dễ thương, gọn gàng, hiện đại, retro, tương lai, v.v._

3. **Phối màu** (tùy chọn)

- Tốt nhất nên để phối màu Logo phù hợp với tông tổng thể của toàn trang web.
- Có thể chỉ định mã hex cụ thể, hoặc gam màu chung (màu lạnh, màu ấm, v.v.).
- _Ví dụ: **`#171721`** (đen), **`#FF7130`** (cam)._

4. **Hình thức (hình dáng / cấu trúc)**

- Làm rõ Logo có cần hình dáng hoặc bố cục cụ thể không.
- _Ví dụ: Chữ trong vòng tròn, tổ hợp icon + chữ, Logo lấy icon làm chủ đạo, v.v._

5. **Yếu tố icon / biểu tượng** (tùy chọn)

- Đồ họa hoặc biểu tượng muốn xuất hiện trong Logo.
- _Ví dụ: Icon sách, biểu tượng tia sét, đồ họa liên quan AI, hình học trừu tượng, v.v._

## 2. Viết prompt thiết kế Logo

**Prompt ví dụ**

```
"Xin thiết kế cho tôi một Logo phong cách tối giản, tên thương hiệu là 'My First Website'.
Sử dụng đen (#171721) và cam (#FF7130), và đặt chữ bên trong một vòng tròn."
```

```
"Xin thiết kế một Logo với tên thương hiệu 'AIID'.
Phong cách tổng thể phải có cảm giác tương lai, sạch sẽ gọn gàng, màu chủ đạo là xanh và trắng.
Kết hợp đồ họa trừu tượng tượng trưng cho AI với chữ, và xuất ra dưới dạng PNG với nền trong suốt."
```

## 3. Yêu cầu thiết kế từ Agent

- Nhập prompt trên → So sánh nhiều bản thiết kế do Agent tạo.

![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image1.png)![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image2.png)

## 4. Xác định Logo cuối cùng

- Chọn phiên bản bạn thích nhất từ bản nháp và tải xuống.

---

# 3. Lập kế hoạch cấu trúc trang web

## 1. Hiểu các khu vực cơ bản

Trước khi thực sự bắt đầu làm trang web, lập kế hoạch các menu (khu vực) muốn bao gồm rất quan trọng. Thiết kế menu phụ thuộc vào việc bạn muốn khách truy cập thấy gì, và muốn họ thực hiện hành động gì.
Nói chung, trang web thường bao gồm các khu vực cơ bản như **Home / About / Contact**.

## 2. Tự vẽ sketch cấu trúc (tùy chọn)

Bạn có thể trước viết ra một cấu trúc menu đơn giản dựa trên mục tiêu trang web.

### Menu cơ bản

1. **Home**
   1. Trang chính mà khách truy cập thấy đầu tiên sau khi vào trang web
   2. Thường bao gồm Logo, hero area và một câu slogan hoặc giới thiệu ngắn
2. **About**
   1. Giới thiệu bạn là ai, hoặc mục đích dự án / dịch vụ
   2. Portfolio cá nhân: Tự giới thiệu + CV ngắn
   3. Trang dịch vụ: Tầm nhìn, mục tiêu và chức năng cốt lõi
3. **Contact**
   1. Thông tin liên hệ, như email, số điện thoại, link mạng xã hội, v.v.
   2. Cũng có thể thêm một form liên hệ đơn giản

### Menu tùy chọn

4. **Services / Projects**
   1. Hiển thị dịch vụ bạn cung cấp, hoặc dự án / portfolio của bạn
   2. Thường hiển thị dạng danh sách hoặc card

5. **Gallery**
   1. Dùng để hiển thị hình ảnh, ảnh hoặc tác phẩm thiết kế

6. **Blog / News**
   1. Dùng để xuất bản bài viết, cập nhật hoặc nhật ký

7. **FAQ**
   1. Tổng hợp các câu hỏi và câu trả lời khách truy cập thường hỏi

## 3. Chọn phối màu (tùy chọn)

Nếu bạn đã có Logo, hoặc muốn dùng kết hợp màu cụ thể để thiết kế trang web, cũng có thể trực tiếp viết mã màu bạn muốn sử dụng trong prompt.

**Ví dụ:** `#171721, #872B97, #FF7130, #FF3C68`

Kể cả bạn tạm chưa nghĩ ra phối màu nào, cũng có thể tìm cảm hứng qua trang web phối màu hoặc tìm kiếm từ khóa.

- **Trang web tham khảo phối màu**
  - https://colorhunt.co/
  - https://coolors.co/

![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image3.png)![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image4.png)

- **Tìm kiếm phối màu qua từ khóa trên Google**

![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image5.png)

## 4. Viết prompt thiết kế trang web

**Prompt ví dụ**

```
"Xin thiết kế một trang web một trang bao gồm 3 khu vực Home, About, Contact.
Sử dụng phối màu #171721, #FF7130 và #FF3C68.
Phong cách tổng thể hiện đại, gọn gàng."
```

---

# 4. Sử dụng Agent thiết kế thiết kế trang web

## 1. Nhập prompt → Tạo bản thiết kế

- Viết cấu trúc đã lên kế hoạch và phối màu đã chọn trong prompt.

**Ví dụ prompt Mastergo**

![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image6.png)![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image7.png)

## 2. Xem xét bản thiết kế và đưa ra ý kiến sửa đổi

Bạn có thể đưa ra phản hồi cho Agent theo nhu cầu của mình, ví dụ:

- "Quá sặc sỡ, đổi phong cách tổng thể gọn gàng hơn."
- "Đổi font khác."
- "Điều chỉnh phối màu."
- "Xóa phần này đi."

![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image8.png)

## 3. Xác định thiết kế cuối cùng

Khi bạn đã sửa đổi nhiều vòng và hài lòng với bản thiết kế, có thể chuyển thiết kế này thành code, để Coding Agent hiểu và tiếp tục làm việc.

Cách chuyển thiết kế thành code sẽ khác nhau tùy nền tảng, nhưng thường là cài đặt và sử dụng một số plugin trong nền tảng thiết kế.

**Ví dụ Mastergo**

1. Mở [trang plugin Mastergo](https://mastergo.com/community/plugin), tìm **seal**.

![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image9.png)

2. Quay lại trang thiết kế, click **icon hình vuông (plugin)**.

![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image10.png)

3. Chọn vùng thiết kế bạn muốn chuyển thành code, click nút **Generate** để tạo code.

![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image11.png)

---

# 5. Sử dụng Coding Agent xây trang web

## 1. Hiểu khái niệm cơ bản HTML/CSS/JS

Bản chất một trang web gồm ba ngôn ngữ:

- **HTML (HyperText Markup Language)** → Cấu trúc (bộ xương)
- **CSS (Cascading Style Sheets)** → Phong cách (ngoại hình)
- **JavaScript (JS)** → Chức năng (tương tác)

Ba thứ phối hợp với nhau, tạo thành trang web hoàn chỉnh mà chúng ta nhìn thấy.

1. **🏗️ HTML (Cấu trúc)**

- Định nghĩa "hiển thị gì" trên trang
- Dùng để đặt các yếu tố như văn bản, hình ảnh, nút bấm, link
- Tương tự như **tường và khung** của tòa nhà

**Ví dụ**

```html
<h1>Hello!</h1>
<p>This is my first website.</p>
<a href="contact.html">Contact</a>
```

2. **🎨 CSS (Phong cách)**

- Quyết định "nội dung hiển thị thế nào"
- Điều khiển kích thước chữ, màu sắc, khoảng cách, nền, hình dạng nút, v.v.
- Cho HTML có "quần áo" và phong cách hình ảnh

**Ví dụ**

```css
h1 {
  color: #FF7130;   /* Text color */
  font-size: 36px;  /* Font size */
  text-align: center; /* Center alignment */
}

body {
  background-color: #171721; /* Background color */
  color: white; /* Default text color */
}
```

3. **⚙️ JavaScript (JS) (Chức năng)**

- Khiến trang web có thể tương tác với người dùng
- Có thể triển khai các hiệu ứng động như click nút, mở menu, slideshow ảnh, submit form
- Nếu HTML/CSS là bộ xương và ngoại hình tĩnh, thì JS là **bộ não** khiến trang web "sống động"

**Ví dụ**

```javascript
function showAlert() {
  alert("The button has been clicked!");
}
```

```html
<button onclick="showAlert()">Click me</button>
```

## 2. Để Coding Agent tạo code

**Prompt ví dụ**

```
"Xin viết HTML và CSS cho một trang web một trang bao gồm các khu vực Home, About và Contact.
Sử dụng phối màu #171721, #FF7130, #FF3C68.
Nền đen, chữ trắng."
```

![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image12.png)

## 3. Chạy trang web

Khi code nháp đã được tạo, Agent thường sẽ tự động khởi động dự án và hiển thị trang web đã tạo.

Nếu bạn khởi động lại Agent, hoặc trang web không hiển thị, có thể nhập prompt kiểu như sau:

```
"Please activate the project"
```

Để Agent khởi động lại dự án và mở trang xem trước, tiện bạn xem hiệu quả hiện tại.

## 4. Sửa đổi đơn giản

Bạn có thể tiếp tục tinh chỉnh bản nháp thông qua ngôn ngữ tự nhiên, ví dụ:

- "Làm nút to hơn."
- "Font đậm hơn."

![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image13.png)![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image14.png)

## 5. Sửa đổi nội dung văn bản trang web

Trang web phiên bản đầu do Agent tạo, thường bao gồm một số văn bản placeholder tự động tạo. Để nó gần hơn với kịch bản thực tế của bạn, bạn có thể chuẩn bị nội dung thực tế trước, rồi để Agent giúp bạn thay thế.

**Ví dụ ứng dụng:** Cập nhật trang About của trang web AIID

1. Trước viết xong nội dung bạn muốn hiển thị trên trang About. Để Agent dễ hiểu, có thể lưu nội dung dưới định dạng Markdown.

![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image15.png)

2. Sau đó nói với Agent trong hội thoại, áp dụng nội dung từ file này lên trang được chỉ định.

![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image16.png)

3. Xem phiên bản cập nhật sau khi áp dụng nội dung.

![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image17.png)

## 6. Chèn hình ảnh

Nếu bạn muốn thêm hình ảnh cụ thể (ví dụ Logo, ảnh nền, v.v.), có thể trước upload hình ảnh vào thư mục dự án, sau đó trong prompt nói rõ muốn sử dụng hình ảnh này ở vị trí nào trên trang.

- **Ví dụ:**

![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image18.png)![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image19.png)![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image20.png)

- **Kết quả:**

![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image21.png)

---

# 6. Tích hợp thiết kế và code

## 1. Tích hợp file thiết kế và code trang web (tùy chọn)

Khi bạn đã tải xuống file code từ Agent thiết kế, có thể di chuyển chúng vào thư mục dự án hiện tại, rồi nhờ Coding Agent giúp bạn hợp nhất code thiết kế này với dự án hiện có.

- **Ví dụ:**

![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image22.png)

- **Kết quả:**

![](../../../../vi-vn/stage-1/appendix-articles/example0-2/images/image23.png)
