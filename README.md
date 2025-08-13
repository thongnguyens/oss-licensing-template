# OSS Licensing Template (VI)

> Bộ khung (template) repo GitHub tập trung vào **giấy phép (license)**, **bản quyền (copyright)**,
> **attribution**, và **sử dụng nội dung bên thứ ba**. Mục tiêu là giúp bạn công khai dự án an toàn,
> rõ quyền & nghĩa vụ, tránh rủi ro DMCA.

<p align="left">
  <img alt="License" src="https://img.shields.io/badge/License-MIT-green">
  <img alt="PRs" src="https://img.shields.io/badge/PRs-welcome-brightgreen">
  <img alt="SPDX" src="https://img.shields.io/badge/SPDX-compliant-blue">
</p>

---

## Mục lục
- [1. Tên repo & mô tả gợi ý](#1-tên-repo--mô-tả-gợi-ý)
- [2. Cấu trúc thư mục](#2-cấu-trúc-thư-mục)
- [3. Giấy phép cho *toàn repo*](#3-giấy-phép-cho-toàn-repo)
- [4. MIT License là gì (tóm tắt)](#4-mit-license-là-gì-tóm-tắt)
- [5. Thêm nội dung bên thứ ba *đúng cách*](#5-thêm-nội-dung-bên-thứ-ba-đúng-cách)
- [6. Attribution (Ghi công) — ví dụ nhanh](#6-attribution-ghi-công--ví-dụ-nhanh)
- [7. SPDX Header: thêm vào file mã/tài liệu](#7-spdx-header-thêm-vào-file-mãtài-liệu)
- [8. NOTICE vs LICENSE vs THIRD_PARTY_LICENSES](#8-notice-vs-license-vs-third_party_licenses)
- [9. DMCA, thương hiệu & hình ảnh](#9-dmca-thương-hiệu--hình-ảnh)
- [10. Quy trình đóng góp](#10-quy-trình-đóng-góp)
- [11. Gắn Topics & mô tả GitHub](#11-gắn-topics--mô-tả-github)
- [12. Miễn trừ trách nhiệm](#12-miễn-trừ-trách-nhiệm)
- [📜 Bản quyền](#📜-bản-quyền)

---

## 1. Tên repo & mô tả gợi ý

- **Tên repo (slug):** `oss-licensing-template` *(gọn, rõ mục đích)*
- **Description:** *"Template hướng dẫn giấy phép, bản quyền & attribution cho dự án GitHub (VI)"*

Bạn có thể đổi tên repo theo dự án thực tế; phần còn lại vẫn dùng chung.

---

## 2. Cấu trúc thư mục

```text
oss-licensing-template/
├─ README.md                   # Hướng dẫn chính (file này)
├─ LICENSE                     # Giấy phép MIT cho toàn repo
├─ NOTICE                      # Thông báo bản quyền/người giữ bản quyền
├─ ATTRIBUTIONS.md             # Ghi công (ảnh, logo, snippet, v.v.)
├─ THIRD_PARTY_LICENSES.md     # Bản quyền/giấy phép của bên thứ ba
├─ CONTRIBUTING.md             # Quy tắc đóng góp
└─ .github/
   └─ PULL_REQUEST_TEMPLATE.md # Mẫu PR (nhắc thêm license/attribution khi cần)
```

---

## 3. Giấy phép cho *toàn repo*

Repo này phát hành theo **MIT License**. Xem chi tiết trong [LICENSE](./LICENSE).  
Nếu bạn sao chép template này, hãy **đổi tên chủ bản quyền & năm** trong `LICENSE` và `NOTICE`.

> **Lưu ý:** MIT chỉ bao phủ **nội dung bạn sở hữu** trong repo. Nội dung bên thứ ba vẫn theo giấy phép riêng.

---

## 4. MIT License là gì (tóm tắt)

- **Cho phép rộng rãi:** dùng/sửa/sao chép/phân phối/bán (kể cả thương mại).
- **Yêu cầu:** giữ lại thông báo copyright + điều khoản MIT.
- **Không bảo hành:** phần mềm cung cấp "AS IS".
- **Không copyleft:** không buộc mở mã nguồn khi phân phối.
- **Không cấp quyền thương hiệu:** logo/nhãn hiệu cần phép riêng.

Chi tiết đầy đủ: xem [LICENSE](./LICENSE).

---

## 5. Thêm nội dung bên thứ ba *đúng cách*

1. **Kiểm tra license** (Apache-2.0, MIT, BSD, GPL, CC BY/CC BY-SA, v.v.).
2. **Tuân thủ yêu cầu:** giữ NOTICE, kèm file license, ghi công, share-alike (nếu CC BY-SA/GPL), v.v.
3. **Tối thiểu cần có:** điền bảng trong `THIRD_PARTY_LICENSES.md` và ghi vào `ATTRIBUTIONS.md` nếu yêu cầu attribution.
4. **Không re-host tài liệu có bản quyền đóng** (sách/slide thương mại, file khoá học…): chỉ **đặt link chính thức**.
5. **Tôn trọng thương hiệu/nhãn hiệu**: không dùng logo nếu chưa được phép (trừ khi license của logo cho phép).

> Nếu license **không rõ ràng**, hãy **liên hệ tác giả** hoặc **không đưa vào**.

---

## 6. Attribution (Ghi công) — ví dụ nhanh

Trong `ATTRIBUTIONS.md`:
```md
- Biểu tượng "Network Icon" của Jane Doe, bản quyền © 2023, dùng theo CC BY 4.0.
  Nguồn: https://example.com/network-icon  |  Bằng chứng license: https://example.com/license
  Thay đổi: đổi màu và kích thước.
```

Trong source code (comment header):
```text
Portions © 2024 John Smith, used under MIT. See THIRD_PARTY_LICENSES.md.
```

---

## 7. SPDX Header: thêm vào file mã/tài liệu

Thêm vào **dòng đầu** mỗi file bạn tạo:
```text
SPDX-License-Identifier: MIT
```

Ví dụ:
```bash
#!/usr/bin/env bash
# SPDX-License-Identifier: MIT
```

```md
<!-- SPDX-License-Identifier: MIT -->
```

---

## 8. NOTICE vs LICENSE vs THIRD_PARTY_LICENSES

- **LICENSE:** giấy phép **chính** của repo (MIT).
- **NOTICE:** ghi nhận **chủ sở hữu bản quyền** & có thể liệt kê tuyên bố bổ sung (nếu áp dụng).
- **THIRD_PARTY_LICENSES.md:** liệt kê nội dung bên thứ ba bạn sử dụng + link đến license tương ứng.

> Một số license (VD: Apache-2.0) **bắt buộc** giữ lại `NOTICE` khi phân phối — hãy tuân thủ nếu bạn sử dụng nội dung Apache-2.0.

---

## 9. DMCA, thương hiệu & hình ảnh

- **DMCA:** Không đưa lên repo nội dung mà bạn **không có quyền** (sách/slide thương mại, tài liệu khoá học, media mua bản quyền…).
- **Thương hiệu:** Tên sản phẩm/nhãn hiệu thuộc về chủ sở hữu; MIT **không** cấp phép dùng nhãn hiệu.
- **Hình ảnh/ảnh chụp màn hình:** đảm bảo có quyền sử dụng hoặc được phép theo license nguồn.

> Đây **không phải tư vấn pháp lý**. Khi nghi ngờ, hãy hỏi luật sư hoặc gỡ nội dung rủi ro.

---

## 10. Quy trình đóng góp

- Đọc [CONTRIBUTING.md](./CONTRIBUTING.md).
- Mọi PR cần:
  - Không đưa nội dung vi phạm bản quyền.
  - Điền/ cập nhật `THIRD_PARTY_LICENSES.md` và/hoặc `ATTRIBUTIONS.md` nếu thêm nội dung bên thứ ba.
  - Giữ header `SPDX-License-Identifier` trong file mới.

---

## 11. Gắn Topics & mô tả GitHub

```bash
gh repo edit <owner>/<repo>   --description "Template hướng dẫn giấy phép, bản quyền & attribution (VI)"   --add-topic license --add-topic oss --add-topic spdx --add-topic attribution   --add-topic dmca --add-topic compliance --add-topic open-source
```

---

## 12. Miễn trừ trách nhiệm

Tài liệu này nhằm mục đích **thông tin/giáo dục**, **không** phải tư vấn pháp lý.  
Bạn chịu trách nhiệm cuối cùng cho việc tuân thủ giấy phép & pháp luật hiện hành.

---

## 📜 Bản quyền

Phát hành theo giấy phép **MIT** — xem [LICENSE](./LICENSE).
