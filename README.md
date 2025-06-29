# 🖋️ Handwriting Tool - Công cụ chuyển đổi văn bản thành chữ viết tay

[![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Version](https://img.shields.io/badge/Version-2.0-orange.svg)]()

> **Công cụ AI chuyển đổi văn bản thành chữ viết tay tự nhiên với nhiều font đa ngôn ngữ**

## ✨ **Tính năng nổi bật**

### 🎨 **Hiệu ứng chữ viết tay tự nhiên**
- **Rung tay tự nhiên**: Mô phỏng chuyển động tay khi viết
- **Biến thể kích thước**: Font size thay đổi ngẫu nhiên ±3px
- **Hiệu ứng mực**: Đậm nhạt và nét bút đứt đoạn
- **Nghiêng dòng**: Góc nghiêng tự nhiên ±3 độ
- **Khoảng cách ngẫu nhiên**: Giữa các ký tự và từ

### 🌍 **Hỗ trợ đa ngôn ngữ**
- **Tiếng Việt**: 5 font thư pháp đẹp
- **Tiếng Anh**: 4 font handwriting
- **Tiếng Nhật**: 2 font Kanji
- **Tiếng Trung**: Font Source Han Sans
- **Tiếng Nga**: Font Balmoral
- **Tiếng Ả Rập**: Font Saudi Arabia
- **Và 30+ ngôn ngữ khác** với font dự phòng

### 📄 **Kiểu giấy đa dạng**
- **Kẻ ngang**: Giấy vở học sinh
- **4 ô ly**: Giấy vở Việt Nam
- **Ô vuông**: Giấy caro
- **Chấm bi**: Giấy kẻ chấm
- **Trắng**: Giấy trắng
- **Giấy thi**: Giấy thi chuyên nghiệp
- **Thư pháp**: Giấy thư pháp
- **Parchment**: Giấy cổ

### 🎛️ **Tùy chỉnh nâng cao**
- **Kích thước chữ**: 16-48px
- **Khoảng cách dòng**: 1.0-3.0
- **Lề giấy**: 20-100px
- **Màu mực**: Tùy chọn màu sắc
- **Kích thước giấy**: A4, A5, Custom
- **Xuất đen trắng**: Giống scan

### 💾 **Hệ thống Template**
- **Lưu cài đặt**: Lưu các preset yêu thích
- **Tải template**: Tái sử dụng cài đặt
- **Quản lý**: Xóa, đổi tên template
- **Tự động**: Lưu ngày tạo

### 🌙 **Dark Mode**
- **Giao diện tối**: Bảo vệ mắt
- **Chuyển đổi mượt**: Light/Dark toggle
- **Tùy chỉnh**: Màu sắc tự động

### 📤 **Xuất file đa định dạng**
- **PNG**: Chất lượng cao
- **PDF**: Vector, có thể in
- **Word**: Chỉnh sửa được
- **SVG**: Vector chất lượng cao

## 🚀 **Cài đặt và sử dụng**

### **Yêu cầu hệ thống**
- Python 3.7+
- Windows 10/11 (đã test)
- RAM: 2GB+
- Dung lượng: 50MB

### **Cài đặt nhanh**
```bash
# Clone repository
git clone https://github.com/fishx2/Handwriting-Tool.git
cd Handwriting-Tool

# Cài đặt dependencies
pip install -r requirements.txt

# Chạy ứng dụng
python handwriting_gui.py
```

### **Hoặc chạy file .bat**
```bash
# Chạy trực tiếp
run.bat
```

## 📖 **Hướng dẫn sử dụng**

### **Bước 1: Nhập văn bản**
- Nhập văn bản vào ô "Văn bản đầu vào"
- Hỗ trợ copy/paste từ file
- Đếm ký tự tự động

### **Bước 2: Tùy chỉnh**
- **Chọn font**: Font phù hợp với ngôn ngữ
- **Kích thước**: Điều chỉnh size chữ
- **Màu mực**: Chọn màu yêu thích
- **Kiểu giấy**: Chọn loại giấy phù hợp

### **Bước 3: Tạo chữ viết tay**
- Nhấn "Tạo chữ viết tay"
- Xem preview real-time
- Zoom in/out để kiểm tra

### **Bước 4: Xuất file**
- **PNG**: Chất lượng cao, phù hợp web
- **PDF**: Vector, in ấn chuyên nghiệp
- **Word**: Chỉnh sửa thêm nội dung
- **SVG**: Vector, scale không giới hạn

## 🎯 **Tính năng nâng cao**

### **Template System**
```python
# Lưu template
1. Tùy chỉnh cài đặt
2. Nhấn "Lưu Template"
3. Đặt tên và mô tả
4. Template được lưu tự động

# Tải template
1. Chọn template từ danh sách
2. Nhấn "Tải Template"
3. Cài đặt được áp dụng ngay
```

### **Dark Mode**
```python
# Bật/tắt Dark Mode
1. Tích vào "🌙 Dark Mode"
2. Giao diện chuyển đổi tự động
3. Bảo vệ mắt khi làm việc lâu
```

### **Keyboard Shortcuts**
- **Preview**: Mũi tên để di chuyển
- **Home/End**: Về đầu/cuối
- **Mouse**: Kéo để pan
- **Wheel**: Zoom in/out

## 📁 **Cấu trúc dự án**

```
Handwriting-Tool/
├── fonts/                 # Thư mục font đa ngôn ngữ
│   ├── vietnamese/       # Font tiếng Việt
│   ├── english/          # Font tiếng Anh
│   ├── japanese/         # Font tiếng Nhật
│   └── ...               # 30+ ngôn ngữ khác
├── output/               # Thư mục xuất file
├── handwriting_gui.py    # File chính
├── requirements.txt      # Dependencies
├── run.bat              # Script chạy nhanh
├── README.md            # Hướng dẫn này
└── templates.json       # File lưu template
```

## 🔧 **Tùy chỉnh nâng cao**

### **Thêm font mới**
1. Copy file font (.ttf/.otf) vào thư mục `fonts/[ngôn_ngữ]/`
2. Khởi động lại ứng dụng
3. Font sẽ xuất hiện trong danh sách

### **Tùy chỉnh màu sắc**
```python
# Trong file handwriting_gui.py
self.ink_color = (25, 25, 112)  # Màu mặc định
# Thay đổi RGB values để tùy chỉnh
```

### **Thêm kiểu giấy mới**
```python
# Thêm vào hàm create_paper_texture()
elif paper_style == "your_style":
    # Code tạo texture mới
```

## 🐛 **Xử lý lỗi thường gặp**

### **Lỗi font không hiển thị**
- Kiểm tra file font có đúng định dạng (.ttf/.otf)
- Đảm bảo font hỗ trợ ký tự cần thiết
- Thử font khác trong cùng ngôn ngữ

### **Lỗi xuất file**
- Kiểm tra quyền ghi thư mục output
- Đảm bảo đủ dung lượng ổ cứng
- Thử xuất định dạng khác

### **Lỗi giao diện**
- Cập nhật Python lên phiên bản mới
- Cài đặt lại tkinter: `pip install tk`
- Kiểm tra độ phân giải màn hình

## 🤝 **Đóng góp**

Chúng tôi rất hoan nghênh mọi đóng góp! Hãy:

1. **Fork** repository
2. Tạo **branch** mới (`git checkout -b feature/AmazingFeature`)
3. **Commit** thay đổi (`git commit -m 'Add some AmazingFeature'`)
4. **Push** lên branch (`git push origin feature/AmazingFeature`)
5. Tạo **Pull Request**

### **Cách đóng góp**
- 🐛 **Báo lỗi**: Tạo Issue với mô tả chi tiết
- 💡 **Đề xuất tính năng**: Thảo luận trong Discussions
- 📝 **Cải thiện docs**: Chỉnh sửa README
- 🔧 **Sửa code**: Pull Request

## 📄 **License**

Dự án này được phân phối dưới giấy phép MIT. Xem file `LICENSE` để biết thêm chi tiết.

## 🙏 **Lời cảm ơn**

- **Font creators**: Cảm ơn các tác giả font đã chia sẻ
- **Python community**: Tkinter, PIL, reportlab
- **Contributors**: Tất cả người đóng góp
- **Users**: Cảm ơn mọi người đã sử dụng và phản hồi

## 📞 **Liên hệ**

- **GitHub**: [@fishx2](https://github.com/fishx2)
- **Email**: [your-email@example.com]
- **Issues**: [GitHub Issues](https://github.com/fishx2/Handwriting-Tool/issues)

---

⭐ **Nếu dự án này hữu ích, hãy cho chúng tôi một star!** ⭐