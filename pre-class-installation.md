# Pre-Class Installation Guide
## AI-Powered Coding Tools Workshop

**Please complete these installations BEFORE the workshop.** This will maximize our hands-on time together. If you encounter issues, we'll have a brief troubleshooting session at the start of class.

---

## Required Software

### 1. Visual Studio Code (VSCode)
**What it is:** A powerful, free code editor that will serve as our main development environment for the workshop.

#### Installation Instructions:

**For Windows:**
1. Go to [https://code.visualstudio.com/](https://code.visualstudio.com/)
2. Click "Download for Windows" (should auto-detect your OS)
3. Run the downloaded `.exe` file
4. Follow the installation wizard:
   - Accept the license agreement
   - Choose installation location (default is fine)
   - **Important:** Check "Add to PATH" option
   - Check "Create a desktop icon" if desired
5. Click "Install" and wait for completion
6. Launch VSCode when installation finishes

**For macOS:**
1. Go to [https://code.visualstudio.com/](https://code.visualstudio.com/)
2. Click "Download for Mac" (should auto-detect your OS)
3. Open the downloaded `.zip` file
4. Drag "Visual Studio Code.app" to your Applications folder
5. Launch VSCode from Applications or use Spotlight search

#### Verification:
- **Windows:** Search for "Visual Studio Code" in Start Menu or click desktop icon
- **macOS:** Look for VSCode in Applications folder or use Spotlight search (`Cmd + Space`, type "vscode")
- **Expected result:** VSCode opens with a welcome screen showing recent files and getting started options

---

### 2. GitHub Account
**What it is:** A platform for code hosting and collaboration. You'll need an account to access AI-powered features later.

#### Account Creation Steps:
1. Go to [https://github.com/](https://github.com/)
2. Click "Sign up" in the top right corner
3. Enter your information:
   - **Username:** Choose something professional (you'll use this for work)
   - **Email:** Use your work or personal email
   - **Password:** Create a strong password
4. Complete the verification puzzle
5. Choose "Free" account when prompted
6. Optionally complete the personalization survey or skip
7. Verify your email address when prompted

#### Verification:
- Log into [https://github.com/](https://github.com/) with your new credentials
- You should see your GitHub dashboard
- **Expected result:** Access to your GitHub profile and repositories page

---

### 3. Python (Latest Version)
**What it is:** The Python programming language and package manager. We'll use the latest stable version for optimal performance and features.

#### Installation Instructions:

**For Windows:**
1. Go to [https://www.python.org/downloads/](https://www.python.org/downloads/)
2. Click "Download Python 3.12.x" (latest version will be shown)
3. Run the downloaded `.exe` file
4. **CRITICAL:** Check "Add Python to PATH" at the bottom of the first screen
5. Click "Install Now" (this installs Python with recommended settings)
6. Wait for installation to complete
7. Click "Close" when finished

**For macOS:**
1. Go to [https://www.python.org/downloads/](https://www.python.org/downloads/)
2. Click "Download Python 3.12.x" (latest version will be shown)
3. Open the downloaded `.pkg` file
4. Follow the installation wizard with default settings
5. Click through "Continue" → "Agree" → "Install"
6. Enter your password when prompted
7. Click "Close" when installation completes

#### Verification:
**Windows (Command Prompt or PowerShell):**
```bash
python --version
pip --version
```

**macOS (Terminal):**
```bash
python3 --version
pip3 --version
```

**Expected result:** 
- Should show Python 3.12.x and pip version numbers
- If Python command isn't recognized, try restarting your terminal/command prompt

---

### 4. Docker Desktop
### 4. Docker Desktop
**What it is:** Containerization platform that enables us to run consistent development environments across different computers.

#### Installation Instructions:

**For Windows:**
1. **System Requirements Check:**
   - Windows 10 64-bit: Pro, Enterprise, or Education (Build 19041 or higher)
   - OR Windows 11 64-bit
   - WSL 2 feature enabled (Docker installer will help with this)

2. **Download and Install:**
   - Go to [https://www.docker.com/products/docker-desktop/](https://www.docker.com/products/docker-desktop/)
   - Click "Download for Windows"
   - Run the `Docker Desktop Installer.exe` file
   - Follow the installation wizard:
     - Check "Use WSL 2 instead of Hyper-V" (recommended)
     - Complete installation and restart when prompted

3. **First Launch:**
   - Start Docker Desktop from Start Menu
   - Accept the service agreement
   - You may need to enable WSL 2 if prompted

**For macOS:**
1. **System Requirements Check:**
   - macOS 11.0 or newer
   - Apple chip (M1/M2) or Intel chip supported

2. **Download and Install:**
   - Go to [https://www.docker.com/products/docker-desktop/](https://www.docker.com/products/docker-desktop/)
   - Click "Download for Mac" 
   - Choose your chip type (Apple Silicon or Intel)
   - Open the downloaded `.dmg` file
   - Drag Docker.app to Applications folder
   - Launch Docker from Applications

3. **First Launch:**
   - Docker will request privileged access (enter your password)
   - Accept the service agreement
   - Complete the tutorial or skip it

#### Verification:
**Both Windows and macOS (Terminal/Command Prompt):**
```bash
docker --version
docker run hello-world
```

**Expected result:** 
- Docker version number displays (e.g., "Docker version 24.0.x")
- "Hello from Docker!" message appears after pulling and running the test container
