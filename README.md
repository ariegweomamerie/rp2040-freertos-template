# 📦 RP2040 FreeRTOS Project Template

A professional, ready-to-use **CMake + FreeRTOS project template** for the **Raspberry Pi Pico** (RP2040).  
This template is designed to help you quickly start real-time operating system (RTOS) projects on the RP2040 using FreeRTOS and the Pico SDK.

---

## ✨ Features

- 🧩 FreeRTOS integrated with Raspberry Pi Pico SDK
- 📁 Organized project structure (source, include, CMake)
- 🛠 Build system based on CMake
- 🧹 Clean and minimal, easy to extend
- 🚀 Ready for multitasking, concurrency, semaphores, queues, mutexes, etc.
- 🛡️ Designed for professional robotics, IoT, and embedded systems projects

---

## 📚 Project Structure

```plaintext
rp2040-freertos-template/
├── CMakeLists.txt       # Top-level CMake build file
├── src/                 # Source code (.c files)
├── include/             # Header files (.h files)
├── freertos/            # FreeRTOS kernel source
├── build/               # (created automatically after building)
├── README.md            # This file
└── .gitignore           # Git ignored files/folders


🛠 Built With
FreeRTOS

Raspberry Pi Pico SDK

CMake

GCC ARM toolchain

. Clone the repository

git clone https://github.com/ariegweomamerie/rp2040-freertos-template.git
cd rp2040-freertos-template
2. Prepare the Pico SDK (if not done already)

git clone https://github.com/raspberrypi/pico-sdk.git
cd pico-sdk
git submodule update --init
Then set the PICO_SDK_PATH environment variable or link the SDK properly in CMake.

3. Build the project

mkdir build
cd build
cmake ..
make
You will get a .uf2 file ready to flash to your Raspberry Pi Pico!

📦 Flash to Pico
Press and hold the BOOTSEL button while plugging in the Pico to your computer.

Drag and drop the generated .uf2 file into the mounted USB storage.

OR use picotool for flashing:

picotool load your_program.uf2
📄 License
This project is licensed under the MIT License.
Feel free to use, modify, and share!


