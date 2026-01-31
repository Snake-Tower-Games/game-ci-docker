ARG baseImage="unityci/base:windows-latest"

FROM $baseImage

# Install unity hub
RUN choco install unity-hub --no-progress -y

SHELL ["powershell", "-Command"]

# Install Unity Editor with Linux and Mac Mono build support
RUN & 'C:\Program Files\Unity Hub\Unity Hub.exe' -- --headless install --version 6000.0.58f2 -m linux-mono -m mac-mono
