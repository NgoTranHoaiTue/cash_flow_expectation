## **GIỚI THIỆU ĐỀ TÀI**
### *Lý do chọn đề tài*
Hoạt động của Ngân hàng thương mại hiện nay đang diễn ra ngày càng mạnh mẽ và trở thành xu thế tất yếu đối với bất cứ nền kinh tế nào. Sự đa dạng hóa của các sản phẩm tài chính biến động không ngừng, tuy nhiên cũng không tránh khỏi nhiều rủi ro và khó kiểm soát. Dòng tiền vô cùng quan trọng với các nhà đầu tư, do đó việc định giá dòng tiền sẽ giúp cho các nhà đầu tư đánh giá và đưa ra quyết định tránh được những mất mát không đáng có. Nghiên cứu về định giá dòng tiền nhằm mang lại hiệu quả kinh tế tốt nhất, vì vậy rất có ý nghĩa trên cả góc độ lí luận và thực tiễn. 
-	Xét trên góc độ lí luận: vấn đề định giá dòng tiền được đề cập tại nhiều công trình nghiên cứu khác nhau. Tuy nhiên chưa có sự thống nhất cả các nhân tố trong dòng tiền. Vì vậy cần có thêm các nghiên cứu về định giá dòng tiền để tổng quan các công trình nghiên cứu trước. 
-	Xét trên góc độ thực tiễn: công tác định giá dòng tiền ở nước ta còn đơn giản, chưa thực sự đánh giá đúng mức ảnh hưởng của nó. Với các nhà đầu tư, nhà quản lí kinh tế, .. định giá dòng tiền tương lai đóng vai trò vô cùng quan trọng trước khi đưa ra quyết định kinh tế, điều này thực sự có ích khi giúp họ đánh giá được dòng tiền theo nhu cầu của họ.
### *Mục tiêu nghiên cứu*
Mục tiêu tổng quát của đề tài là tiến hành xây dựng và so sánh các mô hình định giá dòng tiền của các NHTM tại Việt Nam để tìm ra yếu tố nào mang lại lợi nhuận tốt nhất. 
Đề tài cũng đặt ra các mục tiêu cụ thể sau:
- Thứ nhất, tổng hợp và hệ thống các cơ sở lý thuyết liên quan đến lãi suất và dòng tiền, tổng hợp lãi suất theo từng kì của các NHTM hiện nay. 
- Thứ hai, xây dựng mô hình định giá dòng tiền, xác định lãi suất và kì hạn của ngân hàng nào mang lại lợi nhuận tốt nhất, phù hợp với từng nhu cầu của nhà đầu tư
- Thứ ba, thiết kế giao diện ước tính giá trị tương lai dòng tiền, và vẽ các biểu đồ nhằm phục vụ cho việc so sánh một cách cụ thể hơn. 
### *Phương pháp nghiên cứu*
-	Phương pháp thống kê và tổng hợp: Crawl dữ liệu lãi suất của các ngân hàng. 
-	Phương pháp khác: Sử dụng streamlit để hỗ trợ việc tạo giao diện bằng Python. 
#### **I. Định nghĩa**
##### **1. Giá trị theo thời gian của tiền**
- Theo góc độ tài chính, tiền không ngừng vận động và sinh lời. Giữa tiền với thời gian và rủi ro có quan hệ mật thiết với nhau. Mối quan hệ đó được thể hiện thông qua lãi suất. 
- Đồng tiền nhận được ở các thời điểm khác nhau sẽ có giá trị không giống nhau. Một đồng tiền hôm nay có giá trị hơn một đồng tiền trong tương lai. Giá trị theo thời gian của tiền được cụ thể hóa bởi hai khái niệm cơ bản là giá trị tương lai (FV) và giá trị hiện tại (PV)
##### **2. Lãi suất**
- Lãi suất là tỷ lệ phần trăm phát sinh từ giao dịch cho vay giữa các bên. Số tiền này được gọi là tiền lãi mà người vay tiền cần phải trả thêm cho người cho vay
- Lãi suất ngân hàng là tỷ lệ phần trăm quy định trong hợp đồng vay, mượn giữa tiền vốn gửi vào hoặc cho vay với mức lãi suất trong khoảng thời gian nhất định do ngân hàng đưa ra hoặc do bên vay và bên cho vay tự thỏa thuận để phù hợp.
##### **3. Giá trị hiện tại**
- Giá trị hiện tại của tiền là giá trị của khoản tiền phát sinh trong tương lai được quy về thời điểm hiện tại (thời điểm gốc) theo một tỷ lệ chiết khấu nhất định
- Thời điểm phát sinh khoản tiền càng xa thời điểm hiện tại thì giá trị hiện tại của khoản tiền càng nhỏ.
- Lãi suất chiết khấu hay tỷ lệ hiện tại hoá càng lớn thì giá trị hiện tại của khoản tiền càng nhỏ.
##### **4. Giá trị tương lai**
- Giá trị tương lai của một khoản tiền là giá trị có thể nhận được tại một thời điểm trong tương lai, bao gồm số vốn gốc và toàn bộ tiền lãi tính đến thời điểm đó. Yếu tố ảnh hưởng trực tiếp đến giá trị tương lai của tiền là phương pháp tính lãi
- Trong thực tế, chúng ta thường gặp trường hợp có nhiều khoản tiền phát sinh liên tục theo những khoảng thời gian bằng nhau (điển hình như việc gửi tiết kiệm vào ngân hàng) tạo thành một chuỗi các khoản tiền. Khoảng cách giữa hai khoản tiền phát sinh được tính theo năm, theo quý hoặc theo tháng còn gọi là một kỳ. Tùy theo thời điểm phát sinh các khoản tiền ở đầu kỳ hay cuối kỳ mà người ta sẽ có cách phân biệt và tính toán khác nhau
- Trong đề tài này chúng ta sẽ sử dụng công thức tính giá trị tương lai của dòng tiền đều cuối kỳ khi biết giá trị hiện tại cũng như khoản tiền thanh toán từng kỳ và dựa vào lãi suất thực tế của các ngân hàng hiện nay để tính toán giá trị tương lai của khoản tiền gửi tiết kiệm hoặc vay vốn
> $$ FV = PV(1 + r)^{nper} + PMT \left [\frac{(1 + r)^{nper} - 1}{r} \right ] $$


Trong đó:
- FV: giá trị tương lai sẽ nhận được
- PV: giá trị hiện tại của khoản tiền
- r: lãi suất ngân hàng quy định
- PMT: khoản tiền thanh toán theo từng kỳ cố định
- nper: số kỳ ghép lãi
#### **II. Định giá dòng tiền**
##### **1. Gửi tiết kiệm**
- Gửi tiết kiệm có kỳ hạn là hình thức gửi tiết kiệm trong một khoảng thời gian nhất định và khoảng thời gian này được người gửi thỏa thuận với ngân hàng ngay từ khi mở sổ tiết kiệm. Đây là hình thức gửi tiền được khách hàng ưa chuộng
- Khi gửi tiết kiệm có kỳ hạn, người gửi chỉ có thể nhận đủ số lãi theo dự tính ban đầu khi kết thúc kỳ hạn. Nếu rút tiền trước kỳ hạn, khách hàng chỉ được hưởng mức lãi suất thấp hơn.
##### **2. Vay vốn**
- Vay vốn ngân hàng là số tiền mà cá nhân hoặc doanh nghiệp vay mượn từ ngân hàng và sẽ trả lãi theo kỳ hạn do ngân hàng quy định hoặc có thỏa thuận từ trước.
##### **3. Tại sao nên vay vốn/ gửi tiết kiệm**
*Tại sao nên vay vốn*

Một cá nhân hoặc doanh nghiệp có nhiều lý do dựa trên nhu cầu riêng để thực hiện vay vốn ngân hàng khi gặp khó khăn tài chính:
- Khi có nhu cầu mua một tài sản cá nhân với số tiền lớn (nhà cửa, xe cộ,...)
- Cần mở rộng hoạt động sản xuất kinh doanh nhưng chưa đủ vốn

Việc vay tiền không chỉ dành cho người gặp khó khăn tài chính mà cả những người dư dả tài chính, thông thường người giàu lại đi vay khá nhiều từ các ngân hàng. Việc sử dụng hiệu quả khoản tiền vay vốn có thể mang lại lợi nhuận cho bản thân.

*Tại sao nên gửi tiết kiệm*

Trong cuộc sống chúng ta sẽ phải đối mặt với những tình huống bất ngờ xảy ra không đoán trước được. Để đề phòng cho những trường hợp khẩn cấp chúng ta nên có những khoản tiết kiệm để dễ dàng xoay sở bất cứ lúc nào.

Để thực hiện các mục tiêu ngắn hạn (mua điện thoại, xe cộ) hay những mục tiêu dài hạn (mua nhà, lập gia đình) chúng ta cần phải chuẩn bị ngay cho bản thân khoản tiền tương lai dư dả để có thể hoàn thành các mục tiêu đề ra.

##### **4. Lợi ích của việc dự đoán dòng tiền**
Dưới tác dụng của lãi suất, với thời gian dài thì giá trị của đồng tiền đã có sự thay đổi lớn. Việc quy đổi giá trị tương lai của khoản tiền về giá trị hiện tại giúp chúng ta xem xét mức độ sinh lời của khoản tiền khi gửi tiết kiệm hay khả năng chi trả khi vay vốn.

Thứ hai, việc quy đổi số lượng tiền trong tương lai về hiện tại giúp chúng ta dự báo các trường hợp có thể xảy ra từ đó đưa ra biện pháp quản lý rủi ro hay phát huy tối đa lợi ích của khoản tiền mang lại. 
#### **III. Quy trình thiết kế giao diện định giá dòng tiền**

##### **1. Các Package cần sử dụng**
|Package          | Mô Tả         |
|-----------------|---------------|
| Pandas          | Cung cấp, thiết kế và khởi tạo các cấu trúc dữ liệu như bảng, đa chiều, chuỗi thời gian một cách nhanh chóng, linh hoạt nhằm hỗ trợ cho việc phân tích dữ liệu|
| numpy           | Dùng để hỗ trợ thêm cho các mảng ma trận lớn, đa chiều|
|numpy_financial  | Một tập hợp cung cấp các chức năng tài chính cơ bản|
|beautifulsoup4| Dùng cho việc thu thập dữ liệu từ các trang web trở nên dễ dàng hơn|
|streamlit| Là một framework mã nguồn mở dành cho các nghiệp vụ học máy và phân tích dữ liệu, chuyển đổi các dòng code tính toán, khởi tạo giao diện thành một trang web| 
##### **2. Các thuật toán liên quan**

*Thuật toán PV*

Dùng để tính toán giá trị hiện tại của dòng tiền. 

Cấu trúc như sau:

>$$numpy-financial.pv(rate, nper, pmt, fv, when='end') $$

*Thuật toán FV*

Dùng để tính toán giá trị tương lai của dòng tiền. 

Cấu trúc như sau:
>$$numpy-financial.fv(rate, nper, pmt, pv, when='end')$$

*Thuật toán PMT*

Dùng để tính toán lượng tiền gửi tiết kiệm/trả nợ vay theo từng kỳ của dòng tiền. 

Cấu trúc như sau:

>$$numpy-financial.pmt(rate, nper, pv, fv, when='end')$$
##### **3. Phương pháp tạo giao diện**
- **Bước 01**: Nhập các thư viện vào, tiêu biểu là pandas, numpy, Streamlit
- **Bước 02**: Thu thập, chuẩn bị sẵn bộ dữ liệu lãi suất kỳ hạn tiết kiệm/vay của các ngân hàng
- **Bước 03**: Phác thảo, thiết kế giao diện, canh vị trí, gán tên cho các khung chức năng trong trang web
- **Bước 04**: Nhập các lệnh điều kiện, truy vấn, các thuật toán, công thức tính toán các giá trị hiện tại, tương lai, lượng tiền gửi tiết kiệm/trả nợ vay theo từng kỳ của dòng tiền, các lệnh tạo biểu đồ, đồng thời trích dẫn bộ dữ liệu lãi suất vào bảng, biểu đồ và thuật toán làm cơ sở tính toán
- **Bước 05**: Thêm, chỉnh sửa các chức năng, bảng biểu, phông nền... để làm trang web tiện lợi và ưa nhìn hơn
- **Bước 06**: Chạy code để triển khai trang web tính toán dòng tiền lên ứng dụng Streamlit

#### **IV. Kết luận** 
Nhóm thiết kế trang web tính toán dòng tiền qua ứng dụng Streamlit nhằm:
- Giúp cho người dùng có thể dễ dàng tính toán, ước tính được giá trị cần thiết cũng như thấy được lượng tiền qua từng kỳ của mình biểu hiện qua biểu đồ.
- Cung cấp cho người dùng chức năng so sánh khi gửi tiết kiệm/vay vốn với các lãi suất kỳ hạn khác nhau của cùng một ngân hàng.
- Hỗ trợ so sánh, tính toán giá trị và dòng tiền giữa các ngân hàng khác nhau.

Từ đó giúp người dùng có thể đưa ra biện pháp tối ưu nhất trong việc gửi tiết kiệm cũng như vay vốn.
