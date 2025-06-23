# 🖋️ Handwriting Generator GUI - Hướng dẫn cài đặt & Tính năng mới

## 📦 Dependencies cần thiết

Tạo file `requirements.txt`:

```txt
Pillow==10.0.1
numpy==1.24.3
requests==2.31.0
reportlab==4.0.4
python-docx==0.8.11
```

## 🚀 Cài đặt

### Bước 1: Cài đặt Python packages
```bash
pip install -r requirements.txt
```

### Bước 2: Cấu trúc thư mục
```
Handwriting Tool/
├── handwriting_gui.py          # File GUI chính
├── requirements.txt            # Dependencies
├── fonts/                      # Thư mục fonts (tổ chức theo ngôn ngữ)
│   ├── english/                # Font tiếng Anh
│   ├── vietnamese/             # Font tiếng Việt
│   ├── japanese/               # Font tiếng Nhật
│   └── ...                     # Các ngôn ngữ khác
├── output/                     # Thư mục output (tùy chọn)
└── handwriting_settings.json   # File cài đặt (tự động tạo)
```

### Bước 3: Thêm font mới
- Mỗi ngôn ngữ có thư mục riêng trong `fonts/`.
- Để thêm font, chỉ cần copy file `.ttf` hoặc `.otf` vào đúng thư mục ngôn ngữ.
- Ứng dụng sẽ tự động nhận diện và hiển thị tất cả font, kèm nhãn ngôn ngữ song ngữ (ví dụ: `[Vietnamese/Tiếng Việt] MJ-VIP-Daytonica-lytrx5.ttf`).
- Có thể kéo-thả file font trực tiếp vào cửa sổ ứng dụng.

### Bước 4: Chạy ứng dụng
```bash
python handwriting_gui.py
```

## ✨ Tính năng chính

### 🌍 Quản lý font đa ngôn ngữ & giao diện chọn font mới
- **Tự động quét và hiển thị tất cả font của mọi ngôn ngữ**
- **Nhãn song ngữ cho từng font**: Dễ dàng nhận biết, phù hợp cả người Việt và quốc tế
- **Preview trực tiếp**: Nhập text demo để xem trước font
- **Hướng dẫn thêm font rõ ràng**: Nếu chưa có font, app sẽ hướng dẫn cách thêm
- **Chọn font không cần chọn ngôn ngữ**: Tất cả font đều hiển thị, dễ tìm kiếm

### 🎨 Giao diện thân thiện
- **Text Area không giới hạn**: Nhập văn bản dài tùy ý
- **Live Preview**: Xem trước kết quả ngay lập tức
- **Settings Panel**: Tùy chỉnh đầy đủ các thông số

### ⚙️ Tùy chỉnh nâng cao
- **Font Size**: 16-48px với slider
- **Line Spacing**: 1.0-3.0x với điều chỉnh mịn
- **Margin**: 20-100px
- **Ink Color**: Color picker đầy đủ
- **Paper Style**: Lined/Blank/Grid

### 📤 Xuất đa định dạng
- **PNG**: Hình ảnh chất lượng cao
- **PDF**: Tự động scale fit A4, professional layout
- **Word**: Tương thích Microsoft Word (.docx)

### 💾 Quản lý cài đặt
- **Auto Save**: Lưu cài đặt tự động
- **Load Settings**: Khôi phục cài đặt trước đó
- **Import Text**: Mở file .txt trực tiếp

## 🎯 Cách sử dụng

### 1. Nhập văn bản & chọn font
- Nhập văn bản vào text area
- Chọn font từ combobox, mỗi font đều có nhãn ngôn ngữ song ngữ
- Có thể nhập text demo để xem preview trực tiếp
- Nếu muốn thêm font, chỉ cần copy/kéo-thả vào đúng thư mục ngôn ngữ

### 2. Tùy chỉnh
- Điều chỉnh các slider cho font size, spacing, margin
- Chọn màu mực với color picker
- Chọn kiểu giấy phù hợp

### 3. Tạo và xuất
- Click "🎨 Tạo chữ viết tay" 
- Xem preview bên phải
- Chọn định dạng xuất: PNG/PDF/Word

## 🔧 Tính năng kỹ thuật

### Unicode & Font Fallback thông minh
- **Tự động kiểm tra font**: Nếu font không hỗ trợ ký tự, sẽ tự động bỏ qua hoặc cảnh báo
- **Hỗ trợ nhiều hệ chữ**: Latin, Việt, Trung, Nhật, Ấn Độ, Ả Rập, ...

### Natural Handwriting Simulation
- **Character Variations**: Mỗi ký tự có vị trí và góc xoay ngẫu nhiên
- **Word Spacing**: Khoảng cách từ tự nhiên
- **Line Slant**: Độ nghiêng dòng realistic
- **Ink Effects**: Hiệu ứng mực thấm và texture

### Smart Text Processing
- **Auto Line Breaking**: Tự động xuống dòng thông minh
- **Paragraph Handling**: Xử lý đoạn văn đúng cách
- **Unicode Support**: Hỗ trợ đầy đủ ký tự tiếng Việt

### Performance Optimization
- **Threading**: Xử lý không block UI
- **Memory Management**: Tối ưu memory cho text dài
- **Font Caching**: Cache fonts để tăng tốc

## 📋 Troubleshooting

### Lỗi thường gặp

**1. Lỗi import modules:**
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

**2. Lỗi font không load:**
- Kiểm tra kết nối internet
- Fonts sẽ tự động download lần đầu

**3. Lỗi xuất PDF:**
```bash
pip install --upgrade reportlab
```

**4. Lỗi xuất Word:**
```bash
pip install --upgrade python-docx
```

### Performance Tips

**Cho văn bản dài (>5000 ký tự):**
- Giảm font size xuống 20-24px
- Tăng margin để giảm canvas size
- Chia nhỏ thành nhiều phần

**Cho chất lượng cao:**
- Dùng font size 32-40px
- Paper style "blank" để tối ưu
- Xuất PNG rồi convert sang định dạng khác

### Lỗi font không hiển thị đúng ký tự:
- Đảm bảo font bạn thêm vào hỗ trợ đủ ký tự cho ngôn ngữ mong muốn
- Ưu tiên dùng font Unicode đầy đủ (ví dụ: Source Han Sans, Noto, v.v.)
- Nếu font bị lỗi, app sẽ cảnh báo và hướng dẫn cách sửa

## 🎨 Customization

### Thêm fonts mới cho từng ngôn ngữ
- Copy file font vào đúng thư mục con trong `fonts/` (ví dụ: `fonts/vietnamese/`)
- App sẽ tự động nhận diện và hiển thị

### Thay đổi màu giấy mặc định
```python
# Trong create_paper_texture()
paper = Image.new('RGB', (width, height), color=(255, 255, 255))  # Trắng tinh
```

### Tùy chỉnh ink effects
```python
# Trong add_ink_effects()
noise = np.random.normal(0, 8, img_array.shape)  # Tăng noise
result = result.filter(ImageFilter.GaussianBlur(radius=0.5))  # Tăng blur
```

## 📸 Screenshots

```
┌─────────────────────────────────────────────────────────────┐
│ 🖋️ Handwriting Generator                                    │
├─────────────┬─────────────────────────┬─────────────────────┤
│ ⚙️ Cài đặt   │ ✍️ Văn bản đầu vào        │ 👁️ Xem trước        │
│             │                         │                     │
│ Font: 28    │ Nhập text của bạn...    │ [Preview Image]     │
│ Spacing:1.5 │                         │                     │
│ Margin: 50  │                         │                     │
│ Color: 🔵   │                         │                     │
│ Paper:Lined │                         │                     │
│             │                         │                     │
│ 🎨 Tạo      │                         │                     │
│ 💾 Lưu      │                         │                     │
│ 📁 Mở       │                         │                     │
│             │                         │                     │
│ 📤 Xuất:    │                         │                     │
│ 💾 PNG      │                         │                     │
│ 📄 PDF      │                         │                     │
│ 📝 Word     │                         │                     │
└─────────────┴─────────────────────────┴─────────────────────┘
```

## 🌟 Advanced Features

### Batch Processing
```python
# Trong tương lai có thể thêm:
def batch_process_files(self, file_list):
    for file_path in file_list:
        # Process each file
        pass
```

### Template System
```python
# Templates cho các loại giấy
templates = {
    'homework': {'margin': 80, 'line_spacing': 2.0},
    'letter': {'margin': 60, 'line_spacing': 1.8},
    'note': {'margin': 40, 'line_spacing': 1.5}
}
```

## 📞 Support

Nếu gặp vấn đề:
1. Kiểm tra Python version >= 3.8
2. Cài đặt lại dependencies
3. Kiểm tra quyền ghi file trong thư mục
4. Đảm bảo có kết nối internet cho lần đầu chạy