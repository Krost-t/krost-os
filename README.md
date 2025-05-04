# Krost-OS 🖥️

> **Krost-OS** is a minimal operating system developed **from scratch** in **C** and **x86 assembly**, featuring a basic graphical interface, PS/2 keyboard and mouse support, and an interactive terminal.

![Build Status](https://img.shields.io/badge/build-passing-brightgreen) ![License](https://img.shields.io/badge/license-AGPL%20v3.0-blue)

---

## Presentation 📖

Krost-OS is an academic and personal project to build an operating system from the ground up, running in a virtual machine environment (QEMU/VM) without network connectivity.

---

## Features ✨

* **Bootloader & Kernel**: Boot via GRUB Multiboot, hand off from assembly to a custom C kernel.
* **Memory Management**: Static allocation and protected-mode paging.
* **I/O Drivers**: PS/2 keyboard & mouse, VGA text (80×25) and basic graphics (320×200, 256 colors).
* **Interactive Terminal**: Simple shell with commands (`ls`, `cat`, `echo`, `help`) and basic redirection.
* **Graphical Interface**: Basic windows, focus handling, and a status bar in VGA mode.
* **Cooperative Multitasking**: Scheduler for switching between processes.

---

## Architecture 🏗️

```bash
krost-os/
├─ boot/          # Assembly bootloader + grub.cfg
├─ kernel/        # Custom C kernel: scheduler, memory manager
├─ drivers/       # PS/2 keyboard & mouse, VGA, PIT, disk drivers
├─ fs/            # FAT12-like filesystem support
├─ shell/         # Shell and built-in utilities
├─ Makefile       # Build targets: all, run, clean
└─ README.md      # Project documentation
```

---

## Technologies Used 🛠️

* **Languages**: C (GNU GCC), x86 Assembly (NASM)
* **Boot**: GRUB Multiboot protocol
* **Virtualization**: QEMU/KVM
* **Build System**: Make
* **Debug**: GDB for kernel and user-space debugging

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

1. **Boot**: Launches automatically under QEMU.
2. **Terminal**: Prompt `krost-shell> ` for commands.
3. **Graphics**: Press `F1` to switch into VGA graphical mode.
4. **Mouse**: PS/2 support for cursor movement and window interaction.

---

## Possible Improvements 🔧

* **Preemptive multitasking** with priorities and synchronization.
* **Advanced filesystem** (ext2-like) with journaling.
* **Network drivers** for Ethernet or Wi-Fi.
* **Enhanced GUI**: 2D rendering, font rendering, theming.
* **Security enhancements**: memory protection, ACLs, ASLR.

---

## Contribution 🤝

Contributions and feedback are welcome:

1. Fork the repository
2. Create a branch: `git checkout -b feature/xyz`
3. Commit changes: `git commit -m "Add <feature>"`
4. Push branch: `git push origin feature/xyz`
5. Open a Pull Request

---

## License 📜

This project is licensed under the **GNU Affero General Public License v3.0**. See [LICENSE](LICENSE) for details.

---

## Contact 📫

Christ Matsanga
✉️ [christ.matsanganzoulou@gmail.com](mailto:christ.matsanganzoulou@gmail.com)
🔗 [GitHub](https://github.com/Krost-t)
