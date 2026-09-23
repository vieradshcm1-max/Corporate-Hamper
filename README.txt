VIER FINE WINES — Landing page "Quà Tết Doanh Nghiệp / Corporate Hamper"
Route đề xuất: /qua-tet-doanh-nghiep/

NỘI DUNG GÓI
  index.html      Trang hoàn chỉnh, tự chứa (HTML + CSS + JS inline)
  img/            Toàn bộ hình ảnh (WebP / PNG), lấy từ file gốc độ phân giải cao nhất
  fonts/          3 font self-host (woff2, có subset tiếng Việt) — không phụ thuộc Google Fonts
                    · Playfair Display  → hero & số liệu
                    · Newsreader        → heading
                    · Be Vietnam Pro    → nội dung

CẦN BẠN ĐIỀN 1 CHỖ DUY NHẤT
  Trong khối "NĂNG LỰC DANH MỤC RƯỢU VANG" (section #ruou-vang) có ô đánh dấu
  [số SKU] — tìm chuỗi  class="fill"  trong index.html và thay bằng con số thật.
  Ba ô còn lại đã có số liệu kiểm chứng được:
    · 12 quốc gia — theo bộ lọc "Quốc gia" đang công bố trên vierwines.com
    · 510K – 4,62TR — giá niêm yết thấp nhất / cao nhất đang hiển thị trên vierwines.com
    · Chiết khấu — viết định tính, chưa nêu %; bổ sung mức cụ thể nếu muốn công bố.

CẬP NHẬT MỚI NHẤT
  · Đã bỏ hẳn dải "Những chai vang trong bộ quà Tết năm nay" ở khối rượu vang.
    Mỗi chai giờ nằm trong đúng mức ngân sách dùng nó, ở thanh cuối mỗi thẻ.
  · Sáu mức ngân sách đổi từ danh sách dọc sang BĂNG CUỘN NGANG: một thẻ hiện
    đầy đủ, thẻ kế tiếp lộ ra ở mép phải. Điều hướng bằng 6 tab mức giá, hai nút
    mũi tên tới / lui, vuốt ngang, hoặc phím ← → khi băng đang được focus.
  · Mức "Dưới 1.000.000đ" đã có mô tả đầy đủ (bỏ phần hạt theo yêu cầu):
    Pago de Cirsus Oak Aged · Yến tươi tinh chất chà là · Yến tươi mật hoa thốt nốt
    — Quy cách: Hộp giấy đôi Vier Hoa Sen | Xanh dương.
  · Logo khách hàng: đã cắt hết lề trắng thừa trong file gốc và phóng to nhóm
    Vietcombank · VietinBank · BVBank · Agribank · Sen · Stavian · Gamuda Land ·
    Việt Thái · Satori · Việt Nam Quốc Yến · Văn phòng Chính phủ · Bộ Nông nghiệp
    và Môi trường (thêm Tôm Giống Số 1 cho cân hàng cuối).

CẬP NHẬT VÒNG NÀY (theo feedback.docx)
  1. Ảnh khối giới thiệu đổi sang THUMBNAIL CHO HAMPER copy.png; đã xoá dòng
     caption "QUÀ TẾT DOANH NGHIỆP VIER FINE WINES" bên dưới.
  2. Khối rượu vang: thay lưới "Nhà sản xuất" bằng khối năng lực danh mục
     (SKU · quốc gia · khoảng giá · chiết khấu cho khách hamper và đối tác nhập
     vang kinh doanh). Giữ nguyên button "Khám phá VIER Fine Wines".
  3. Logo wall: thêm Việt Nam Quốc Yến (logo mới) và HSC → 21 logo, lưới 7×3.
  4. Bảy set quà → SÁU MỨC NGÂN SÁCH, bỏ tên set và bỏ giá từng set:
       01  Dưới 1.000.000đ            05  2.500.000đ – 3.000.000đ
       02  1.000.000đ – 1.500.000đ    06  Trên 3.000.000đ
       03  1.500.000đ – 2.000.000đ
       04  2.000.000đ – 2.500.000đ
  5. Nút "XEM THÀNH PHẦN BỘ QUÀ" dạng button lớn thay cho dấu cộng nhỏ;
     cỡ chữ thành phần tăng từ 14px lên 16px (dòng phụ 12px → 13,5px).
  6. Dải hình chai rượu đổi sang 7 packshot trong folder "Hình chai rượu",
     tách nền và chuẩn hoá về cùng một khung 3:4.
  7. Đã xoá section "Quy trình — Từ ý tưởng đến món quà hoàn chỉnh".
  8. Đã xoá section "Why VIER · Proven capability".

LƯU Ý NỘI DUNG
  · Mức 04 (2–2,5 triệu) chưa có ảnh packshot cho chai V8 Rosso Puglia IGP —
    thanh chai vang ở thẻ này đang để ô trống nét đứt. Thả file ảnh chai vào
    folder "Hình chai rượu" là thay được ngay.
  · Mức 04 đang dùng ảnh set Hồng Phú Quý (cùng bộ hộp + túi cao cấp Camellia)
    vì folder chưa có file ảnh tên "Tết Giao Hoà".
  · Ảnh banner giới thiệu có sẵn hotline 090 980 96 43 in trong hình; ba hotline
    ở khối liên hệ vẫn là 0909 809 643 · 0909 172 665 · 0938 775 906.

TÍCH HỢP FORM
  Tìm chuỗi "INTEGRATION POINT" trong index.html (2 vị trí: thẻ <form> và khối
  JS xử lý submit). Thay khối JS bằng fetch() tới endpoint thật
  (WPForms / Contact Form 7 / HubSpot / Google Apps Script…).

TRIỂN KHAI WORDPRESS
  · Upload img/ và fonts/ giữ nguyên cấu trúc thư mục cạnh trang.
  · Nếu đổi đường dẫn asset, sửa tiền tố "img/" và "fonts/" trong index.html.
  · Trang luôn hiển thị nền sáng (đã gỡ Dark Mode), đã kiểm tra ở 1440px và 400px,
    không tràn ngang, không ảnh nào bị crop hay bóp méo.
