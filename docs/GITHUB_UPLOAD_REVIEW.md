# Kiểm tra repository sau upload — 16/10/2026

Đã đọc GitHub API không xác thực: repository `khoana3105-svg/Rever-apartment-analysisHCM` có `private=false`, branch `main`. Các file hiện nằm ở root, chưa giữ cấu trúc `notebooks/`, `outputs/`, `docs/`, `data/` của bản cục bộ.

## Điểm cần sửa

1. README trỏ vào thư mục chưa tồn tại, nên ảnh/link notebook nội bộ không khớp. Notebook DA cũng tìm CSV trong `data/`, trong khi CSV hiện ở root.
2. CSV đã xuất hiện trong repository công khai. Bản chuẩn bị chỉ định CSV dùng cục bộ; `.gitignore` không ngăn upload qua trình duyệt. Cần quyết định dữ liệu được phép chia sẻ lại hay chỉ giữ cục bộ trước khi tiếp tục.

## Khôi phục cấu trúc bằng giao diện GitHub

Với mỗi file, mở file → Edit (biểu tượng bút chì; notebook/ảnh có thể không có chế độ sửa phù hợp). Nếu có thể sửa đường dẫn ở ô tên, đổi theo bảng dưới rồi commit. Nếu không có chế độ sửa, dùng Git cục bộ để di chuyển, không cần tạo lại nội dung file.

| File hiện ở root | Đường dẫn đúng |
|---|---|
| `01_rever_market_analysis.ipynb` | `notebooks/01_rever_market_analysis.ipynb` |
| `Rever_Price_Segment_Classification_Port.ipynb` | `notebooks/Rever_Price_Segment_Classification_Port.ipynb` |
| `area_vs_price.png` | `outputs/area_vs_price.png` |
| `district_comparison.png` | `outputs/district_comparison.png` |
| `price_distributions.png` | `outputs/price_distributions.png` |
| `district_summary.csv` | `outputs/district_summary.csv` |
| `findings.txt` | `outputs/findings.txt` |
| `provenance.json` | `docs/provenance.json` |
| `UPLOAD_GUIDE_VI.md` | `docs/UPLOAD_GUIDE_VI.md` |

Giữ `README.md`, `.gitignore`, `requirements.txt` ở root. Thêm `data/README.md` từ bản cục bộ bằng **Add file → Create new file**, nhập đầy đủ đường dẫn và dán nội dung.

**CSV nguồn:** nếu không chia sẻ công khai, xóa file khỏi phiên bản hiện tại bằng giao diện GitHub và commit; lưu bản máy của bạn. Việc xóa ở commit mới không xóa bản trong lịch sử Git. Nếu đã xác nhận được phép chia sẻ và muốn giữ công khai, đặt đúng đường dẫn `data/rever_apartments_clean_fetcher.csv`, đồng thời điều chỉnh `.gitignore` và phần mô tả dữ liệu trong README cho nhất quán.

Không sửa hoặc xóa remote tự động trong lần kiểm tra này. Sau khi sửa, mở README và thử các link ảnh/notebook bằng cửa sổ ẩn danh; chạy notebook với CSV ở đúng đường dẫn cục bộ.

CV đã thêm link repository, bản Intern nhấn mạnh phân tích mô tả; bản AI giữ kết quả phân loại. Cần hoàn tất sửa cấu trúc repository trước khi nộp CV để người xem không gặp các link minh chứng lỗi.
