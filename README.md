# Telemetrix4Microbit
Telemetrix Servers for the Micro:bit V1 and V2

This project takes advantage of [the docker tool chain](https://github.com/carlosperate/docker-microbit-toolchain)
developed by Carlos Pereira Atencio.

Before attempting to recompile the source code, you must:

1. [Install docker](https://docs.docker.com/desktop/linux/install/) on your system.
2. If using Linux, make docker available to your login:
```asm
sudo usermod -aG docker $USER
```
3. Install the docker tool chain:
```asm
docker pull ghcr.io/carlosperate/microbit-toolchain:latest
```

4. If using Linux, change the permissions of the build scripts:
```asm
cd build_scripts
chmod ugo+x *
```
5. Compile for the desired micro:bit version.
   To build for microbit v1, go to the build scripts directory and type:
```asm
./dal
```

To build for microbit v2, go to build scripts directory and type:
```asm
./codal
```
THIS IS A WORK IN PROGRESS
