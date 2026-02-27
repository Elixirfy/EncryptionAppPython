# EncryptionAppPython
Ứng dụng mã hóa dữ liệu

# Workflow
Khi làm tính năng mới, ví dụ AES file encryption:

1. Chuyển sang dev:
- git checkout dev
- git pull

2. Tạo feature branch:
- git checkout -b feature/new-feature-name

3. Code

4. Commit:
- git add .
- git commit -m "Cài đặt thêm tính năng <tên tính năng>"

5. Push:
- git push -u origin feature/new-feature-name

6. Lên GitHub → Compare & Pull Request
- Base: dev
- Compare: feature/new-feature-name
- Điền theo PR template
- Create PR

7. Đợi review → Merge vào dev

# Project Skeleton
```
EncryptionAppPython/
│
├── src/
│   ├── __init__.py
│   │
│   ├── crypto/
│   │   ├── __init__.py
│   │   ├── symmetric/
│   │   │   ├── __init__.py
│   │   │   ├── aes.py
│   │   │   ├── triple_des.py
│   │   │   └── blowfish.py
│   │   │
│   │   ├── hashing/
│   │   │   ├── __init__.py
│   │   │   └── password_hash.py
│   │   │
│   │   └── utils/
│   │       ├── __init__.py
│   │       └── key_derivation.py
│   │
│   ├── password/
│   │   ├── __init__.py
│   │   ├── vault.py
│   │   ├── generator.py
│   │   └── storage.py
│   │
│   ├── auth/
│   │   ├── __init__.py
│   │   └── two_factor.py
│   │
│   ├── file_ops/
│   │   ├── __init__.py
│   │   ├── file_encryptor.py
│   │   ├── secure_delete.py
│   │   └── integrity_check.py
│   │
│   └── main.py
│
├── tests/
│   ├── __init__.py
│   ├── test_aes.py
│   ├── test_password_hash.py
│   ├── test_vault.py
│   └── test_secure_delete.py
│
├── .github/
│   ├── pull_request_template.md
│   └── CODEOWNERS
│
├── requirements.txt
├── README.md
└── .gitignore
```
- Tạo và push theo Skeleton này. Mới chỉ có folders chưa có file.
