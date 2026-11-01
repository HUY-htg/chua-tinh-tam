# Chùa Tịnh Tâm 3D

Không gian chùa 3D trên trình duyệt: dạo bước sân chùa, thỉnh Đại Hồng Chung, thả hoa đăng, dâng hương và tụng kinh cùng tiếng mõ, chuông.

## Tính năng mới nổi bật

1. **Đồ hoạ tinh xảo (Cinematic 3D Fidelity)**:
   - Tích hợp chuẩn **ACES Filmic Tone Mapping** cho hình ảnh chân thực, chiều sâu và độ tương phản ấm áp chốn thiền môn.
   - Hệ thống bóng đổ mềm mại (**PCFSoftShadowMap**), luồng ánh sáng thiêng liêng (**volumetric light beam**) từ giếng trời chiếu lên tượng Phật Thích Ca Mâu Ni.
   - Hào quang đa tầng luân xa tỏa sáng rực rỡ sau lưng Đức Phật, ngọn nến và đèn dầu bập bùng chân thực, sóng nước lung linh nơi Hồ Liên Hoa.

2. **Phân loại danh xưng: Phật tử vs Lữ khách**:
   - **Phật tử** (đã ghi danh): Hiện huy hiệu vàng kim `☸️ Phật tử [Pháp danh/Họ tên]`, khoác Áo Lam truyền thống, cổ tay đeo chuỗi Tràng Hạt Trầm Hương 14 hạt, chắp tay búp sen.
   - **Lữ khách** (chưa ghi danh): Hiện huy hiệu thanh nhã `🕊️ Lữ khách #[Mã số]`, trang phục lữ hành mộc mạc. Bất cứ lúc nào cũng có thể nhấn *"Đăng ký Phật tử"* để nhận Thẻ Phật tử và chuyển đổi phục trang, danh hiệu tức thì.

3. **Hiện diện đa người dùng & Tự do di chuyển (Multiplayer Sangha)**:
   - Đồng bộ thời gian thực qua **Supabase Realtime**: người vào chùa từ các máy khác nhau thấy nhau di chuyển, quỳ/đứng, ngồi tọa cụ nào, kèm bảng tên 3D trên đầu. Sơ đồ 50 chỗ và hàng chờ tính theo người thật; người mẫu tự nhường tọa cụ khi cần.
   - Cấu hình: điền `SUPABASE_URL` và `SUPABASE_PUBLISHABLE_KEY` (khoá công khai, **không** dùng khoá secret/service_role) trong `index.html`. Không cần tạo bảng dữ liệu nào.
   - Khi chưa cấu hình hoặc Supabase không kết nối được, trang tự quay về `BroadcastChannel`: chỉ các tab trong cùng một trình duyệt thấy nhau.
   - Đạo tràng đồng tu luôn ấm cúng với các Phật tử và Lữ khách thập phương dạo bước sân chùa, ngắm hoa sen, thỉnh chuông.

4. **Chánh Điện 50 Chỗ Ngồi & Hàng Chờ Bên Ngoài**:
   - Bố trí chính xác **50 Tọa cụ Bồ Đoàn sen vàng** sắp xếp đối xứng trang nghiêm: **Tả Ban (25 chỗ)** và **Hữu Ban (25 chỗ)**, để trống lối đi đại lễ Tam Bảo ở chính giữa.
   - Phật tử và Lữ khách được sắp xếp an tọa cùng nhau thiền định, quỳ lễ hướng về tượng Phật.
   - **Giới hạn tối đa 50 chỗ**: Khi đủ 50 người, cửa Chánh Điện sẽ giữ lại và đưa người đến sau vào **Hàng chờ ngoài sân chùa**.
   - Người chờ có thể tự do đi dạo sân chùa, nghe chuông, thả hoa đăng. Ngay khi có người xuất điện ra sân, hệ thống sẽ tự động thỉnh chuông và mời người tiếp theo vào vị trí tọa cụ.
   - Bảng **"Sơ Đồ 50 Chỗ Ngồi & Hàng Chờ"** trực quan: xem ai đang ngồi ở tọa cụ nào, bấm vào chỗ trống để an tọa.

## Hướng dẫn sử dụng

- Mở trực tiếp file `index.html` trên trình duyệt (hoặc tải lên GitHub Pages / Hosting).
- Phím tắt: `W A S D` đi dạo · `F` tương tác · `C` quỳ/đứng · `E` xá lễ · `V` thu gọn bảng · `H` ẩn giao diện.
- Đăng ký Phật tử và dữ liệu chỉ lưu trên trình duyệt của người dùng, không gửi về máy chủ.

Xây dựng bằng Three.js, Tailwind CSS và Web Audio API — toàn bộ nằm gọn trong một file HTML.

