<div align="center">
  <img src="assets/logo.svg" width="72" height="72" alt="Agy Powertools Logo" />
  <h1>Agy Powertools (Bản Việt hóa)</h1>
  <p><strong>Plugin mở rộng giao diện nguyên bản cho Antigravity 2.0 - Hỗ trợ đầy đủ Tiếng Việt</strong></p>
  <p>Giao diện Tiếng Việt &amp; 9 ngôn ngữ khác, thống kê Context &amp; mức sử dụng, bố cục gọn, phân nhánh &amp; sửa tin nhắn, chuyển đổi nhiều tài khoản, Proxy không cần TUN, hỗ trợ SSH &amp; WSL2</p>
  <!-- plugin-badges:start -->
  <p>
    <a href="https://github.com/WhiteBr1ck/agy-powertools/releases"><img src="https://img.shields.io/github/v/release/WhiteBr1ck/agy-powertools?label=Upstream&color=2563eb" height="20" alt="Upstream Release" /></a>
    <a href="LICENSE"><img src="https://img.shields.io/github/license/WhiteBr1ck/agy-powertools?label=License&color=16a34a" height="20" alt="MIT License" /></a>
    <img src="https://img.shields.io/badge/Locale-Ti%E1%BA%BFng%20Vi%E1%BB%87t%20(100%25)-e11d48" height="20" alt="Tiếng Việt" />
    <img src="https://img.shields.io/badge/Antigravity-2.35.0-0f172a" height="20" alt="Antigravity 2.35.0" />
    <img src="https://img.shields.io/badge/Node.js-%3E%3D22.13-339933" height="20" alt="Node.js >= 22.13" />
    <img src="https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux%20%7C%20WSL2-475569" height="20" alt="Platform" />
  </p>
  <!-- plugin-badges:end -->
  <p><a href="https://github.com/WhiteBr1ck/agy-powertools/blob/main/README.md">简体中文 (Gốc)</a> | <a href="docs/README_ZH_TW.md">繁體中文</a> | <a href="README_EN.md">English</a> | <a href="docs/README_FR.md">Français</a> | <a href="docs/README_JA.md">日本語</a> | <a href="docs/README_KO.md">한국어</a> | <a href="docs/README_DE.md">Deutsch</a> | <a href="docs/README_ES.md">Español</a> | <a href="docs/README_RU.md">Русский</a> | <strong>Tiếng Việt</strong></p>
  <p>
    <a href="#cai-dat-nhanh">Cài đặt nhanh</a> |
    <a href="#anh-chup-man-hinh">Ảnh chụp màn hình</a> |
    <a href="#tinh-nang">Tính năng</a> |
    <a href="#cau-hinh">Cấu hình</a> |
    <a href="#lich-su-phien-ban">Lịch sử phiên bản</a>
  </p>
</div>

<p align="center">
  <img src="docs/images/hero-workspace.png" alt="Giao diện làm việc Agy Powertools" width="100%" />
</p>

> **Giới thiệu bản Fork Việt hóa:** Đây là nhánh phát triển bổ sung gói ngôn ngữ **Tiếng Việt hoàn chỉnh (`lib/locales/vi.mjs` - hơn 2.300 chuỗi)** trên nền mã nguồn gốc [WhiteBr1ck/agy-powertools](https://github.com/WhiteBr1ck/agy-powertools) (giấy phép MIT).
> - Gắn vào Antigravity 2.0 qua giao diện debug cục bộ và đọc các tệp session SQLite/JSONL ở chế độ **chỉ đọc**, không sửa file cài đặt gốc của ứng dụng.
> - **Lưu ý khi dùng bản Fork này:** Không bấm cập nhật tự động (In-app Update) trong Settings, vì bản phát hành từ repo gốc hiện chưa có sẵn gói Tiếng Việt và sẽ ghi đè bản dịch cục bộ.

---

<a id="cai-dat-nhanh"></a>
## Cài đặt nhanh & Bật Tiếng Việt

> Yêu cầu: Đã cài và mở Antigravity ít nhất một lần. Sử dụng Node.js cục bộ `>= 22.13` hoặc tự động dùng `agy-node` đi kèm Antigravity. Không cần `npm install` hay quyền quản trị viên.

### Bước 1: Tải và cài đặt từ nhánh này

```sh
# macOS / Linux / WSL2
git clone -b vi https://github.com/nhattuan612/agy-powertools.git
cd agy-powertools
sh ./install.sh
```

```powershell
# Windows (PowerShell)
git clone -b vi https://github.com/nhattuan612/agy-powertools.git
cd agy-powertools
powershell -NoProfile -ExecutionPolicy Bypass -File .\install.ps1
```

*(Hoặc tải file ZIP nhánh `vi` trên GitHub, giải nén rồi chạy `./install.sh` hoặc `install.ps1`.)*

### Bước 2: Chuyển giao diện sang Tiếng Việt

1. Khởi động lại Antigravity (trên macOS, plugin sẽ tự khởi động lại 1 lần kèm cờ debug nếu bạn mở app trực tiếp).
2. Mở mục **Powertools** ở thanh bên trái -> chọn tab **Settings** -> tìm mục **Language** -> chọn **Tiếng Việt**.
3. Toàn bộ giao diện Powertools và các menu/hộp thoại thường dùng của Antigravity sẽ chuyển sang Tiếng Việt ngay lập tức.

### Gỡ cài đặt

- Chạy `sh ./uninstall.sh` (macOS / Linux / WSL2) hoặc `powershell -NoProfile -ExecutionPolicy Bypass -File .\uninstall.ps1` (Windows). Thêm `--keep-settings` nếu muốn giữ lại cấu hình đã lưu. Lịch sử chat, tài khoản và các plugin khác hoàn toàn không bị ảnh hưởng.

---

<a id="anh-chup-man-hinh"></a>
## Ảnh chụp màn hình

<table>
  <tr>
    <th width="50%">Context Window &amp; Thống kê tốc độ</th>
    <th width="50%">Tiến độ tác vụ &amp; Quota trong Overview</th>
  </tr>
  <tr>
    <td>
      <img src="docs/images/card-composer.png" alt="Context window và thống kê tốc độ" width="100%" />
      <p>Xem mức dùng Context, tỷ lệ tái sử dụng Cache và tốc độ sinh token ngay cạnh bộ chọn model, kèm tùy chọn vòng Quota bao quanh khung nhập liệu.</p>
    </td>
    <td>
      <img src="docs/images/card-overview-panel.png" alt="Tiến độ tác vụ và Quota trong Overview" width="100%" />
      <p>Theo dõi từng bước thực thi trực tiếp, thời gian mỗi bước và Quota model còn lại ở bảng Overview bên phải; nhấn vào tiêu đề mục để thu gọn.</p>
    </td>
  </tr>
  <tr>
    <th>Tổng quan sử dụng (Giao diện Sáng)</th>
    <th>Tổng quan sử dụng (Giao diện Tối)</th>
  </tr>
  <tr>
    <td>
      <img src="docs/images/card-dashboard-light.png" alt="Tổng quan sử dụng ở giao diện sáng" width="100%" />
      <p>Mặc định hiển thị theo chu kỳ Quota tuần hiện tại, gồm số request, Token, tỷ lệ cache hit, chi phí ước tính, biểu đồ nhiệt 53 tuần và tình trạng từng model.</p>
    </td>
    <td>
      <img src="docs/images/card-dashboard-dark.png" alt="Tổng quan sử dụng ở giao diện tối" width="100%" />
      <p>Tự động đồng bộ giao diện sáng/tối của ứng dụng, so sánh tỷ trọng Token, chi phí, tỷ lệ cache hit và tốc độ giữa các model.</p>
    </td>
  </tr>
  <tr>
    <th>Danh sách Request &amp; Bất thường Cache</th>
    <th>Đa tài khoản &amp; Quản lý Quota (Mặc định tắt)</th>
  </tr>
  <tr>
    <td>
      <img src="docs/images/card-requests.png" alt="Danh sách request và cảnh báo bất thường cache" width="100%" />
      <p>Lọc request theo tài khoản, model, hội thoại và trạng thái; gắn cờ các lần rớt Cache bất thường trong khoảng thời gian ngắn (bỏ qua cold start và compaction).</p>
    </td>
    <td>
      <img src="docs/images/card-accounts.png" alt="Chuyển đổi nhiều tài khoản và quản lý Quota" width="100%" />
      <p>Lưu và chuyển đổi nhiều tài khoản Google cục bộ qua kho khóa bảo mật của hệ điều hành, xem Quota 5 giờ và theo tuần tại một nơi.</p>
    </td>
  </tr>
  <tr>
    <th>Cài đặt Ngôn ngữ &amp; Hiển thị</th>
    <th>Proxy không cần TUN (Mặc định tắt)</th>
  </tr>
  <tr>
    <td>
      <img src="docs/images/card-settings.png" alt="Cài đặt ngôn ngữ và hiển thị" width="100%" />
      <p>Hỗ trợ 10 ngôn ngữ giao diện, bật/tắt bố cục gọn, tô màu bong bóng tin nhắn người dùng và vòng viền Quota.</p>
    </td>
    <td>
      <img src="docs/images/card-proxy.png" alt="Cài đặt Proxy riêng không cần TUN" width="100%" />
      <p>Định tuyến riêng Antigravity qua HTTP hoặc SOCKS5 kèm kiểm tra kết nối tích hợp, ép HTTP/1.1 và xác minh cập nhật trong ứng dụng.</p>
    </td>
  </tr>
</table>

---

<a id="tinh-nang"></a>
## Tính năng

- **Giao diện đa ngôn ngữ (10 ngôn ngữ)**: Việt hóa đầy đủ (1.611 nhãn giao diện gốc, 589 chuỗi bảng điều khiển, 145 mẫu động, 39 chuỗi Sidecar) cho Powertools, menu thường dùng của Antigravity, hộp thoại cấp quyền, cài đặt và iframe Swarm, giữ nguyên nội dung chat và khối code.
- **Đo lường Context và tốc độ**: Thêm vòng tròn sử dụng Context (kèm tỷ lệ tái sử dụng Cache, số lần nén và thanh planner/executor của Orchestrator) cùng đồng hồ tốc độ (`tok/s`, TTFT, thời gian model vs tool, chi phí phiên ước tính) ngay cạnh khung nhập, bao gồm cả thống kê Subagent.
- **Dashboard sử dụng và log Request cục bộ**: Thêm trang `Powertools` ở thanh bên kết hợp dữ liệu Desktop và `agy` CLI, gồm tổng quan sử dụng (biểu đồ nhiệt 53 tuần, biểu đồ tròn Token/chi phí, bảng model), nhật ký từng request, cờ bất thường Cache, nút copy lỗi 1 chạm, ước tính Quota và làm mới bảng giá API chính thức.
- **Bố cục gọn và cập nhật theo giai đoạn**: Giữ nguyên cỡ chữ của ứng dụng trong khi tinh chỉnh giãn dòng và khoảng cách khối; hiển thị tiến độ ngắn gọn trong lượt chạy nhiều bước và tự gập vào tiêu đề thời gian xử lý khi hoàn tất.
- **Phân nhánh hội thoại và sửa tin nhắn tại chỗ**: Tạo nhánh (fork) hội thoại mới từ bất kỳ phản hồi hoặc menu hội thoại nào với đầy đủ lịch sử (kể cả hội thoại có Subagent), hoặc sửa trực tiếp tin nhắn đã gửi ngay trên khung nhập nguyên bản của Antigravity.
- **Chuyển đổi nhiều tài khoản (mặc định tắt)**: Dùng Windows Credential Manager, macOS Keychain hoặc Linux Secret Service để cô lập nhiều tài khoản Google không lưu token văn bản thuần; theo dõi Quota 5 giờ / tuần ở thanh bên và tùy chọn tự chuyển khi cạn Quota.
- **Proxy riêng cho ứng dụng không cần TUN (mặc định tắt)**: Tiêm cờ Proxy và biến môi trường chỉ cho Antigravity khi khởi động lại, hỗ trợ kiểm tra HTTP CONNECT / SOCKS5, nhắc khi cold-start và tùy chọn `GODEBUG=http2client=0` để giảm lỗi ngắt `EOF`.
- **Hỗ trợ SSH Remote và WSL2**: Đọc dữ liệu phiên từ xa, Subagent và thống kê trên cửa sổ `SSH` qua OpenSSH cục bộ mà không cần cài gì lên server; hỗ trợ Antigravity trên Windows kết hợp WSL2 ở cả chế độ mạng NAT và Mirrored.
- **Menu chuột phải cho tệp và tiện ích nhỏ**: Chuột phải vào liên kết tệp hoặc cây Files để đính kèm vào chat, mở, mở thư mục chứa, sao chép tệp hoặc đường dẫn (kể cả đường dẫn NAS / SMB LAN trên Windows); bổ sung các mục thu gọn Tiến độ tác vụ & Quota trong Overview, bộ đếm chưa đọc trên thanh tiêu đề, vòng Quota và tô màu tin nhắn người dùng.

---

## Tính năng vui (Nhưng đẹp mắt)

<p align="center">
  <img src="docs/images/card-border-beam.webp" alt="Hiệu ứng dải sáng viền khung nhập khi đang xử lý" width="100%" />
</p>

- **Dải sáng viền khung nhập khi đang xử lý (mặc định tắt)**: Lấy cảm hứng từ [border-beam-ios](https://github.com/ismnoiet/border-beam-ios), dùng shader WebGL SDF bo góc nhẹ. Tạo vệt sáng mượt chạy đều quanh khung nhập liệu khi agent đang làm việc và mờ dần về 0% tải CPU/GPU khi lượt chạy kết thúc. Chuyển mượt với vòng viền Quota khi bật cả hai, kèm 6 bảng màu (`Gemini`, `Aurora`, `Colorful`, `Neon`, `Accent`, `Quota`) và nút **Thử xem trước** trong Cài đặt.

---

<a id="cau-hinh"></a>
## Cấu hình

Mọi thiết lập áp dụng trực tiếp trong **Powertools -> Cài đặt** và tự động lưu (**Khôi phục mặc định** nằm ở cuối trang). Xem hướng dẫn cài qua Agent tại [docs/INSTALL_AGENT.md](docs/INSTALL_AGENT.md).

<details>
<summary><strong>Mở rộng toàn bộ danh sách cài đặt, biến môi trường và đường dẫn</strong></summary>

### Giao diện & hiển thị

| Thiết lập | Mặc định | Mô tả |
| --- | --- | --- |
| Bật Powertools | Bật | Công tắc tổng; tạm dừng mọi mở rộng giao diện mà vẫn giữ cấu hình đã lưu |
| Ngôn ngữ | `简体中文` | Chọn một trong 10 ngôn ngữ giao diện (bao gồm `Tiếng Việt`) |
| Phông chữ và độ đậm cục bộ | Mặc định app | Tìm theo tên bản địa hoặc họ font để áp dụng; chỉnh độ đậm riêng; đặt lại để về mặc định; Terminal vẫn dùng font riêng |
| Bố cục gọn | Bật | Giảm chiều cao dòng (`1.4`) và khoảng cách khối/tool trong khi giữ nguyên cỡ chữ |
| Tô màu bong bóng tin nhắn người dùng | Tắt | Thêm nền màu và viền cho tin nhắn người dùng (Accent, 5 mẫu màu, màu tùy chỉnh và thanh trượt độ đậm 10%-100%) |
| Luôn hiện thanh điều hướng hội thoại | Bật | Giữ thanh nhảy giữa các lượt trong hội thoại nhiều lượt luôn hiển thị |
| Giữ mở Overview khi chuyển hội thoại | Bật | Lưu trạng thái mở/đóng bảng Overview bên phải khi chuyển đổi chat |
| Số hội thoại mỗi dự án | `Mặc định (6)` | Điều chỉnh số chat hiển thị mỗi dự án ở thanh bên (`Mặc định (6)`, `1-10`, hoặc `Hiện tất cả`) |
| Kéo thả thư mục vào thanh bên | Bật | Tạo hoặc mở dự án bằng cách kéo thả thư mục cục bộ vào thanh bên |
| Ghim dự án vừa kéo thả | Tắt | Tự động ghim các dự án được tạo hoặc mở qua thao tác kéo thả |
| Dải sáng chạy trên thanh bên | Tắt | Vẽ vệt sáng SVG chạy quanh khung hội thoại đang chạy ở thanh bên (hỗ trợ ẩn vòng quay 4 chấm gốc, cảnh báo màu hổ phách khi chờ xác nhận) |
| Nhóm hội thoại đang chạy | Tắt | Ghim mục Đang chạy thu gọn được ở đầu thanh bên hiển thị tất cả chat, dự án, Subagent đang hoạt động và cảnh báo chờ xác nhận |
| Huy hiệu chưa đọc trên thanh tiêu đề | Bật | Hiện số `(N)` chưa đọc trên tiêu đề cửa sổ/thanh tác vụ khi chat chạy nền hoàn tất |

### Đo lường & tiến độ

| Thiết lập | Mặc định | Mô tả |
| --- | --- | --- |
| Khoảng thời gian Overview mặc định | `Quota tuần hiện tại` | Chọn chu kỳ Quota tuần, Hôm nay, 24h, Hôm qua, Tuần này, Tháng này, 30 ngày, hoặc Toàn bộ |
| Vòng tròn Context | Bật | Hiển thị vòng mức dùng Context, chi tiết tái sử dụng Cache và thanh theo từng model của Orchestrator |
| Tốc độ & thống kê | Bật | Hiển thị đồng hồ tốc độ và mở chi tiết thống kê phiên kèm chi phí ước tính |
| Tiến độ tác vụ | Bật | Mục thu gọn trong Overview hiển thị danh sách kiểm tra, giai đoạn hiện tại và thời lượng từng bước |
| Hiện Quota trong Overview | Tắt | Mục thu gọn trong Overview hiển thị Quota 5 giờ và hàng tuần còn lại |
| Mở nhanh Overview ở thanh tiêu đề | Tắt | Thêm nút Powertools ở góc trên bên phải để mở popover 6 tab ngay trên hội thoại hiện tại |
| Vòng viền Quota quanh khung nhập | Tắt | Vẽ vòng Quota còn lại theo chiều kim đồng hồ quanh khung nhập (xanh ngọc, hổ phách hoặc đỏ) |
| Cửa sổ vòng Quota | `Tự động (thấp hơn)` | Chọn `Tự động (thấp hơn)`, `Giới hạn tuần` hoặc `Giới hạn 5 giờ` khi bật vòng Quota |
| Dải sáng viền khung nhập khi xử lý | Tắt | Chạy hiệu ứng dải sáng mượt quanh khung nhập khi đang xử lý (0% tải khi nghỉ), chuyển mượt với vòng Quota, có 6 bảng màu & Xem trước |
| Context & thống kê Subagent | Bật | Hiển thị model, mức dùng Context, Token, tỷ lệ cache hit, tốc độ và chi phí cho từng Subagent |
| Thời lượng lượt chạy / Mở rộng tool | Bật | Hiển thị tổng thời gian ở lượt đã xong và nhấn để mở rộng chi tiết tool |
| Thống kê cuối mỗi lượt trả lời | Tắt | Hiện model, tỷ lệ cache hit, Token vào/ra và chi phí ước tính ở chân phản hồi, rê chuột để xem chi tiết |

### Tính năng mở rộng, Tài khoản, Proxy & Context thử nghiệm

| Thiết lập | Mặc định | Mô tả |
| --- | --- | --- |
| Cập nhật tiến độ theo giai đoạn | Bật | Báo cáo tiến độ ngắn trong lượt chạy tool nhiều bước và gập lại khi xong |
| Tìm kiếm & đọc song song | Tắt | Hướng dẫn agent gộp nhiều thao tác tìm kiếm và đọc tệp trong một lượt |
| Tìm kiếm toàn văn trong hộp thoại gốc | Bật | Mở rộng modal tìm kiếm hội thoại gốc để tìm nội dung tin nhắn, khối code, lệnh và nhảy thẳng tới lượt khớp |
| Phân nhánh / Sửa tin nhắn / Menu tệp | Bật | Phân nhánh hội thoại nguyên bản, sửa tin nhắn tại chỗ và menu chuột phải cho tệp (kèm Mở bằng... và nhảy tới `#L:C`) |
| Nhận diện lệnh SSH khi dán | Bật | Tự trích xuất `user@host:port` khi dán `ssh -p PORT user@host` vào ô SSH Host (tự loại bỏ mật khẩu đi kèm) |
| Bật chuyển đổi nhiều tài khoản | Tắt | Cần chủ động bật kèm cảnh báo rủi ro; bộ chuyển ở thanh bên, dạng danh sách/thẻ, xem 5H/tuần và tự chuyển tài khoản |
| Proxy cho ứng dụng (không cần TUN) | Tắt | Nhập giao thức/host/port, kiểm tra kết nối, nhắc khi cold-start và ép HTTP/1.1 |
| Mục tiêu Context (Thử nghiệm) | `Mặc định` | Chọn `Mặc định`, `256K`, `500K` hoặc `1M` (`Mặc định` giữ nguyên thiết lập gốc) |

### Biến môi trường & đường dẫn

| Tên / Đường dẫn | Mô tả |
| --- | --- |
| `ANTIGRAVITY_USER_DATA_DIR` | Thư mục dữ liệu người dùng Antigravity tùy chỉnh cho profile tách biệt |
| `ANTIGRAVITY_CLI_DATA_DIR` | Thư mục dữ liệu `agy` CLI tùy chỉnh (mặc định `~/.gemini/antigravity-cli`) |
| `ANTIGRAVITY_CDP_PORT_FILE` | Đường dẫn chỉ định tới `DevToolsActivePort` (cũng hỗ trợ `AGY_BROWSER_ACTIVE_PORT_FILE`) |
| `~/.gemini/config/plugins/agy-powertools/` | Thư mục chứa tệp plugin và script thực thi đã cài |
| `~/.gemini/antigravity/plugin_data/agy-powertools/` | Dữ liệu cài đặt đã lưu, metadata tài khoản, mẫu Quota và bộ nhớ đệm bảng giá |

</details>

---

<a id="lich-su-phien-ban"></a>
## Lịch sử phiên bản

### Bản Việt hóa (trên nền v2.16.11)
- **Bổ sung gói ngôn ngữ Tiếng Việt (`vi`) hoàn chỉnh**: Việt hóa toàn bộ 1.611 chuỗi giao diện gốc Antigravity, 589 chuỗi bảng điều khiển/cài đặt Powertools, 145 pattern động, 39 chuỗi Aux Pane Sidecar, định dạng thời gian tiếng Việt và tài liệu hướng dẫn Tiếng Việt.
- **Vượt qua toàn bộ kiểm thử tự động**: Toàn bộ test i18n, lifecycle, settings và đóng gói đều đạt chuẩn tương thích với dự án gốc `WhiteBr1ck/agy-powertools`.

### v2.16.11 (Upstream)
- Sửa lỗi crash sidecar khi dùng Proxy SOCKS5 (#93, #64), sửa lỗi lẫn thông tin đăng nhập đa tài khoản và giải mã tiền tố Keyring macOS (#97, #95), hỗ trợ NTFS junction `.gemini` trên Windows (#96, #100), sửa độ đậm font tùy chỉnh, sửa lỗi Node 24 quét `.lnk`, nâng giới hạn `custom-i18n.json` lên 2000 ký tự và gộp 3 PR cộng đồng (#94, #98, #86, #83).

Xem toàn bộ lịch sử phiên bản đầy đủ tại [README_EN.md](README_EN.md#changelog).

---

## Giấy phép & liên kết

- **Mã nguồn gốc**: [WhiteBr1ck/agy-powertools](https://github.com/WhiteBr1ck/agy-powertools)
- **Giấy phép**: [MIT License](LICENSE) (lịch chọn khoảng ngày tùy biến từ HextaUI dùng `react-day-picker` và `date-fns`; xem [lib/vendor/NOTICE.txt](lib/vendor/NOTICE.txt))
- **Báo lỗi**: [GitHub Issues (Upstream)](https://github.com/WhiteBr1ck/agy-powertools/issues)
