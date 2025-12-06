# Copy Shared Drive Content to MyDrive

## English

## Description

This tool uses **Google Colab** resources to back up publicly downloadable files from a Google Drive Shared Folder into your personal MyDrive.

The tool works by:
- Utilizing free Google Colab resources (GPU/CPU and bandwidth)
- Copying the entire contents of a publicly shared folder into MyDrive
- Supporting the copying of very large folders without downloading to your local computer

## Requirements

- A Google account (to use Google Colab and Google Drive)
- The source folder must be shared publicly or you must have access to it
- The source folder must have a shortcut created in your MyDrive

## Usage Instructions

### Step 1: Insttall Colaboratory

1. Open this link with the Google account you want to use:  
   https://workspace.google.com/u/1/marketplace/app/colaboratory/1014160490159

2. Click **Install** (or **Open** if it’s already installed)  
   → Make sure you are logged in with the **correct Google account** (the one that owns the MyDrive where you will save the backup).

3. After installation finishes, a new tab will open with Google Colab ready to use.  
   (You can also access it anytime later via https://colab.research.google.com)

### Step 2: Create a Shortcut of the Folder in MyDrive

To allow the tool to access the shared folder, you need to add a shortcut of that folder to your MyDrive:

1. Open **Google Drive** in your browser
2. Locate the shared folder you want to back up
3. **Right-click** on the folder
4. Choose **"Organize"** → **"Add shortcut to Drive"**
5. Select the location for the shortcut (recommended: choose **"All locations"** and **MyDrive** for easy access)
6. Click **"Add"**

> **Note:** The shortcut folder will appear in MyDrive with the same name as the original folder. You will use this name in the next step.

### Step 3: Run the Notebook

1. Open the **`Copy_Shared_Drive_Content_to_MyDrive.ipynb`** file in Google Colab: 
   - Upload the file to Google Colab, or
   - Open it directly from Google Drive if it's already saved there 
     https://colab.research.google.com/drive/1ubaAiPUox_T6jny-R_-zcOn7g7adkuXu

2. Run the cells in order:
   - **Cell 1:** Mount Google Drive (authentication will be requested)
   - **Cell 2:** Check MyDrive access permissions
   - **Cell 3:** Enter the source folder name and destination folder name:
     - Enter the **source folder name** (the shortcut folder you created in Step 1)
     - Enter the **destination folder name** (the new backup folder that will be created)

3. Wait for the copy process to complete (may take from a few minutes to several hours depending on folder size)

## Important Notes

- ⚠️ If the destination folder already exists, it will be **deleted** before copying
- 📊 The tool will display file sizes after copying for verification
- ⏱️ Copy time depends on folder size and network speed
- 💾 Uses free Colab resources; runtime may be limited
- 🔒 Ensure the source folder is publicly accessible or you have view permissions

## Troubleshooting

If you encounter errors:
- **"Source directory does not exist"**: Double-check the shortcut folder name in MyDrive
- **"Permission denied"**: Make sure the folder is shared publicly or you have access
- **Timeout**: Try again or split the folder into smaller parts

## Support

If you experience issues, please check:
- The shortcut folder name is correct
- Source folder access permissions
- Network connection and Google Colab status




## Vietnamese

## Mô tả

Tool này sử dụng tài nguyên của **Google Colab** để backup các file được cho phép tải xuống công khai từ Google Drive Shared Folder vào thư mục MyDrive của bạn. 

Tool hoạt động bằng cách:
- Sử dụng tài nguyên miễn phí của Google Colab (GPU/CPU và băng thông)
- Copy toàn bộ nội dung từ folder được chia sẻ công khai vào MyDrive
- Hỗ trợ copy folder có kích thước lớn mà không cần tải về máy tính cá nhân

## Yêu cầu

- Tài khoản Google (để sử dụng Google Colab và Google Drive)
- Folder nguồn phải được chia sẻ công khai hoặc bạn có quyền truy cập
- Folder nguồn phải được tạo shortcut trong MyDrive của bạn

## Hướng dẫn sử dụng

### Bước 1: Cài đặt và mở Google Colaboratory

1. Mở link sau bằng chính tài khoản Google mà bạn muốn sử dụng:  
   https://workspace.google.com/u/1/marketplace/app/colaboratory/1014160490159

2. Nhấn nút **Cài đặt** (hoặc **Mở** nếu đã cài rồi)  
   → Đảm bảo bạn đang đăng nhập đúng tài khoản Google cần dùng.

3. Sau khi cài đặt xong, một tab mới sẽ tự động mở ra giao diện Google Colab sẵn sàng sử dụng.  
   (Sau này bạn cũng có thể mở lại bất kỳ lúc nào qua https://colab.research.google.com)

### Bước 2: Tạo Shortcut Folder về MyDrive

Để tool có thể truy cập folder được chia sẻ, bạn cần tạo shortcut của folder đó vào MyDrive:

1. Mở **Google Drive** trên trình duyệt
2. Tìm folder được chia sẻ mà bạn muốn backup
3. **Click chuột phải** vào folder
4. Chọn **"Organize"** → Sau đó chọn **"Add shortcut to Drive"** (Thêm lối tắt vào Drive)
5. Chọn vị trí lưu shortcut (khuyến nghị: chọn **"All locations"** và **MyDrive** để dễ tìm)
6. Click **"Add"** (Thêm lối tắt)

> **Lưu ý:** Folder shortcut sẽ xuất hiện trong MyDrive với tên giống như folder gốc. Bạn sẽ sử dụng tên này trong bước tiếp theo.

### Bước 3: Khởi chạy file Notebook

1. Mở file **`Copy_Shared_Drive_Content_to_MyDrive.ipynb`** trên Google Colab:
   - Upload file lên Google Colab, hoặc
   - Mở trực tiếp từ Google Drive nếu đã lưu ở đó 
    https://colab.research.google.com/drive/1ubaAiPUox_T6jny-R_-zcOn7g7adkuXu

2. Chạy các cell theo thứ tự:
   - **Cell 1:** Mount Google Drive (sẽ yêu cầu xác thực)
   - **Cell 2:** Kiểm tra quyền truy cập MyDrive
   - **Cell 3:** Nhập tên folder nguồn và folder đích:
     - Nhập **tên folder nguồn** (folder shortcut bạn đã tạo ở Bước 1)
     - Nhập **tên folder đích** (tên folder backup mới sẽ được tạo)

3. Đợi quá trình copy hoàn tất (có thể mất vài phút đến vài giờ tùy kích thước)


## Lưu ý quan trọng

- ⚠️ Folder đích nếu đã tồn tại sẽ **bị xóa** trước khi copy
- 📊 Tool sẽ hiển thị kích thước file sau khi copy để xác minh
- ⏱️ Thời gian copy phụ thuộc vào kích thước folder và tốc độ mạng
- 💾 Sử dụng tài nguyên Colab miễn phí, có thể bị giới hạn thời gian chạy
- 🔒 Đảm bảo folder nguồn có quyền truy cập công khai hoặc bạn có quyền xem

## Xử lý lỗi

Nếu gặp lỗi:
- **"Source directory does not exist"**: Kiểm tra lại tên folder shortcut trong MyDrive
- **"Permission denied"**: Đảm bảo folder được chia sẻ công khai hoặc bạn có quyền truy cập
- **Timeout**: Thử lại hoặc chia nhỏ folder thành các phần nhỏ hơn

## Hỗ trợ

Nếu gặp vấn đề, vui lòng kiểm tra:
- Tên folder shortcut có đúng không
- Quyền truy cập folder nguồn
- Kết nối mạng và trạng thái Google Colab

