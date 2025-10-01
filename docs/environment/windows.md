# Windows Development Setup Guide

This guide will help you set up a basic development environment on Windows.

## Step 1: Install Node Version Manager (NVM) for Windows

`nvm` (Node Version Manager) allows you to manage multiple versions of Node.js on your system. Follow these steps to install `nvm` for Windows:

1. Visit the [nvm for Windows GitHub page](https://github.com/coreybutler/nvm-windows).
2. Download the latest release from the "Releases" section. Look for the `nvm-setup.zip` or `nvm-setup.exe` file.
3. Extract the downloaded `.zip` file and/or run the `nvm-setup.exe` installer.
4. Follow the installation prompts and complete the setup.

### Verifying the Installation

1. Open a new Command Prompt or PowerShell window.
2. Run the following command to verify that `nvm` is installed:

   ```bash
   nvm -v
   ```

If installed correctly, this will display the installed version of `nvm`.

## Step 2: Install Node.js Using NVM

1. To install a specific version of Node.js, use the following command and replace `<version>` with a specific version (e.g., `16.20.0`), `latest`, or `lts`:

    ```bash
    nvm install <version>
    ```
2. Use the installed version by running:
    ```bash
    nvm use <version>
    ```

3. Verify the active Node.js version:
    ```bash
    node -v
    ```
This should display the version you just installed.

## Step 3: Additional Tools
- **Code Editor**: Download and install [Visual Studio Code](https://code.visualstudio.com/).
- **Git**: Install [Git for Windows](https://gitforwindows.org/) for version control.

## Step 4: Configure Environment Variables

To ensure that `nvm` and `Node.js` work correctly, you may need to update your system's `PATH` environment variable.

### Steps to Update Environment Variables

1. Open the **Start Menu** and search for `Environment Variables`. Select **Edit the system environment variables**.
2. In the **System Properties** window, click the **Environment Variables** button.
3. Under **System Variables**, locate the `Path` variable and click **Edit**.
4. Ensure the following paths are added to the `Path` variable:
   - The directory where `nvm` is installed (e.g., `C:\Program Files\nvm`).
   - The directory where `Node.js` versions are installed (e.g., `C:\Program Files\nvm\v<version>`).

   If these paths are missing, add them manually:
   - Click **New** and enter the path for `nvm`.
   - Click **New** again and enter the path for the active `Node.js` version.

5. Click **OK** to save your changes and close all windows.

### Verifying the Configuration

1. Open a new Command Prompt or PowerShell window.
2. Run the following commands to ensure `nvm` and `Node.js` are accessible:
   ```bash
   nvm -v
   node -v
   npm -v
   ```

## Step 5: Troubleshooting Tips

If you encounter issues during setup, here are some common solutions:

- **`nvm` commands are not recognized**:
  - Ensure the `nvm` installation directory is correctly added to the `PATH` variable.
  - Restart your Command Prompt or PowerShell after making changes to the `PATH` variable.

- **Node.js is not working after installation**:
  - Verify that the correct Node.js version is active by running `nvm use <version>`.
  - Check that the Node.js installation directory is included in the `PATH` variable.

- **Permission issues**:
  - Run your Command Prompt or PowerShell as an administrator if you encounter permission errors.

You're now ready to start developing on Windows!
