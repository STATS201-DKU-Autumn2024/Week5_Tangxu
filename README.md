# System Configuration Report

### CPU Information:
- **Architecture:** x86_64
- **CPU op-mode(s):** 32-bit, 64-bit
- **Address sizes:** 46 bits physical, 48 bits virtual
- **Byte Order:** Little Endian
- **CPU(s):** 2
- **On-line CPU(s) list:** 0,1
- **Vendor ID:** GenuineIntel
- **Model name:** Intel(R) Xeon(R) CPU @ 2.20GHz
- **CPU family:** 6
- **Model:** 79
- **Thread(s) per core:** 2
- **Core(s) per socket:** 1
- **Socket(s):** 1
- **Stepping:** 0
- **BogoMIPS:** 4400.29
- **Flags:** fpu, vme, de, pse, tsc, msr, pae, mce, cx8, apic, sep, mtrr, pge, mca, cmov, pat, pse36, clflush, mmx, fxsr, sse, sse2, ss, ht, syscall, nx, pdpe1gb, rdtscp, lm, constant_tsc, rep_good, nopl, xtopology, nonstop_tsc, cpuid, tsc_known_freq, pni, pclmulqdq, ssse3, fma, cx16, pcid, sse4_1, sse4_2, x2apic, movbe, popcnt, aes, xsave, avx, f16c, rdrand, hypervisor, lahf_lm, abm, 3dnowprefetch, invpcid_single, ssbd, ibrs, ibpb, stibp, fsgsbase, tsc_adjust, bmi1, hle, avx2, smep, bmi2, erms, invpcid, rtm, rdseed, adx, smap, xsaveopt, arat, md_clear, arch_capabilities
- **Hypervisor vendor:** KVM
- **Virtualization type:** full
- **L1d cache:** 32 KiB (1 instance)
- **L1i cache:** 32 KiB (1 instance)
- **L2 cache:** 256 KiB (1 instance)
- **L3 cache:** 55 MiB (1 instance)
- **NUMA node(s):** 1
- **NUMA node0 CPU(s):** 0,1

### Vulnerabilities:
- **Gather data sampling:** Not affected
- **Itlb multihit:** Not affected
- **L1tf:** Mitigation; PTE Inversion
- **Mds:** Vulnerable; SMT Host state unknown
- **Meltdown:** Vulnerable
- **Mmio stale data:** Vulnerable
- **Reg file data sampling:** Not affected
- **Retbleed:** Vulnerable
- **Spec rstack overflow:** Not affected
- **Spec store bypass:** Vulnerable
- **Spectre v1:** Vulnerable: __user pointer sanitization and usercopy barriers only; no swapgs barriers
- **Spectre v2:** Vulnerable; IBPB: disabled; STIBP: disabled; PBRSB-eIBRS: Not affected; BHI: Vulnerable (Syscall hardening enabled)
- **Srbds:** Not affected
- **Tsx async abort:** Vulnerable

### GPU Information:
- No GPU found

### Memory Information:
- **Total:** 12 GiB
- **Used:** 805 MiB
- **Free:** 7.9 GiB
- **Shared:** 1.0 MiB
- **Buffer/Cache:** 4.0 GiB
- **Available:** 11 GiB
- **Swap:** Not enabled

### Disk Space:
| Filesystem | Size | Used | Available | Use% | Mounted on |
|------------|------|------|-----------|------|------------|
| overlay    | 108G | 38G  | 71G       | 35%  | /          |
| tmpfs      | 64M  | 0B   | 64M       | 0%   | /dev       |
| shm        | 5.8G | 0B   | 5.8G      | 0%   | /dev/shm   |
| /dev/root  | 2.0G | 1.2G | 820M      | 59%  | /usr/sbin/docker-init |
| tmpfs      | 6.4G | 128K | 6.4G      | 1%   | /var/colab |
| /dev/sda1  | 77G  | 57G  | 20G       | 74%  | /etc/hosts |
| tmpfs      | 6.4G | 0B   | 6.4G      | 0%   | /proc/acpi |
| tmpfs      | 6.4G | 0B   | 6.4G      | 0%   | /proc/scsi |
| tmpfs      | 6.4G | 0B   | 6.4G      | 0%   | /sys/firmware |

### Python Version:
- **Python 3.10.12**

### Installed Packages:
| Package              | Version  |
|----------------------|----------|
| absl-py              | 1.4.0    |
| accelerate           | 0.34.2   |
| aiohappyeyeballs     | 2.4.3    |
| aiohttp              | 3.10.10  |
| aiosignal            | 1.3.1    |
| alabaster            | 0.7.16   |
| albucore             | 0.0.16   |
| albumentations       | 1.4.15   |
| altair               | 4.2.2    |
| annotated-types      | 0.7.0    |
| anyio                | 3.7.1    |
| argon2-cffi          | 23.1.0   |
| argon2-cffi-bindings | 21.2.0   |
| array_record         | 0.5.1    |
| arviz                | 0.19.0   |
| ...                  | ...      |
| werkzeug             | 3.0.4    |
| wheel                | 0.44.0   |
| widgetsnbextension   | 3.6.10   |
| wordcloud            | 1.9.3    |
| wrapt                | 1.16.0   |
| xarray               | 2024.9.0 |
| xgboost              | 2.1.1    |
| yfinance             | 0.2.46   |
| zipp                 | 3.20.2   |
