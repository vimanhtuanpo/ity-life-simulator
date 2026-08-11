# City Life Simulator - REALISTIC GAMEPLAY FIXED V3

Godot 4.x project, cleaned and packaged with the included human, sedan and building GLB assets.

## Chạy
1. Giải nén ZIP.
2. Mở thư mục bằng Godot 4.x.
3. Mở `project.godot`.
4. Bấm Run.

## Điều khiển
- W A S D: di chuyển
- Chuột: xoay camera
- TAB: mở/đóng bảng quản lý
- ESC: đóng bảng quản lý / ẩn-hiện khóa chuột
- E: tương tác với điểm gần nhất

## Đã sửa trong V3
- Sửa lỗi type inference/parser trong `_load_model()`.
- Người được đặt đúng tỉ lệ và chân bám mặt đất/via hè.
- Xe được hạ đúng vị trí bánh xe, không còn bay.
- Xe dùng `CharacterBody3D + move_and_slide()` để collision với người/xe/công trình.
- NPC có collision và đi theo tuyến via hè, không đi xuyên nhà.
- A/D là di chuyển ngang; không tự xoay camera.
- Camera xoay bằng chuột.
- TAB/ESC đóng mở bảng quản lý.
- Đồng hồ mô phỏng chậm lại: 1 ngày trong game mất khoảng 5 giờ thực thay vì chạy quá nhanh.
- Công trình có tiến độ và hiện tượng thi công.
- Thêm cần/cột cầu thấp, cửa Khu nhà ở A và điểm tương tác E.
- Thêm collision của đường, via hè, nhà, người và xe.
- Không dùng asset tải ngoài; các GLB đã nằm trong `assets/`.

## Lưu ý về "thực tế"
Bộ GLB đi kèm là model game medium-detail, không phải photogrammetry/AAA photorealistic. Bản V3 tập trung vào tỉ lệ, vật lý, collision, giao thông, NPC và gameplay để tránh lỗi bay/xuyên. Nếu muốn đạt mức photorealistic như game AAA, cần thay asset bằng model PBR chi tiết hơn và thêm texture/animation mộc nhất.