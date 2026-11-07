# op8pro-hakios-ci

HakiOS OnePlus 8 Pro (IN2020 / SM8250) CI: assembles the HakiOS common tree with the
[device port](https://github.com/ilmilm/hakios-oneplus8pro), builds the XNU kernel with the
`oneplus8pro` configuration, builds the open-profile loader, and runs the full chain
(U-Boot → xnuloader → XNU → `hello` user space) as a QEMU smoke test.

Artifacts: `hakios-kernel`, `payload-op8pro-open.bin` (fastboot-bootable via the U-Boot route once
the sm8250 device tree port lands), QEMU log.
