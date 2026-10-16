# Đưa bản portfolio này vào repository đã tạo

Repository người dùng cung cấp: `https://github.com/khoana3105-svg/Rever-apartment-analysisHCM`. Công cụ web chưa truy cập được URL trong lần kiểm tra; không khẳng định repo chưa tồn tại hoặc đã Public. Chưa upload/commit/push trong phiên này.

## Xem trước trên máy

1. Mở `README.md` bằng Markdown Preview trong VS Code.
2. Mở `notebooks/01_rever_market_analysis.ipynb` và đọc bảng/biểu đồ đã lưu.
3. Chọn Python kernel có pandas, NumPy, Matplotlib; Run All để xác nhận trong IDE của bạn. Notebook không scrape web, không huấn luyện ML và không cài package.
4. Đọc phần giới hạn: snapshot chưa xác nhận ngày thu thập, toàn bộ ngày đăng thiếu, khác biệt địa bàn có thể do cơ cấu mẫu.

## Upload bằng trình duyệt

Sau khi bạn đã rà soát và muốn đưa nội dung lên repo:

1. Mở repository khi đang đăng nhập GitHub.
2. Với repo trống, chọn **uploading an existing file**; nếu đã có file, chọn **Add file → Upload files**.
3. Chọn đúng các thành phần sau, giữ nguyên cấu trúc thư mục:

```text
README.md
.gitignore
requirements.txt
notebooks/
outputs/
docs/
data/README.md
```

**Không kéo nguyên thư mục dự án:** CSV đang có trong `data/` chỉ phục vụ chạy cục bộ. `.gitignore` không bảo vệ thao tác upload thủ công. Không upload CSV, thư mục Data Mining UEL, CV hoặc ảnh/chứng chỉ cá nhân.

4. Kiểm tra danh sách file hiển thị. Commit message đề xuất: `Add Rever analysis notebooks and portfolio summary`.
5. Bấm **Commit changes** khi bạn đã sẵn sàng lưu lên GitHub.
6. Mở README và notebook trên GitHub, kiểm tra hình và bảng hiển thị. Nếu repo Private, HR chưa xem được; chuyển Public sau khi đã rà nội dung bạn muốn công khai.

## Sau khi có nội dung trên GitHub

Link repository có thể đặt cạnh tên Rever trong CV sau khi kiểm tra truy cập. Chỉ ghi kết quả mới trong CV khi bạn đã đọc, chạy lại và hiểu chúng. Chưa sửa CV để nhận các kết quả DA mới như một phần bạn đã tự kiểm tra.

## Ba câu hỏi luyện giải thích

1. Vì sao không lấy trung bình giá làm kết luận chính khi phân bố lệch phải?
2. Vì sao Quận 2 có trung vị đơn giá cao hơn chưa chứng minh vị trí gây ra giá cao?
3. Vì sao không dùng giá chào tin đăng để tuyên bố giá giao dịch hoặc lợi nhuận đầu tư?
