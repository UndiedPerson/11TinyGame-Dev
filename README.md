# README - Windows 11 Custom (Tiny11 Base)

นี่คือไฟล์ Readme สำหรับ Windows 11 ที่ได้รับการปรับแต่งโดยใช้ NTLite โดยมีพื้นฐานมาจาก Tiny11 โดยเน้นการลดขนาดและปรับปรุงประสิทธิภาพการทำงาน

## การปรับแต่งหลัก

* **ลบส่วนประกอบที่ไม่จำเป็น:** ได้ลบแอปและส่วนประกอบของ Windows ที่ไม่จำเป็นออกไปหลายรายการ เช่น Clipchamp, Bing News, Get Help, Solitaire Collection, Sticky Notes, Paint, Power Automate, Photos, Alarms, Calculator, Camera, Feedback Hub, Notepad, Sound Recorder, Terminal, Xbox Components และ Phone Link เป็นต้น เพื่อลดขนาดและลดภาระการทำงานของระบบ
* **คงไว้ซึ่งฟีเจอร์สำคัญ:** ฟีเจอร์ที่จำเป็นสำหรับการใช้งานพื้นฐานและสำหรับนักพัฒนาบางส่วนยังคงถูกเปิดใช้งาน เช่น Bluetooth, USB Camera, File Sharing, Network Discovery, Printing, Scanning, SFC (System File Checker), Default Fonts, TeamViewer, USB Modem/USB Support, Video Playback, Activation (KMS และปกติ), Windows Setup, Windows Store และ Windows Update เพื่อให้ยังคงใช้งานได้หลากหลายและอัปเดตได้
* **รองรับ .NET Framework 3.5 และ WSL:** มีการเปิดใช้งาน .NET Framework 3.5 และ Windows Subsystem for Linux (WSL) เพื่อรองรับแอปพลิเคชันและเครื่องมือที่ต้องการ
* **การตั้งค่า Unattended Installation:** ไฟล์นี้ถูกตั้งค่าสำหรับการติดตั้งแบบ Unattended ซึ่งจะช่วยให้กระบวนการติดตั้ง Windows ทำงานได้โดยอัตโนมัติ โดยที่ Product Key ยังคงต้องใส่ด้วยตนเองในระหว่างหรือหลังการติดตั้ง
* **ปิดการตรวจสอบระบบ (Bypass System Requirement Check):** มีการตั้งค่าใน Registry เพื่อข้ามการตรวจสอบข้อกำหนดขั้นต่ำของ Windows 11 สำหรับ TPM 2.0, Secure Boot, RAM, Storage และ Processor (CPU) ทำให้สามารถติดตั้งบนฮาร์ดแวร์ที่ไม่รองรับได้อย่างง่ายดาย
#If BypassCPUCheck not work  You should fix add regedit when install at HKEY_LOCAL_MACHINE\SYSTEM\Setup\LabConfig Also set value to 1
---

# README - Windows 11 Custom (Tiny11 Base)

This Readme file is for a customized Windows 11 image, based on Tiny11 and optimized using NTLite, focusing on reducing size and improving performance.

## Key Customizations

* **Removed Unnecessary Components:** Numerous Windows applications and components have been removed, such as Clipchamp, Bing News, Get Help, Solitaire Collection, Sticky Notes, Paint, Power Automate, Photos, Alarms, Calculator, Camera, Feedback Hub, Notepad, Sound Recorder, Terminal, Xbox Components, and Phone Link. This reduces the image size and system overhead.
* **Retained Essential Features:** Key features crucial for basic functionality and some developer tools remain enabled. These include Bluetooth, USB Camera, File Sharing, Network Discovery, Printing, Scanning, SFC (System File Checker), Default Fonts, TeamViewer, USB Modem/USB Support, Video Playback, Activation (KMS and regular), Windows Setup, Windows Store, and Windows Update. This ensures broad usability and update capabilities.
* **.NET Framework 3.5 and WSL Support:** .NET Framework 3.5 and Windows Subsystem for Linux (WSL) are enabled to support various applications and tools.
* **Unattended Installation Setup:** This file is configured for unattended installation, streamlining the Windows setup process. The Product Key still needs to be entered manually during or after installation.
* **Bypassed System Requirement Checks:** Registry settings have been added to bypass Windows 11's minimum system requirements for TPM 2.0, Secure Boot, RAM, Storage, and Processor (CPU). This facilitates installation on unsupported hardware.
