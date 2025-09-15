# Automated-Flutter-Installation-Script - DRAFT

## Purpose
```
The goal of this
project is to simplify
flutter in the shell
and to make the
build process platform- independent
via command, so that
you can generate the
corresponding iOS and Android
APK on a Mac
or Windows/Linux computer.
```

## Notes for further processing
```
sudo apt-get update -y && sudo apt-get upgrade -y;
sudo apt-get install -y curl git unzip xz-utils zip libglu1-mesa
sudo apt-get install libc6:amd64 libstdc++6:amd64 lib32z1 libbz2-1.0:amd64
wget https://storage.googleapis.com/flutter_infra_release/releases/stable/linux/flutter_linux_3.35.3-stable.tar.xz
https://docs.flutter.dev/install/archive
cd ~/development/
tar -xf ~/Downloads/flutter_linux_3.35.3-stable.tar.xz -C ~/development/
echo $SHELL
echo $0
echo 'export PATH="$HOME/development/flutter/bin:$PATH"' >> ~/.bash_profile
Android SDK Platform, API 35
Android SDK Command-line Tools
Android SDK Build-Tools
Android SDK Platform-Tools
Android Emulator
flutter doctor --android-licenses
flutter doctor
flutter doctor -v

sudo softwareupdate --install-rosetta --agree-to-license
https://storage.googleapis.com/flutter_infra_release/releases/stable/macos/flutter_macos_arm64_3.35.3-stable.zip
https://storage.googleapis.com/flutter_infra_release/releases/stable/macos/flutter_macos_3.35.3-stable.zip
unzip ~/Downloads/flutter_macos_arm64_3.35.3-stable.zip -d ~/development/
export PATH=$HOME/development/flutter/bin:$PATH
~/.zshenv
install Xcode
sudo sh -c 'xcode-select -s /Applications/Xcode.app/Contents/Developer && xcodebuild -runFirstLaunch'
sudo xcodebuild -license
xcodebuild -downloadPlatform iOS
open -a Simulator
sudo gem install cocoapods
export PATH=$HOME/.gem/bin:$PATH
flutter doctor
flutter doctor
flutter doctor -v

https://storage.googleapis.com/flutter_infra_release/releases/stable/windows/flutter_windows_3.35.3-stable.zip
%USERPROFILE% (C:\Users\{username}) or %LOCALAPPDATA% (C:\Users\{username}\AppData\Local
PS C:\> Expand-Archive `
-Path $env:USERPROFILE\Downloads\flutter_windows_3.35.3-stable.zip `
-Destination $env:USERPROFILE\dev\
PS C:\> Expand-Archive `
-Path $env:USERPROFILE\Downloads\flutter_windows_3.35.3-stable.zip `
-Destination $env:USERPROFILE\dev\
%USERPROFILE%\dev\flutter
%USERPROFILE%\dev\flutter\bin
%USERPROFILE%\dev\flutter\bin
flutter doctor --android-licenses

https://dl.google.com/android/repository/commandlinetools-win-13114758_latest.zip?hl=de
https://dl.google.com/android/repository/commandlinetools-mac-13114758_latest.zip?hl=de
https://dl.google.com/android/repository/commandlinetools-linux-13114758_latest.zip?hl=de

export ANDROID_HOME=~/Android/sdk
export PATH=$PATH:$ANDROID_HOME/cmdline-tools/latest/bin:$ANDROID_HOME/platform-tools
source ~/.bashrc
~/.zshrc
sdkmanager --update
sdkmanager --licenses -y

sdkmanager "platform-tools"  # Android SDK Platform-Tools (ADB, Fastboot)
sdkmanager "build-tools;35.0.0"  # Android SDK Build-Tools (neueste für API 35; passe Version an, falls nötig)
sdkmanager "platforms;android-35"  # Android SDK Platform, API 35
sdkmanager "emulator"  # Android Emulator
sdkmanager --list | grep build-tools
adb version
sdkmanager "system-images;android-35;google_apis;x86_64
%ANDROID_HOME%\cmdline-tools\latest\bin und %ANDROID_HOME%\platform-tools
ANDROID_HOME = C:\Android\sdk
sdkmanager --list_installed
Linux: commandlinetools-linux-*.zip
macOS: commandlinetools-mac-*.zip
Windows: commandlinetools-win-*.zip
export ANDROID_HOME=~/Android/sdk
export PATH=$PATH:$ANDROID_HOME/cmdline-tools/latest/bin:$ANDROID_HOME/platform-tools
sdkmanager --update
sdkmanager --licenses
kmanager "platform-tools"  # Android SDK Platform-Tools (ADB, Fastboot)
sdkmanager "build-tools;35.0.0"  # Android SDK Build-Tools (neueste für API 35; passe Version an, falls nö
tig)
sdkmanager "platforms;android-35"  # Android SDK Platform, API 35
sdkmanager "emulator"  # Android Emulator

sdkmanager --list_installed
sdkmanager --list | grep build-tools
sdkmanager "system-images;android-35;google_apis;x86_64"
adb version
aapt version
$ANDROID_HOME/build-tools/35.0.0/
emulator -list-avds
avdmanager create avd -n TestDevice -k "system-images;android-35;google_apis;x86_64"
emulator -avd TestDevice
sudo apt update && sudo apt install libc6:i386 libncurses5:i386 libstdc++6:i386 lib32z1 openjdk-17-jdk.
sudo apt install libc6-dev-i386.
sudo apt install qemu-kvm libvirt-clients libvirt-daemon-system bridge-utils und füge User zur kvm-Gruppe 
hinzu: sudo usermod -aG kvm $USER.

linux
sudo apt update && sudo apt install libc6:i386 libncurses5:i386 libstdc++6:i386 lib32z1 openjdk-17-jdk.
Für 64-Bit: sudo apt install libc6-dev-i386.
Emulator braucht KVM: sudo apt install qemu-kvm libvirt-clients libvirt-daemon-system bridge-utils und füg
e User zur kvm-Gruppe hinzu: sudo usermod -aG kvm $USER.

windows
sdkmanager "extras;intel;Hardware_Accelerated_Execution_Manager"

macOS
Installiere Xcode Command Line Tools: xcode-select --install.
Für Emulator: Aktiviere Hardware-Beschleunigung in den Systemeinstellungen (falls Apple Silicon, verwende 
ARM-Images).
Homebrew-Alternative für Platform-Tools: brew install android-platform-tools (nur für ADB/Fastboot, nicht 
vollständig).

sdkmanager --licenses
sdkmanager --list | grep android-35
sdkmanager --update
```
