# Hyojun Jo (조효준)

> **Principal Systems Architect & Infrastructure Engineer**  
> Architecting high-performance systems software, zero-driver network telemetry, and memory-safe concurrent runtimes.

---

### 🌐 Language Navigation (10 Languages)

| 🇰🇷 [한국어](#korean) | 🇺🇸 [English](#english) | 🇯🇵 [日本語](#japanese) | 🇨🇳 [简体中文](#chinese) | 🇪🇸 [Español](#spanish) |
| :---: | :---: | :---: | :---: | :---: |
| 🇫🇷 [Français](#french) | 🇩🇪 [Deutsch](#german) | 🇷🇺 [Русский](#russian) | 🇸🇦 [العربية](#arabic) | 🇮🇳 [हिन्दी](#hindi) |

---

<a id="english"></a>
## ⚡ Executive Overview

I am **Hyojun Jo** — a systems software engineer and infrastructure architect dedicated to low-level engineering, deterministic runtimes, and high-performance network telemetry.

My engineering practice is grounded in **fundamental computing principles**:
- Eliminating driver dependency by building user-mode telemetry engines directly atop Windows Filtering Platform (WFP) and Linux eBPF.
- Designing high-concurrency, memory-safe network pipelines utilizing zero-copy ring buffers and strict ownership invariants in Rust and Go.
- Enforcing orthodox software standards: standard-library-first design, deterministic state machines, and zero-leak resource lifecycles.

---

<a id="korean"></a>
## 🏛️ 엔지니어링 철학 및 핵심 원칙 (Core Principles)

```yaml
engineer:
  name: Hyojun Jo (조효준)
  role: Principal Systems Architect & Infrastructure Engineer
  location: Seoul, Republic of Korea
  disciplines:
    - "Orthodox Engineering: Standard libraries before bloated dependencies"
    - "Zero Driver: Pure user-mode WFP & eBPF over invasive kernel drivers"
    - "Deterministic Lifecycles: Leak-free memory and strict RAII resource ownership"
    - "Zero-Copy Concurrency: Microsecond-latency event loops and ring buffers"
```

1. **정통파 시스템 엔지니어링 (Orthodox Systems Engineering)**:
   - 과도한 서드파티 의존성을 지양하고, 운영체제 네이티브 API와 제1원리(First-Principles)에 기반하여 장기적인 유지보수성과 견고성을 보장합니다.
2. **비침습적 커널 텔레메트리 (Zero-Driver Telemetry)**:
   - 외부 커널 드라이버(Npcap 등) 설치 없이 OS 기본 필터링 엔진(WFP/eBPF)을 직접 제어하여 시스템 안정성과 보안 무결성을 극대화합니다.
3. **결정론적 상태 관리 및 메모리 안전성 (Deterministic State & Memory Safety)**:
   - RAII 패턴과 소유권 모델을 엄격히 적용하여 메모리 누수, 리소스 고갈, 교착 상태(Deadlock)를 원천 배제합니다.

---

## 🛠️ Comprehensive Technology Stack

| 계층 (Domain) | 핵심 기술 및 프레임워크 (Core Stack) |
| :--- | :--- |
| **Languages & Runtimes** | `Rust`, `Go`, `C/C++17`, `TypeScript`, `Node.js (v20+)`, `Python 3.12`, `PowerShell Core` |
| **Network & Telemetry** | `Windows Filtering Platform (WFP)`, `Linux eBPF`, `Raw Sockets`, `Zero-Copy RingBuffer` |
| **Protocols & Concurrency** | `gRPC`, `HTTP/2 & HTTP/3 (QUIC)`, `WebSocket`, `Protocol Buffers`, `JSON-RPC 2.0` |
| **Security & Cryptography** | `Windows DPAPI`, `X25519 (age)`, `Ed25519 (minisign)`, `Constant-Time Crypto`, `Memory Wipe` |
| **Infrastructure & CI/CD** | `GitHub Actions`, `GitLab CI/CD`, `Linux Systemd Daemons`, `Multi-Platform Packaging` |

---

## 📂 Key Architecture & Open-Source Projects

### 🌐 `netvibe` — Zero-Driver Process Network Telemetry
- **Overview**: Pure Rust 기반의 고성능 네트워크 패킷 분석 및 트래픽 셰이핑 엔진.
- **Key Features**:
  - Wireshark/Npcap 설치 없이 특정 PID 프로세스의 소켓 트래픽만 무침습적으로 정밀 격리 캡처.
  - Zero-Copy RingBuffer 구조를 통한 마이크로초 단위 저지연 및 최소 CPU 오버헤드 달성.
  - REST/gRPC 트랜잭션 흐름 분석 및 정규화 명세 자동 추출 지원.

### 🛡️ `sys-guard` — Deterministic System Daemon & Process Supervisor
- **Overview**: 저수준 프로세스 수명주기 감시 및 보안 무결성 검증 런타임.
- **Key Features**:
  - 비동기 이벤트 루프 기반의 실시간 시스템 리소스 할당량(Quota) 제어.
  - 프로세스 좀비화 방지 및 리소스 누수 없는 클린 셧다운 라이프사이클 보장.

---

<a id="japanese"></a>
### 🇯🇵 日本語概要
システムの堅牢性と決定論的なランタイム設計を追求するシステムアーキテクトです。Rust、Go、WFP/eBPF技術を活用し、不要な依存関係を排除した高性能でセキュアなインフラソフトウェアを構築しています。

<a id="chinese"></a>
### 🇨🇳 中文概述
专注于高可靠性、高性能系统架构与内存安全工程的资深系统架构师。使用 Rust、Go 与底层操作系统原语（WFP、eBPF），构建无驱动网络遥测与高性能并发基础设施。

<a id="spanish"></a>
### 🇪🇸 Resumen en Español
Arquitecto de sistemas enfocado en infraestructura de alto rendimiento, telemetría de red sin controladores y software de sistemas seguro en memoria mediante Rust, Go y primitivas del sistema operativo.

<a id="french"></a>
### 🇫🇷 Résumé en Français
Architecte de systèmes dédié aux infrastructures logicielles haute performance, à la télémétrie réseau sans pilote et à la sécurité mémoire avec Rust, Go et les primitives système de bas niveau.

<a id="german"></a>
### 🇩🇪 Deutsche Zusammenfassung
Leitender Systemarchitekt für hochperformante Softwareinfrastruktur, treiberlose Netzwerktelemetrie und speichersichere Systeme mit Rust, Go und systemnahen Betriebssystemprimitiven.

<a id="russian"></a>
### 🇷🇺 Кратко на русском
Ведущий системный архитектор, специализирующийся на высокопроизводительной инфраструктуре, безинтерфейсной сетевой телеметрии и безопасном системном программировании на Rust и Go.

<a id="arabic"></a>
### 🇸🇦 نبذة بالعربية
مهندس معماري لأنظمة البرمجيات عالية الأداء ومقاييس الشبكات بدون برامج تشغيل، متخصص في هندسة النظم الآمنة للذاكرة والتطوير منخفض المستوى باستخدام Rust وGo.

<a id="hindi"></a>
### 🇮🇳 हिन्दी सारांश
उच्च-प्रदर्शन 시스템 इंफ्रास्ट्रक्चर, बिना ड्राइवर के नेटवर्क टेलीमेट्री और मेमोरी-सुरक्षित 시스템 सॉफ्टवेयर में विशेषज्ञता प्राप्त 시스템 आर्किटेक्ट। Rust और Go का उपयोग करके सुरक्षित और कुशल प्लेटफॉर्म का निर्माण।

---

## 📬 Connectivity & Platforms

- **GitHub**: [github.com/jo060235354-design](https://github.com/jo060235354-design)
- **GitLab**: [gitlab.com/jo060235354](https://gitlab.com/jo060235354)
- **Hugging Face**: [huggingface.co/sfmiko](https://huggingface.co/sfmiko)
- **Direct Mail**: `jo060235354@gmail.com`
