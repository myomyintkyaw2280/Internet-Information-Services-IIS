# Internet-Information-Services-IIS

## Enable or Disable IIS Server

To enable or disable IIS (Internet Information Services) on Windows, follow these methods:

## Enable IIS Server

### Using Windows Features
1. Press `Win + R`, type `appwiz.cpl`, and press `Enter`.
2. Click **Turn Windows features on or off** (on the left panel).
3. Scroll down and check **Internet Information Services (IIS)**.
4. Click **OK** and wait for the installation to complete.
5. Restart your computer if prompted.

### Using Command Prompt (Admin)
1. Open **Command Prompt as Administrator**.
2. Run:
   ```bash
   dism /online /enable-feature /featurename:IIS-WebServer /all
   ```
3. Wait for the process to complete and restart if required.

---

## Disable IIS Server

### Using Windows Features
1. Press `Win + R`, type `appwiz.cpl`, and press `Enter`.
2. Click **Turn Windows features on or off**.
3. Uncheck **Internet Information Services (IIS)**.
4. Click **OK** and restart your system if necessary.

### Using Command Prompt (Admin)
1. Open **Command Prompt as Administrator**.
2. Run:
   ```bash
   dism /online /disable-feature /featurename:IIS-WebServer
   ```
3. Restart your system.

---

## Start or Stop IIS Services

### Using Command Prompt (Admin)
- **Start IIS**:
  ```sql
  net start W3SVC
  ```
- **Stop IIS**:
  ```arduino
  net stop W3SVC
  ```
- **Restart IIS**:
  ```nginx
  iisreset
  ```

Let me know if you need further help! 🚀
