Debian/Ubuntu için Node.js kurulum kılavuzu:

**TÜRKÇE:**

1. **NVM (Node Version Manager) Kurulumu:**
```bash
# NVM kurulum scripti
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash

# veya wget ile
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash
```

2. **NVM'i Aktif Etme:**
```bash
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
```

3. **Node.js Kurulumu:**
```bash
# En son kararlı sürümü kurma
nvm install node

# Belirli bir sürümü kurma
nvm install 14.17.0

# LTS (Uzun Süreli Destek) sürümünü kurma
nvm install --lts
```

4. **Node Sürümünü Kontrol Etme:**
```bash
node --version
npm --version
```

5. **Temel Global Paketler (İsteğe Bağlı):**
```bash
npm install -g nodemon
npm install -g pm2
npm install -g yarn
```

**ENGLISH:**

1. **Installing NVM (Node Version Manager):**
```bash
# NVM installation script
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash

# or with wget
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash
```

2. **Activating NVM:**
```bash
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
```

3. **Installing Node.js:**
```bash
# Install latest stable version
nvm install node

# Install specific version
nvm install 14.17.0

# Install LTS (Long Term Support) version
nvm install --lts
```

4. **Check Node Version:**
```bash
node --version
npm --version
```

5. **Basic Global Packages (Optional):**
```bash
npm install -g nodemon
npm install -g pm2
npm install -g yarn
```

**Yararlı NVM Komutları / Useful NVM Commands:**

```bash
# Mevcut sürümleri listeleme / List installed versions
nvm ls

# Kullanılabilir sürümleri görüntüleme / Show available versions
nvm ls-remote

# Sürüm değiştirme / Switch version
nvm use 14.17.0

# Varsayılan sürümü ayarlama / Set default version
nvm alias default 14.17.0

# Node'u kaldırma / Uninstall Node
nvm uninstall 14.17.0
```

**Proje Başlatma / Starting a Project:**
```bash
# Yeni proje oluşturma / Create new project
mkdir my-project
cd my-project

# Package.json oluşturma / Create package.json
npm init

# veya varsayılan ayarlarla / or with default settings
npm init -y

# Bağımlılık ekleme / Add dependencies
npm install express
npm install dotenv
```

**PM2 Temel Komutlar / PM2 Basic Commands:**
```bash
# Uygulamayı başlatma / Start application
pm2 start app.js

# Durum kontrolü / Check status
pm2 status

# Log görüntüleme / View logs
pm2 logs

# Uygulamayı yeniden başlatma / Restart application
pm2 restart app.js

# Tüm uygulamaları durdurma / Stop all applications
pm2 stop all
```

Bu kurulum ve komutlarla Node.js geliştirme ortamınız hazır olacaktır. / With these installations and commands, your Node.js development environment will be ready.
