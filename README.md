# Vietnamese-Spelling-Correction

Dự án này cung cấp một hệ thống sửa lỗi chính tả tiếng Việt dựa trên mô hình học sâu, sử dụng kiến trúc Transformer và kỹ thuật mã hóa Byte Pair Encoding (BPE).
Hệ thống có khả năng phát hiện và sửa lỗi chính tả trong văn bản tiếng Việt với độ chính xác cao.

## 📌 Giới thiệu

Sửa lỗi chính tả là một bài toán quan trọng trong xử lý ngôn ngữ tự nhiên (NLP). 
Đối với tiếng Việt, việc sửa lỗi chính tả gặp nhiều thách thức do đặc điểm ngôn ngữ và cấu trúc từ phức tạp. 
Dự án này áp dụng mô hình Transformer kết hợp với kỹ thuật BPE để xây dựng hệ thống sửa lỗi chính tả hiệu quả.

## 🧠 Kiến trúc mô hình

- **Mã hóa Byte Pair Encoding (BPE):** Giúp giảm kích thước từ vựng và xử lý hiệu quả các từ chưa từng xuất hiện.
- **Mô hình Seq2Seq dựa trên Transformer:** Cho phép mô hình học được ngữ cảnh dài và mối quan hệ giữa các từ trong câu.
- **Huấn luyện trên dữ liệu tổng hợp:** Mô hình được huấn luyện trên tập dữ liệu tổng hợp với các lỗi chính tả được tạo ngẫu nhiên, giúp mô hình học được nhiều loại lỗi khác nhau.

## 📁 Cấu trúc thư mục

- `data/`: Chứa tập dữ liệu huấn luyện và kiểm tra.
- `GetData.ipynb`: Notebook để tải và xử lý dữ liệu.
- `TrainModel.ipynb`: Notebook để huấn luyện mô hình.
- `CorrectSpelling.ipynb`: Notebook để thử nghiệm mô hình sửa lỗi chính tả.
- `spellcheck_model`: Tệp mô hình đã được huấn luyện.
- `Xây-dựng-hệ-thống-sửa-lỗi-chính-tả.pptx`: Bài thuyết trình giới thiệu về dự án.

## 🚀 Hướng dẫn sử dụng

1. **Cài đặt các thư viện cần thiết:**

   ```bash
   pip install -r requirements.txt
   ```

2. **Tải và xử lý dữ liệu:**

   Chạy notebook `GetData.ipynb` để tải và xử lý dữ liệu huấn luyện và kiểm tra.

3. **Huấn luyện mô hình:**

   Chạy notebook `TrainModel.ipynb` để huấn luyện mô hình trên dữ liệu đã xử lý.

4. **Thử nghiệm mô hình:**

   Chạy notebook `CorrectSpelling.ipynb` để thử nghiệm mô hình sửa lỗi chính tả trên các câu đầu vào.

## 📊 Kết quả

Mô hình đạt được độ chính xác cao trong việc phát hiện và sửa lỗi chính tả trên tập dữ liệu kiểm tra. Cụ thể, mô hình đạt:

- **Tỷ lệ phát hiện lỗi:** 86.8%
- **Tỷ lệ sửa lỗi chính xác:** 81.5%

So với các phương pháp trước đó, mô hình này cải thiện hiệu suất phát hiện lỗi thêm 5.6% và sửa lỗi chính xác thêm 2.2%.

## 📚 Tài liệu tham khảo

- [VSEC: Transformer-based Model for Vietnamese Spelling Correction](https://arxiv.org/abs/2111.00640)
- [Hierarchical Transformer Encoders for Vietnamese Spelling Correction](https://arxiv.org/abs/2105.13578)

## 📄 Giấy phép
Nếu bạn cần thêm thông tin hoặc hỗ trợ, vui lòng liên hệ với [devk1ngz](https://github.com/devk1ngz).
