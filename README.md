# Path of Exile Leveling Guide Plugin (ExileAPI)
<br>

<div align="center">
  <img src="https://i.imgur.com/rB0rY6e.png" alt="Leveling Guide Preview" width="600"/>
</div>

<p align="center">
  [ <b><a href="#english">English</a></b> | <b><a href="#tiếng-việt">Tiếng Việt</a></b> ]
</p>

---

<br>

<h2 id="english">🇬🇧 English</h2>

A lightweight, multi-language (English/Vietnamese) leveling assistant plugin for Path of Exile, designed specifically for **ExileAPI**. It displays a transparent overlay with step-by-step leveling tasks, zone info, recommended levels, and automated passive tree switching.

### ✨ Features
- **Multi-Language Support**: Swap between English and Vietnamese on the fly straight from the UI. All interface texts and guide contents are fully translated.
- **Dynamic Build Switching**: Manage multiple `.json` build files effortlessly. Drop your new builds into the `config/builds/` folder, and they will automatically populate the in-game dropdown menu.
- **Gem Highlighting**: Highlights required gems for your build directly in the NPC Vendor window.
- **Zone Awareness**: Automatically updates tasks when you enter a new zone, showing your current objective, area name, and level recommendations.
- **Collapsible UI**: Easily collapse the guide into a minimal UI arrow if you just want it out of the way.

### 📥 Installation
1. Ensure you have a working version of **ExileAPI**.
2. Download or clone this repository into your ExileAPI plugins folder. The path should look like this:
   `ExileApi/Plugins/Compiled/LevelingGuide`
3. Launch Path of Exile, then launch ExileAPI.
4. Open the ExileAPI menu (usually `F2`) and enable **LevelingGuide** in the **Core** plugins list.

### ⚙️ How to Add Custom Builds
The plugin comes with a default `Absolution_Guardian` build. To add your own:
1. Navigate to: `ExileApi/Plugins/Compiled/LevelingGuide/config/builds/`
2. Create or drop your build files there.
   - For a universal file: `MyBuild.json`
   - For language-specific files: `MyBuild_en.json` and `MyBuild_vn.json`
3. The plugin will automatically detect these files and list `MyBuild` in the settings dropdown.

### 📘 How to Use
- **Toggle Overlay**: Open Settings (F2) -> LevelingGuide -> check `Enable` and `Show Overlay`.
- **Change Language**: In the plugin settings, change `Language` to **en** or **vn**.
- **Pick a Build**: Use the `Selected Build` dropdown in settings to pick your active build.

### ⚠️ How to Fix Missing/Square Vietnamese Text (Font Issue)
If you switch to Vietnamese (`vn`) but see squares or question marks (`?`) instead of text, it's because your **ExileAPI Core** is not using a unicode-supported font.

**Fix 1: Via ExileAPI Menu**
1. Open ExileAPI menu (`F2`).
2. Go to `Core` -> `ThemeEditor` (or Font Settings).
3. Change the `Font` path to a standard font like Arial. E.g.: `C:\Windows\Fonts\arial.ttf`
4. Restart ExileAPI.

**Fix 2: Via Config File**
1. Go to your ExileAPI folder -> `config` folder.
2. Open `settings.json` or `CoreSettings.json` with a text editor.
3. Find `"FontPath"` and change it to `"C:\\Windows\\Fonts\\arial.ttf"`.
4. Save the file and restart ExileAPI.

<br>

---

<br>

<h2 id="tiếng-việt">🇻🇳 Tiếng Việt</h2>

Plugin hỗ trợ leveling (cày cấp) gọn nhẹ đa ngôn ngữ (Tiếng Anh/Tiếng Việt) dành riêng cho **ExileAPI** trong Path of Exile. Nó hiển thị một bảng trong suốt trên màn hình chứa các nhiệm vụ từng bước, thông tin khu vực, level đề xuất, và tự động chuyển đổi bảng Passive Tree.

### ✨ Tính Năng Nổi Bật
- **Hỗ trợ Đa Ngôn Ngữ**: Thay đổi giữa Tiếng Anh và Tiếng Việt ngay lập tức trong Menu. Toàn bộ chữ trên GUI và nội dung đều được dịch mượt mà.
- **Chuyển Đổi Build Nhanh Chóng**: Quản lý nhiều file build `.json` khác nhau. Dễ dàng thả file build mới của bạn vào folder `config/builds/`, plugin sẽ tự động cập nhật danh sách chọn lựa.
- **Highlight Gem (Kỹ Năng)**: Đánh dấu các gem cần thiết trong quá trình leveling khi bạn mở cửa sổ mua bán với NPC.
- **Nhận Diện Zone Tương Thích**: Tự động chuyển đổi nhiệm vụ khi bạn qua Map/Zone mới, hiển thị gợi ý cấp độ và cảnh báo nếu level của bạn quá thấp.
- **Giao Diện Thu Gọn**: Nhấn nút mũi tên trên GUI để thu gọn bảng nhiệm vụ lại cho đỡ tốn diện tích màn hình.

### 📥 Cài Đặt
1. Đảm bảo bạn đang sử dụng **ExileAPI** đang hoạt động bình thường.
2. Tải về hoặc clone kho lưu trữ này vào thư mục plugins của ExileAPI. Đường dẫn chuẩn sẽ trông như sau:
   `ExileApi/Plugins/Compiled/LevelingGuide`
3. Mở game Path of Exile, sau đó chạy ứng dụng ExileAPI.
4. Bật menu chuột của ExileAPI (thường là phím `F2`), chọn **LevelingGuide** trong danh sách plugin và tích bật nó lên.

### ⚙️ Thêm Build Theo Sở Thích Cá Nhân
Plugin có sẵn một build mẫu `Absolution_Guardian`. Để thêm build của bạn:
1. Vào thư mục: `ExileApi/Plugins/Compiled/LevelingGuide/config/builds/`
2. Tạo hoặc chép file gốc của bạn vào đây.
   - Nếu chung 1 ngôn ngữ hãy đặt tên: `BuildCuaToi.json`
   - Nếu bạn muốn hỗ trợ tiếng anh/tiếng việt riêng biệt: phân loại bằng hậu tố `BuildCuaToi_en.json` và `BuildCuaToi_vn.json`.
3. Plugin sẽ tự tìm kiếm và hiển thị `BuildCuaToi` trong menu chọn build.

### 📘 Hướng Dẫn Sử Dụng
- **Bật bảng hướng dẫn**: Mở Setting (F2) -> LevelingGuide -> Bật `Enable` và `Show Overlay`.
- **Đổi ngôn ngữ**: Chỉnh `Language` thành **vn** hoặc **en** tuỳ thích.
- **Chọn Build**: Dùng menu thả xuống ở mục `Selected Build` để tìm và kích hoạt build.

### ⚠️ Lỗi Hiển Thị Font Chữ Tiếng Việt (Hình Vuông, Dấu Chấm Hỏi)
Lý do bị lỗi chữ hình vuông là do **bản ExileAPI gốc chưa được cài đặt font hỗ trợ tiếng Việt**. Plugin chỉ mượn thư viện chữ của ExileAPI để vẽ, chứ không tự có font riêng. Hãy làm theo cách sau để sửa lỗi vĩnh viễn:

**Cách 1: Sửa qua Menu ExileAPI**
1. Vào game và mở menu ExileAPI (`F2`).
2. Vào tab `Core` -> Chọn `ThemeEditor`.
3. Tìm vùng cấu hình đường dẫn **Font** và sửa lại thành một font chuẩn có tiếng Việt (Ví dụ: `C:\Windows\Fonts\arial.ttf` hoặc `.tahoma.ttf`).
4. Tắt đi bật lại ExileAPI.

**Cách 2: Sửa bằng file config**
1. Mở thư mục chứa ExileAPI gốc, vào folder `config`.
2. Mở file `settings.json` (hoặc `CoreSettings.json`) bằng Notepad.
3. Tìm đến dòng có chứa chữ `"FontPath"`. Sửa đường dẫn bên cạnh thành một font hỗ trợ unicode. VD: `"FontPath": "C:\\Windows\\Fonts\\arial.ttf"`.
4. Lưu file và khởi động lại ExileAPI. 

<br>

*Designed and updated to streamline your Path of Exile campaign progression.*
