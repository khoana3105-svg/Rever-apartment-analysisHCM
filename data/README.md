# Dữ liệu cục bộ

Notebook đọc file `rever_apartments_clean_fetcher.csv` tại thư mục này. Bản CSV nguồn được sao chép cục bộ từ dự án hiện có để chạy lại, không nằm trong danh sách upload.

Nguồn: tin đăng căn hộ Rever.vn do tác giả thu thập. Ngày thu thập chưa xác nhận; trường ngày đăng thiếu toàn bộ trong snapshot. Một dòng là một tin đăng, không đảm bảo một căn hộ duy nhất. Dữ liệu đã qua bước làm sạch của bài học phần; notebook DA kiểm tra lại đầu vào sạch chứ không tái dựng HTML/raw.

Các cột bắt buộc của notebook DA: `listing_id`, `price_vnd`, `area_m2`, `district`. Notebook ML cần thêm `bedrooms`, `bathrooms`, `balcony_direction`. Bảng missingness trong notebook thể hiện schema đầy đủ của CSV gốc; README công khai không chứa dữ liệu từng tin.

SHA-256 của snapshot và phiên bản thư viện được ghi ở `docs/provenance.json`. Người chạy cần có bản dữ liệu được phép sử dụng và đặt đúng tên; notebook không tự tạo dữ liệu giả thay thế.

Trước khi chia sẻ lại dữ liệu, cần xác định điều kiện sử dụng nguồn và rà nội dung cá nhân. `.gitignore` chỉ có tác dụng với Git; upload thủ công bằng trình duyệt vẫn có thể gửi nhầm file, vì vậy không chọn CSV để upload.
