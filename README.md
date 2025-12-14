# Copy Shared Drive Content to MyDrive

## English

## Description

This tool uses **Google Colab** resources to copy files from a Google Drive Shared Folder (via link) into your personal MyDrive folder.

The tool works by:
- Utilizing free Google Colab resources (GPU/CPU and bandwidth)
- Copying the entire contents of a shared folder directly from a Google Drive link into MyDrive
- Supporting the copying of very large folders without downloading to your local computer
- Using Google Drive API to copy folders and files directly (no need to create shortcuts)

## Requirements

- A Google account (to use Google Colab and Google Drive)
- The source folder must be shared publicly or you must have access to it
- **No need to create shortcuts** - just provide the Google Drive folder link

## Usage Instructions

### Step 1: Install Google Colaboratory

1. Open this link with the Google account you want to use:  
   https://workspace.google.com/u/1/marketplace/app/colaboratory/1014160490159

2. Click **Install** (or **Open** if it's already installed)  
   → Make sure you are logged in with the **correct Google account** (the one that owns the MyDrive where you will save the backup).

3. After installation finishes, a new tab will open with Google Colab ready to use.  
   (You can also access it anytime later via https://colab.research.google.com)

### Step 2: Run the Notebook

1. Open the **`Copy_Shared_Drive_Content_to_MyDrive.ipynb`** file in Google Colab: 
   - Upload the file to Google Colab, or https://colab.research.google.com/drive/1ubaAiPUox_T6jny-R_-zcOn7g7adkuXu
   - Open it directly from Google Drive if it's already saved there

2. Run the cells in order:
   - **Cell 1:** Mount Google Drive (authentication will be requested)
   - **Cell 2:** (Optional) Verify MyDrive access by listing contents
   - **Cell 3:** Install required libraries (Google Drive API)
   - **Cell 4:** Copy folder from Google Drive link:
     - Enter the **Google Drive folder link (URL)** - e.g., `https://drive.google.com/drive/folders/1ABC123xyz...`
     - Enter the **destination folder name** (the new backup folder that will be created in your MyDrive)

3. Wait for the copy process to complete (may take from a few minutes to several hours depending on folder size)

### How to Get the Google Drive Folder Link

1. Open **Google Drive** in your browser
2. Navigate to the shared folder you want to copy
3. **Right-click** on the folder
4. Select **"Get link"** or **"Share"**
5. Copy the link (it should look like: `https://drive.google.com/drive/folders/1ABC123xyz...`)
6. Make sure the folder has **"Anyone with the link"** or you have access permissions

> **Note:** The tool will automatically extract the folder ID from the link. You can paste the full URL or just the folder ID.

## Important Notes

- ⚠️ The destination folder will be created in your MyDrive root directory
- 📊 The tool will display the source folder name and copy progress
- ⏱️ Copy time depends on folder size and network speed
- 💾 Uses free Colab resources; runtime may be limited
- 🔒 Ensure the source folder is publicly accessible or you have view permissions
- 🔄 The tool recursively copies all subfolders and files
- ✅ No need to create shortcuts - just provide the link!

## Troubleshooting

If you encounter errors:
- **"Could not extract folder ID from URL"**: Check that the link is a valid Google Drive folder link
- **"Permission denied"** or **"File not found"**: Make sure the folder is shared publicly or you have access permissions
- **"Error getting folder name"**: Verify that you have view access to the source folder
- **Timeout**: Try again or split the folder into smaller parts
- **Authentication errors**: Make sure you're logged in with the correct Google account

## Support

If you experience issues, please check:
- The Google Drive folder link is correct and accessible
- Source folder access permissions (should be "Anyone with the link" or you have access)
- Network connection and Google Colab status
- You're using the correct Google account

---

## Tiếng Việt

## Mô tả

Tool này sử dụng tài nguyên của **Google Colab** để copy các file từ Google Drive Shared Folder (qua link) vào thư mục MyDrive của bạn.

Tool hoạt động bằng cách:
- Sử dụng tài nguyên miễn phí của Google Colab (GPU/CPU và băng thông)
- Copy toàn bộ nội dung từ folder được chia sẻ trực tiếp từ link Google Drive vào MyDrive
- Hỗ trợ copy folder có kích thước lớn mà không cần tải về máy tính cá nhân
- Sử dụng Google Drive API để copy folder và file trực tiếp (không cần tạo shortcut)

## Yêu cầu

- Tài khoản Google (để sử dụng Google Colab và Google Drive)
- Folder nguồn phải được chia sẻ công khai hoặc bạn có quyền truy cập
- **Không cần tạo shortcut** - chỉ cần cung cấp link Google Drive folder

## Hướng dẫn sử dụng

### Bước 1: Cài đặt Google Colaboratory

1. Mở link sau bằng chính tài khoản Google mà bạn muốn sử dụng:  
   https://workspace.google.com/u/1/marketplace/app/colaboratory/1014160490159

2. Nhấn nút **Cài đặt** (hoặc **Mở** nếu đã cài rồi)  
   → Đảm bảo bạn đang đăng nhập đúng tài khoản Google cần dùng.

3. Sau khi cài đặt xong, một tab mới sẽ tự động mở ra giao diện Google Colab sẵn sàng sử dụng.  
   (Sau này bạn cũng có thể mở lại bất kỳ lúc nào qua https://colab.research.google.com)

### Bước 2: Khởi chạy file Notebook

1. Mở file **`Copy_Shared_Drive_Content_to_MyDrive.ipynb`** trên Google Colab:
   - Upload file lên Google Colab, hoặc https://colab.research.google.com/drive/1ubaAiPUox_T6jny-R_-zcOn7g7adkuXu
   - Mở trực tiếp từ Google Drive nếu đã lưu ở đó

2. Chạy các cell theo thứ tự:
   - **Cell 1:** Mount Google Drive (sẽ yêu cầu xác thực)
   - **Cell 2:** (Tùy chọn) Kiểm tra quyền truy cập MyDrive bằng cách liệt kê nội dung
   - **Cell 3:** Cài đặt thư viện cần thiết (Google Drive API)
   - **Cell 4:** Copy folder từ link Google Drive:
     - Nhập **link Google Drive folder (URL)** - ví dụ: `https://drive.google.com/drive/folders/1ABC123xyz...`
     - Nhập **tên folder đích** (tên folder backup mới sẽ được tạo trong MyDrive của bạn)

3. Đợi quá trình copy hoàn tất (có thể mất vài phút đến vài giờ tùy kích thước)

### Cách lấy link Google Drive Folder

1. Mở **Google Drive** trên trình duyệt
2. Điều hướng đến folder được chia sẻ mà bạn muốn copy
3. **Click chuột phải** vào folder
4. Chọn **"Lấy liên kết"** hoặc **"Chia sẻ"**
5. Sao chép link (link sẽ có dạng: `https://drive.google.com/drive/folders/1ABC123xyz...`)
6. Đảm bảo folder có quyền **"Bất kỳ ai có liên kết"** hoặc bạn có quyền truy cập

> **Lưu ý:** Tool sẽ tự động trích xuất folder ID từ link. Bạn có thể dán toàn bộ URL hoặc chỉ folder ID.

## Lưu ý quan trọng

- ⚠️ Folder đích sẽ được tạo trong thư mục gốc MyDrive của bạn
- 📊 Tool sẽ hiển thị tên folder nguồn và tiến trình copy
- ⏱️ Thời gian copy phụ thuộc vào kích thước folder và tốc độ mạng
- 💾 Sử dụng tài nguyên Colab miễn phí, có thể bị giới hạn thời gian chạy
- 🔒 Đảm bảo folder nguồn có quyền truy cập công khai hoặc bạn có quyền xem
- 🔄 Tool sẽ copy đệ quy tất cả subfolder và file
- ✅ Không cần tạo shortcut - chỉ cần cung cấp link!

## Xử lý lỗi

Nếu gặp lỗi:
- **"Could not extract folder ID from URL"**: Kiểm tra xem link có phải là link Google Drive folder hợp lệ không
- **"Permission denied"** hoặc **"File not found"**: Đảm bảo folder được chia sẻ công khai hoặc bạn có quyền truy cập
- **"Error getting folder name"**: Xác minh rằng bạn có quyền xem folder nguồn
- **Timeout**: Thử lại hoặc chia nhỏ folder thành các phần nhỏ hơn
- **Lỗi xác thực**: Đảm bảo bạn đang đăng nhập đúng tài khoản Google

## Hỗ trợ

Nếu gặp vấn đề, vui lòng kiểm tra:
- Link Google Drive folder có đúng và có thể truy cập được không
- Quyền truy cập folder nguồn (nên là "Bất kỳ ai có liên kết" hoặc bạn có quyền truy cập)
- Kết nối mạng và trạng thái Google Colab
- Bạn đang sử dụng đúng tài khoản Google

