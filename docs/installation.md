# Installation

This guide explains how to install **DAI** using the official prebuilt binaries from the `dai-releases` repository.  
Building from source is only recommended for contributors or developers.

---

## 📦 Install from prebuilt binary (recommended)

1. **Download the latest release** for your OS from:  
   [https://github.com/gorankrgovic/dai-releases/releases/latest](https://github.com/gorankrgovic/dai-releases/releases/latest)

2. **Unpack the archive** (if downloaded as `.zip` or `.tar.gz`):
```bash
tar -xvzf dai_<version>_linux_amd64.tar.gz
# or
unzip dai_<version>_macos_arm64.zip
```

3. **Make the binary executable**:
```bash
chmod +x dai
```

4. **Move it to your PATH**:
```bash
sudo mv dai /usr/local/bin
```

5. **Verify installation**:
```bash
dai --version
```

---

## 🛠 Build from source (for contributors only)

If you want to work on DAI or contribute to its development:

1. **Clone the main repository**:
```bash
git clone https://github.com/gorankrgovic/dai.git
cd dai
```

2. **Build the binary**:
```bash
go build -o dai
```

3. **Move to your PATH**:
```bash
sudo mv dai /usr/local/bin
```

4. **Verify installation**:
```bash
dai --version
```

---

## First-time setup

After installing, run:
```bash
dai config
```
This will start the configuration wizard to set your **OpenAI API key** and select the preferred AI model.  
Configuration is stored locally at:
```text
~/.dai/config.yaml
```

---

Next: [Configuration](configuration.md)
