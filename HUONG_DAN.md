# HƯỚNG DẪN SỬ DỤNG & THÊM FONT CHỮ (FONTS) - HANDWRITING TOOL

## 1. Cách sử dụng font chữ
- Khi mở ứng dụng, bạn sẽ thấy danh sách tất cả các font chữ có sẵn, mỗi font đều có nhãn ngôn ngữ song ngữ (ví dụ: `[Vietnamese/Tiếng Việt] MJ-VIP-Daytonica-lytrx5.ttf`).
- Chọn font bạn muốn sử dụng từ combobox. Có thể nhập đoạn văn bản demo để xem preview trực tiếp.
- Nếu font không hỗ trợ ký tự bạn nhập, ứng dụng sẽ tự động chuyển sang font khác hoặc cảnh báo.

## 2. Cách thêm font mới vào ứng dụng
1. Xác định ngôn ngữ của font bạn muốn thêm (ví dụ: tiếng Việt, tiếng Anh, tiếng Nhật...).
2. Mở thư mục `fonts` trong thư mục ứng dụng.
   - Mỗi ngôn ngữ sẽ có một thư mục con, ví dụ:
     - `fonts/vietnamese/` (cho font tiếng Việt)
     - `fonts/english/` (cho font tiếng Anh)
     - `fonts/japanese/` (cho font tiếng Nhật)
     - ...
3. Copy file font (.ttf hoặc .otf) vào đúng thư mục ngôn ngữ tương ứng.
   - **Hoặc:** Kéo-thả file font trực tiếp vào cửa sổ ứng dụng, app sẽ tự động đưa font vào đúng thư mục.
4. Khởi động lại ứng dụng (hoặc nhấn nút reload fonts nếu có).
5. Font mới sẽ xuất hiện trong danh sách, kèm nhãn ngôn ngữ.

## 3. Lưu ý khi thêm font
- Nên dùng font Unicode đầy đủ để đảm bảo hiển thị đúng ký tự.
- Nếu font không hỗ trợ ngôn ngữ bạn cần, app sẽ cảnh báo hoặc bỏ qua font đó.
- Tên file font nên đặt rõ ràng, dễ nhận biết.

---

**Ví dụ:**
Bạn muốn thêm font tiếng Việt mới tên là `MyHandwriting.ttf`:
1. Copy file `MyHandwriting.ttf` vào thư mục `fonts/vietnamese/`.
2. Mở lại app, chọn `[Vietnamese/Tiếng Việt] MyHandwriting.ttf` trong danh sách font. 