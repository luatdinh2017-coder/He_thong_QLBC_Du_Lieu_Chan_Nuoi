# He_thong_QLBC_Du_Lieu_Chan_Nuoi
monthly-report-webapp/
│
├── app/                        # Thư mục chính cho ứng dụng Flask
│   ├── __init__.py             # Khởi tạo Flask app
│   ├── routes.py               # Định nghĩa các route (form nhập liệu, xuất báo cáo)
│   ├── drive_service.py        # Tích hợp Google Drive API (đọc/ghi file Excel)
│   ├── excel_utils.py          # Hàm xử lý Excel (openpyxl)
│   ├── templates/              # HTML templates (Jinja2)
│   │   ├── base.html
│   │   ├── form.html           # Form nhập liệu
│   │   └── report.html         # Trang xuất báo cáo
│   └── static/                 # CSS, JS, hình ảnh
│       ├── style.css
│       └── script.js
│
├── tests/                      # Unit tests
│   ├── test_routes.py
│   └── test_excel_utils.py
│
├── requirements.txt            # Danh sách thư viện Python
├── Procfile                    # Khai báo cho Heroku (ví dụ: web: gunicorn app:app)
├── runtime.txt                 # Phiên bản Python (ví dụ: python-3.10.12)
├── config.json                 # Cấu hình OAuth Google Drive (không commit file thật, chỉ mẫu)
├── README.md                   # Hướng dẫn cài đặt và chạy
└── .gitignore                  # Loại trừ file nhạy cảm (config, venv, cache)
