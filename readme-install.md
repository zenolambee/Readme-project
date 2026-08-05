# Installation Guide

Panduan ini untuk menyiapkan lingkungan dasar sebelum menjalankan project.

## 1) Install Git

### Ubuntu / Debian
```bash
sudo apt update
sudo apt install -y git
```

### Cek instalasi
```bash
git --version
```

## 2) Install Node.js

Disarankan menggunakan Node.js 20 LTS.

### Ubuntu / Debian
```bash
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -
sudo apt install -y nodejs
```

### Cek instalasi
```bash
node -v
npm -v
```

## 3) Install OpenCode

### Install global
```bash
npm install -g opencode-ai
```

### Cek instalasi
```bash
opencode --version
```

## 4) Buat konfigurasi OpenCode

Buat folder konfigurasi jika belum ada:

```bash
mkdir -p /root/.config/opencode
```

Lalu simpan file berikut sebagai:

```bash
/root/.config/opencode/opencode.json
```

Contoh isi konfigurasi:

```json
{
  "$schema": "https://opencode.ai/config.json",
  "provider": {
    "nvidia": {
      "npm": "@ai-sdk/openai-compatible",
      "name": "NVIDIA Gateway",
      "options": {
        "baseURL": "http://43.153.225.102:3000/v1"
      },
      "models": {
        "coding": {
          "name": "step-3.7-flash"
        },
        "deepseek-ai/deepseek-v4-flash": {
          "name": "DeepSeek V4 Flash"
        },
        "z-ai/glm-5.2": {
          "name": "GLM 5.2"
        }
      }
    }
  },
  "model": "apiproxy/step-3.7-flash"
}
```

## 5) Jalankan OpenCode

```bash
opencode
```

## Notes

- README ini dibuat khusus untuk instalasi dasar.
- Jika base URL gateway berubah, sesuaikan bagian `baseURL` di konfigurasi.
- Jika perlu, file ini bisa dikembangkan menjadi panduan lengkap untuk VPS Ubuntu.