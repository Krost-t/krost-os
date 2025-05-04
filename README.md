# Krost-OS 🖥️

> **Krost-OS** is a Unix-like operating system developed **from scratch** in **C** and **x86 assembly**, featuring a basic graphical interface, PS/2 keyboard and mouse support, and an interactive terminal.

![Build Status](https://img.shields.io/badge/build-passing-brightgreen) ![License](https://img.shields.io/badge/license-AGPL%20v3.0-blue)

---

## Presentation 📖

Krost-OS is an academic and personal project aiming to rebuild an operating system from the ground up, without network connectivity, inspired by Unix architecture and running in a virtual environment (QEMU/VM).

---

## Features ✨

* **Bootloader & Kernel**: Start via GRUB Multiboot, transition from assembly bootloader to a monolithic C kernel.
* **Memory Management**: Static allocation, paging, and protection in protected mode.
* **I/O Drivers**: PS/2 keyboard & mouse, VGA text (80×25) and graphics mode (320×200, 256 colors), FAT12-like disk access.
* **Interactive Terminal**: A simple shell implementing commands (`ls`, `cat`, `echo`, `help`) with basic redirections.
* **Basic GUI**: Simple window rectangles, focus management, and a status bar.
* **Cooperative Multitasking**: A scheduler for context switching between user processes.

---

## Architecture 🏗️

```bash
krost-os/
├─ boot/          # Bootloader (assembly) + grub.cfg
├─ kernel/        # C kernel: syscalls, scheduler, memory management
├─ drivers/       # Keyboard, mouse, VGA, PIT, disk drivers
├─ fs/            # FAT12-like filesystem implementation
├─ shell/         # Shell and utility programs
├─ Makefile       # Build targets: all, run, clean
└─ README.md      # Project documentation
```

---

## Technologies Used 🛠️

* **Languages**: C (GNU GCC), x86 Assembly (NASM)
* **Boot**: GRUB Multiboot protocol
* **Virtualization**: QEMU/KVM
* **Build System**: Make
* **Debug**: GDB for kernel and user processes

---

## Installation & Execution ⚙️

```bash
# Clone the repository
git clone https://github.com/Krost-t/krost-os.git
cd krost-os

# Build the project
make all

# Run Krost-OS in QEMU
make run
```

> **Prerequisites**: `nasm`, `gcc`, `grub2`, `qemu-system-x86_64`, `make`.

---

## Usage 🚀

1. **Boot**: QEMU automatically loads Krost-OS.
2. **Terminal**: Use the `krost-shell> ` prompt to enter commands.
3. **Graphics**: Press `F1` to switch to VGA graphics mode.
4. **Mouse**: PS/2 emulation to move the cursor and click windows.

---

## Possible Improvements 🔧

* **Preemptive multitasking** with priority scheduling and synchronization primitives (mutex, semaphore).
* **Advanced filesystem** (ext2-like) with journaling support.
* **Network drivers** for Ethernet or Wi-Fi connectivity.
* **Enhanced GUI**: 2D rendering engine, font support, theming.
* **Security features**: memory protection, ACLs, address space layout randomization (ASLR).

---

## Contribution 🤝

Contributions and feedback are welcome!

1. Fork the repository.
2. Create a branch: `git checkout -b feature/your-feature`.
3. Commit your changes: `git commit -m "Add <feature>"`.
4. Push to your branch: `git push origin feature/your-feature`.
5. Open a Pull Request.

---

## License 📜

This project is licensed under the **GNU Affero General Public License v3.0**. See [LICENSE](LICENSE) for details.

---

## Contact 📫

Christ Matsanga
✉️ [christ.matsanganzoulou@gmail.com](mailto:christ.matsanganzoulou@gmail.com)
🔗 [GitHub](https://github.com/Krost-t)
