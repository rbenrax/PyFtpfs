# PyFtpfs

**PyFtpfs** is a Python-based tool that allows you to mount FTP file systems using FUSE (Filesystem in Userspace), enabling interaction with remote FTP servers as if they were local file systems.  
> ⚠️ *This project is under development and not yet recommended for production use.*

---

## 📌 Features

- Mount a remote FTP server as a local filesystem.
- Written in **Python** and built on top of FUSE.
- Seamlessly interact with FTP files via local paths after mounting.

---

## 🚀 Requirements

Before installing and using PyFtpfs, make sure you have:

- **Python** (version 3.7+ recommended).
- A system with **FUSE** support (Linux / macOS with FUSE installed).
- The `fusepy` library and other dependencies installed.

---

## 🛠️ Installation

```bash
git clone https://github.com/rbenrax/PyFtpfs.git
cd PyFtpfs
```

(Optional) Create a virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 🚀 Usage

### 🌐 Mount an FTP server

```bash
python pyftpfs.py ftp.server.com /mnt/ftp -u username -P password
```

### 🔧 Common options

| Option | Description |
|-------|-------------|
| `-p <port>` | FTP port (default: 21) |
| `-u <username>` | FTP username |
| `-P <password>` | FTP password |
| `-d` | Enable debug output |

Example:

```bash
python pyftpfs.py ftp.server.com /mnt/ftp -p 21 -u myuser -P mypassword -d
```

---

## 🔌 Unmounting

To unmount the filesystem:

```bash
fusermount -u /mnt/ftp
```

On macOS:

```bash
umount /mnt/ftp
```

---

## 🧪 Project Status

This project is **under active development** and may lack full features or optimizations. Please check the *issues* section to view pending enhancements or bugs.

---

## 📝 Contributing

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/name`).
3. Commit your changes (`git commit -m "Description"`).
4. Open a Pull Request.

---

## 📜 License

This project is licensed under the **Apache-2.0 License**.

---

## 📎 Resources

- 📦 Source code: https://github.com/rbenrax/PyFtpfs
