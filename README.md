#!/data/data/com.termux/files/usr/bin/bash

# Update & upgrade
pkg update -y && pkg upgrade -y

# Cài gói cần thiết
pkg install -y python clang git libffi openssl libcrypt ndk-sysroot wget curl

# Fix pip
pip install --upgrade pip setuptools wheel

# Cài thư viện Python
pip install requests beautifulsoup4 colorama cloudscraper wget

# Vào thư mục Download
cd /sdcard/download

# Tải file golike.py về
wget -O golike.py "https://drive.usercontent.google.com/download?id=1yj9OFn4EY9s8dIt70UCukfylgwcQpUxw&export=download&authuser=0&confirm=t&uuid=bb78e2e0-fd67-4250-917f-22ef2ed49cdc&at=AN8xHoofSyvZsrgAXrnqkhmnh7Ce%3A1756039723050"

# Chạy tool
python golike.py
