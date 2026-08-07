

🎉 Dự án mã nguồn mở giúp toàn trình reup các video đa nên tảng

Nếu bạn đang tìm một công cụ tự host để tải video và âm thanh từ nhiều nền tảng khác nhau thì ReClip là một dự án mã nguồn mở rất đáng chú ý.

Được xây dựng trên yt-dlp, ReClip cung cấp một giao diện web đơn giản để tải video từ hơn 1.000 website, bao gồm YouTube, TikTok, Instagram, X, Facebook, Reddit, Vimeo và nhiều nền tảng khác.

Một số điểm nổi bật:

* Hỗ trợ tải video từ hơn 1.000 nền tảng thông qua yt-dlp.
* Cho phép tải dưới dạng MP4 hoặc trích xuất MP3.
* Tự động lấy thông tin video và thumbnail trước khi tải.
* Hỗ trợ chọn chất lượng và độ phân giải.
* Có thể dán nhiều liên kết cùng lúc và tự động loại bỏ liên kết trùng.
* Giao diện Web tối giản, không sử dụng framework frontend phức tạp.
* Backend chỉ khoảng 150 dòng Python với rất ít phụ thuộc, dễ đọc và tùy biến.

Ứng dụng thực tế:

* Xây dựng hệ thống tải video nội bộ.
* Thu thập dữ liệu video phục vụ AI và Machine Learning.
* Lưu trữ nội dung đào tạo để xem ngoại tuyến khi được phép.
* Tích hợp vào các workflow xử lý video tự động.
* Làm nền tảng cho các AI Agent xử lý và phân tích nội dung video.

Lưu ý, dự án được phát triển cho mục đích hợp pháp và cá nhân. Khi sử dụng, hãy luôn tuân thủ bản quyền và điều khoản của từng nền tảng đối với nội dung bạn tải xuống.



# ReClip

A self-hosted, open-source video and audio downloader with a clean web UI. Paste links from YouTube, TikTok, Instagram, Twitter/X, and 1000+ other sites — download as MP4 or MP3.

![Python](https://img.shields.io/badge/python-3.8+-blue)
![License](https://img.shields.io/badge/license-MIT-green)

https://github.com/user-attachments/assets/419d3e50-c933-444b-8cab-a9724986ba05

![ReClip MP3 Mode](assets/preview-mp3.png)

## Features

- Download videos from 1000+ supported sites (via [yt-dlp](https://github.com/yt-dlp/yt-dlp))
- MP4 video or MP3 audio extraction
- Quality/resolution picker
- Bulk downloads — paste multiple URLs at once
- Automatic URL deduplication
- Clean, responsive UI — no frameworks, no build step
- Single Python file backend (~150 lines)

## Quick Start

```bash
brew install yt-dlp ffmpeg    # or apt install ffmpeg && pip install yt-dlp
git clone https://github.com/averygan/reclip.git
cd reclip
./reclip.sh
```

Open **http://localhost:8899**.

Or with Docker:

```bash
docker build -t reclip . && docker run -p 8899:8899 reclip
```

## Usage

1. Paste one or more video URLs into the input box
2. Choose **MP4** (video) or **MP3** (audio)
3. Click **Fetch** to load video info and thumbnails
4. Select quality/resolution if available
5. Click **Download** on individual videos, or **Download All**

## Supported Sites

Anything [yt-dlp supports](https://github.com/yt-dlp/yt-dlp/blob/master/supportedsites.md), including:

YouTube, TikTok, Instagram, Twitter/X, Reddit, Facebook, Vimeo, Twitch, Dailymotion, SoundCloud, Loom, Streamable, Pinterest, Tumblr, Threads, LinkedIn, and many more.

## Stack

- **Backend:** Python + Flask (~150 lines)
- **Frontend:** Vanilla HTML/CSS/JS (single file, no build step)
- **Download engine:** [yt-dlp](https://github.com/yt-dlp/yt-dlp) + [ffmpeg](https://ffmpeg.org/)
- **Dependencies:** 2 (Flask, yt-dlp)

## Disclaimer

This tool is intended for personal use only. Please respect copyright laws and the terms of service of the platforms you download from. The developers are not responsible for any misuse of this tool.

## License

[MIT](LICENSE)
