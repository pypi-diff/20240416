# Comparing `tmp/dtschema-2024.2.tar.gz` & `tmp/dtschema-2024.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtschema-2024.2.tar", last modified: Tue Feb 27 20:48:02 2024, max compression
+gzip compressed data, was "dtschema-2024.4.tar", last modified: Tue Apr 16 20:30:10 2024, max compression
```

## Comparing `dtschema-2024.2.tar` & `dtschema-2024.4.tar`

### file list

```diff
@@ -1,160 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.184203 dtschema-2024.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.160202 dtschema-2024.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.164203 dtschema-2024.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-02-27 20:47:52.000000 dtschema-2024.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-02-27 20:47:52.000000 dtschema-2024.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-27 20:47:52.000000 dtschema-2024.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-27 20:47:52.000000 dtschema-2024.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-02-27 20:48:02.184203 dtschema-2024.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-02-27 20:47:52.000000 dtschema-2024.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.168202 dtschema-2024.2/dtschema/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1531 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/check_compatible.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2028 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/doc_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14932 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/dtb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1306 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/dtb2py.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5580 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/dtb_validate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1200 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/extract_compatibles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2613 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/extract_example.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1790 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/extract_props.py
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/fixups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.172202 dtschema-2024.2/dtschema/meta-schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/boolean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/cell.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/clocks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/core.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/dma.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/gpios.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/hwlock.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/iio.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/interrupts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/iommu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/items.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/keywords.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/mailbox.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/nodes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/nvmem.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/phy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/power-domain.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/pwm.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/reset.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/string-array.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/meta-schemas/vendor-props.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1326 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/mk_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.176203 dtschema-2024.2/dtschema/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/aliases.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/bootph.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.176203 dtschema-2024.2/dtschema/schemas/bus/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/bus/qemu,platform.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/cache-controller.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/cache.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/chosen.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.176203 dtschema-2024.2/dtschema/schemas/clock/
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/clock/clock.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/cpu-map.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/cpu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/cpus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.176203 dtschema-2024.2/dtschema/schemas/dma/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/dma/dma.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/dt-core.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.176203 dtschema-2024.2/dtschema/schemas/gpio/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/gpio/gpio-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/gpio/gpio-hog.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/gpio/gpio.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/graph.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.180203 dtschema-2024.2/dtschema/schemas/hwlock/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/hwlock/hwlock-consumer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.180203 dtschema-2024.2/dtschema/schemas/i2c/
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/i2c/i2c-controller.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.180203 dtschema-2024.2/dtschema/schemas/iio/
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/iio/iio-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/iio/iio.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/interconnects.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/interrupt-controller.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/interrupts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.180203 dtschema-2024.2/dtschema/schemas/iommu/
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/iommu/iommu.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.180203 dtschema-2024.2/dtschema/schemas/isa/
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/isa/isa-bridge.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/isa/isa-bus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.180203 dtschema-2024.2/dtschema/schemas/mbox/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/mbox/mbox-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/memory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/msi-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/numa-distance-map-v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.180203 dtschema-2024.2/dtschema/schemas/opp/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/opp/opp.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.180203 dtschema-2024.2/dtschema/schemas/options/
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/options/u-boot.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/options.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.180203 dtschema-2024.2/dtschema/schemas/pci/
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/pci/pci-bus-common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/pci/pci-bus.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/pci/pci-device.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/pci/pci-host-bridge.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/pci/pci-iommu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/pci/pci-pci-bridge.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.180203 dtschema-2024.2/dtschema/schemas/phy/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/phy/phy-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/phy/phy-provider.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.180203 dtschema-2024.2/dtschema/schemas/pinctrl/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/pinctrl/pinctrl-consumer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.180203 dtschema-2024.2/dtschema/schemas/power-domain/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/power-domain/power-domain-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/property-units.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.180203 dtschema-2024.2/dtschema/schemas/pwm/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/pwm/pwm-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/reg.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.180203 dtschema-2024.2/dtschema/schemas/reserved-memory/
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/reserved-memory/framebuffer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/reserved-memory/memory-region.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/reserved-memory/reserved-memory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/reserved-memory/shared-dma-pool.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.180203 dtschema-2024.2/dtschema/schemas/reset/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/reset/reset.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/root-node.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/serial.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/simple-bus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.184203 dtschema-2024.2/dtschema/schemas/thermal/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/thermal/thermal.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/schemas/types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17354 2024-02-27 20:47:52.000000 dtschema-2024.2/dtschema/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-02-27 20:48:02.000000 dtschema-2024.2/dtschema/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.184203 dtschema-2024.2/dtschema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-02-27 20:48:02.000000 dtschema-2024.2/dtschema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-02-27 20:48:02.000000 dtschema-2024.2/dtschema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 20:48:02.000000 dtschema-2024.2/dtschema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-27 20:48:02.000000 dtschema-2024.2/dtschema.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-27 20:48:02.000000 dtschema-2024.2/dtschema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-27 20:48:02.000000 dtschema-2024.2/dtschema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-02-27 20:47:52.000000 dtschema-2024.2/example-schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-02-27 20:47:52.000000 dtschema-2024.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 20:48:02.184203 dtschema-2024.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.184203 dtschema-2024.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-02-27 20:47:52.000000 dtschema-2024.2/test/bootphases.dts
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-02-27 20:47:52.000000 dtschema-2024.2/test/child-node-fail.dts
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-02-27 20:47:52.000000 dtschema-2024.2/test/child-node.dts
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-02-27 20:47:52.000000 dtschema-2024.2/test/conditionals-allof-fail.dts
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-27 20:47:52.000000 dtschema-2024.2/test/conditionals-allof-pass.dts
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-27 20:47:52.000000 dtschema-2024.2/test/conditionals-single-fail.dts
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-27 20:47:52.000000 dtschema-2024.2/test/conditionals-single-pass.dts
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-02-27 20:47:52.000000 dtschema-2024.2/test/device-fail.dts
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-02-27 20:47:52.000000 dtschema-2024.2/test/device.dts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.184203 dtschema-2024.2/test/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-02-27 20:47:52.000000 dtschema-2024.2/test/schemas/bad-example.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-02-27 20:47:52.000000 dtschema-2024.2/test/schemas/child-node-example.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-02-27 20:47:52.000000 dtschema-2024.2/test/schemas/conditionals-allof-example.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-02-27 20:47:52.000000 dtschema-2024.2/test/schemas/conditionals-single-example.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-02-27 20:47:52.000000 dtschema-2024.2/test/schemas/good-example.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-27 20:47:52.000000 dtschema-2024.2/test/simple-bus-fail.dts
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-27 20:47:52.000000 dtschema-2024.2/test/simple-bus-pass.dts
--rwxr-xr-x   0 runner    (1001) docker     (127)     5664 2024-02-27 20:47:52.000000 dtschema-2024.2/test/test-dt-validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 20:48:02.184203 dtschema-2024.2/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6206 2024-02-27 20:47:52.000000 dtschema-2024.2/tools/dt-prop-populate
--rwxr-xr-x   0 runner    (1001) docker     (127)     2135 2024-02-27 20:47:52.000000 dtschema-2024.2/tools/yaml-format
--rwxr-xr-x   0 runner    (1001) docker     (127)      766 2024-02-27 20:47:52.000000 dtschema-2024.2/tools/yaml2json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.869605 dtschema-2024.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.849605 dtschema-2024.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.853605 dtschema-2024.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-16 20:30:06.000000 dtschema-2024.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-16 20:30:06.000000 dtschema-2024.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 20:30:06.000000 dtschema-2024.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-16 20:30:06.000000 dtschema-2024.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-04-16 20:30:10.869605 dtschema-2024.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-16 20:30:06.000000 dtschema-2024.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.853605 dtschema-2024.4/dtschema/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1531 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/check_compatible.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2028 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/doc_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15470 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/dtb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1306 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/dtb2py.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5937 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/dtb_validate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1200 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/extract_compatibles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2613 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/extract_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1790 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/extract_props.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/fixups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.857605 dtschema-2024.4/dtschema/meta-schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/boolean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/cell.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/clocks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/core.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/dma.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/gpios.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/hwlock.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/iio.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/interrupts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/iommu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/items.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/keywords.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/mailbox.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/nodes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/nvmem.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/phy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/power-domain.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/pwm.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/reset.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/string-array.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/vendor-props.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1326 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/mk_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.861605 dtschema-2024.4/dtschema/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/aliases.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/bootph.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.861605 dtschema-2024.4/dtschema/schemas/bus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/bus/qemu,platform.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/cache-controller.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/cache.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8432 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/chosen.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.861605 dtschema-2024.4/dtschema/schemas/clock/
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/clock/clock.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/cpu-map.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/cpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/cpus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.861605 dtschema-2024.4/dtschema/schemas/dma/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/dma/dma.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/dt-core.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/gpio/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/gpio/gpio-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/gpio/gpio-hog.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/gpio/gpio.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/graph.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/hwlock/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/hwlock/hwlock-consumer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/i2c/
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/i2c/i2c-controller.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/iio/
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/iio/iio-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/iio/iio.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/interconnects.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/interrupt-controller.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/interrupts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/iommu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/iommu/iommu.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/isa/
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/isa/isa-bridge.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/isa/isa-bus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/mbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/mbox/mbox-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/memory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/msi-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/numa-distance-map-v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/opp/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/opp/opp.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/options/
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/options/u-boot.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/options.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/pci/
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/pci/pci-bus-common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/pci/pci-bus.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/pci/pci-device.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/pci/pci-host-bridge.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/pci/pci-iommu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/pci/pci-pci-bridge.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/phy/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/phy/phy-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/phy/phy-provider.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/pinctrl/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/pinctrl/pinctrl-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/post-init-providers.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/power-domain/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/power-domain/power-domain-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/property-units.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/pwm/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/pwm/pwm-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/reg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.869605 dtschema-2024.4/dtschema/schemas/reserved-memory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/reserved-memory/framebuffer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/reserved-memory/memory-region.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/reserved-memory/reserved-memory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/reserved-memory/shared-dma-pool.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.869605 dtschema-2024.4/dtschema/schemas/reset/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/reset/reset.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/root-node.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/serial.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/simple-bus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.869605 dtschema-2024.4/dtschema/schemas/thermal/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/thermal/thermal.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    18559 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-16 20:30:10.000000 dtschema-2024.4/dtschema/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.869605 dtschema-2024.4/dtschema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-04-16 20:30:10.000000 dtschema-2024.4/dtschema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-16 20:30:10.000000 dtschema-2024.4/dtschema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:30:10.000000 dtschema-2024.4/dtschema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-16 20:30:10.000000 dtschema-2024.4/dtschema.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-16 20:30:10.000000 dtschema-2024.4/dtschema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 20:30:10.000000 dtschema-2024.4/dtschema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-16 20:30:06.000000 dtschema-2024.4/example-schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-16 20:30:06.000000 dtschema-2024.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:30:10.873605 dtschema-2024.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.869605 dtschema-2024.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-16 20:30:06.000000 dtschema-2024.4/test/bootphases.dts
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-16 20:30:06.000000 dtschema-2024.4/test/child-node-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-16 20:30:06.000000 dtschema-2024.4/test/child-node.dts
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-16 20:30:06.000000 dtschema-2024.4/test/conditionals-allof-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-16 20:30:06.000000 dtschema-2024.4/test/conditionals-allof-pass.dts
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-16 20:30:06.000000 dtschema-2024.4/test/conditionals-single-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-16 20:30:06.000000 dtschema-2024.4/test/conditionals-single-pass.dts
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-16 20:30:06.000000 dtschema-2024.4/test/device-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-16 20:30:06.000000 dtschema-2024.4/test/device.dts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.869605 dtschema-2024.4/test/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-16 20:30:06.000000 dtschema-2024.4/test/schemas/bad-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-16 20:30:06.000000 dtschema-2024.4/test/schemas/child-node-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-16 20:30:06.000000 dtschema-2024.4/test/schemas/conditionals-allof-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-16 20:30:06.000000 dtschema-2024.4/test/schemas/conditionals-single-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-16 20:30:06.000000 dtschema-2024.4/test/schemas/good-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-16 20:30:06.000000 dtschema-2024.4/test/simple-bus-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-16 20:30:06.000000 dtschema-2024.4/test/simple-bus-pass.dts
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5664 2024-04-16 20:30:06.000000 dtschema-2024.4/test/test-dt-validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.869605 dtschema-2024.4/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6206 2024-04-16 20:30:06.000000 dtschema-2024.4/tools/dt-prop-populate
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2135 2024-04-16 20:30:06.000000 dtschema-2024.4/tools/yaml-format
+-rwxr-xr-x   0 runner    (1001) docker     (127)      766 2024-04-16 20:30:06.000000 dtschema-2024.4/tools/yaml2json
```

### Comparing `dtschema-2024.2/.github/workflows/ci.yml` & `dtschema-2024.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/.github/workflows/publish.yml` & `dtschema-2024.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/LICENSE.txt` & `dtschema-2024.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/PKG-INFO` & `dtschema-2024.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtschema
-Version: 2024.2
+Version: 2024.4
 Summary: DeviceTree validation schema and tools
 Author-email: Rob Herring <robh@kernel.org>
 License: Copyright 2018-2019 Linaro Ltd.
         Copyright 2018-2020 Arm Ltd.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -41,15 +41,15 @@
 Requires-Dist: rfc3987
 Requires-Dist: pylibfdt
 
 # Devicetree Schema Tools
 
 The dtschema module contains tools and schema data for Devicetree
 schema validation using the
-[json-schema](http://json-schema.org/documentation.html) vocabulary.
+[json-schema](https://json-schema.org) vocabulary.
 The tools validate Devicetree files using DT binding schema files. The
 tools also validate the DT binding schema files. Schema files are
 written in a JSON compatible subset of YAML to be both human and machine
 readable.
 
 ## Data Model
```

### Comparing `dtschema-2024.2/README.md` & `dtschema-2024.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Devicetree Schema Tools
 
 The dtschema module contains tools and schema data for Devicetree
 schema validation using the
-[json-schema](http://json-schema.org/documentation.html) vocabulary.
+[json-schema](https://json-schema.org) vocabulary.
 The tools validate Devicetree files using DT binding schema files. The
 tools also validate the DT binding schema files. Schema files are
 written in a JSON compatible subset of YAML to be both human and machine
 readable.
 
 ## Data Model
```

### Comparing `dtschema-2024.2/dtschema/__init__.py` & `dtschema-2024.4/dtschema/__init__.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/check_compatible.py` & `dtschema-2024.4/dtschema/check_compatible.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/doc_validate.py` & `dtschema-2024.4/dtschema/doc_validate.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/dtb.py` & `dtschema-2024.4/dtschema/dtb.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     'uint8': u8,
     'int16': s16,
     'uint16': u16,
     'int32': s32,
     'uint32': u32,
     'int64': s64,
     'uint64': u64,
-    'phandle': u32
+    'phandle': u32,
+    'address': u32
 }
 
 
 def bytes_to_string(b):
     try:
         strings = b.decode(encoding='ascii').split('\0')
 
@@ -85,14 +86,21 @@
         return data[:-1].decode(encoding='ascii').split('\0')
 
     prop_types = set(validator.property_get_type(p.name))
     prop_types -= {'node'}
 
     # Filter out types impossible for the size of the property
     if len(prop_types) > 1:
+        if len(p) % 8:
+            prop_types -= {'int64', 'uint64', 'int64-array', 'uint64-array'}
+        if len(p) % 4:
+            prop_types -= {'int32', 'uint32', 'int32-array', 'uint32-array', 'phandle', 'phandle-array'}
+        if len(p) % 2:
+            prop_types -= {'int16', 'uint16', 'int16-array', 'uint16-array'}
+
         if len(p) > 4:
             prop_types -= {'int32', 'uint32', 'phandle'}
         else:
             prop_types -= {'int64', 'uint64', 'int64-array', 'uint64-array', 'phandle-array'}
         if len(p) > 2:
             prop_types -= {'int16', 'uint16'}
         else:
@@ -133,14 +141,17 @@
         if not len(data) % 4:
             fmt = 'uint32-array'
         else:
             #print(p.name + ': no type found', file=sys.stderr)
             return data
 
     if fmt.startswith('string'):
+        if not data.endswith(b'\0'):
+            # Wrong data type?, skip decoding to force errors
+            return data
         return data[:-1].decode(encoding='ascii').split('\0')
 
     if {'flag'} & prop_types:
         if len(data):
             if fmt == 'flag':
                 print('{prop}: boolean property with value {val}'.format(prop=p.name, val=data),
                       file=sys.stderr)
@@ -437,23 +448,23 @@
                         p_ac = 0
 
                     cells = ac + icells + 1 + p_ac + p_icells
                     dt[k] += [val[i:i + cells]]
                     i += cells
 
 
-def fixup_addresses(dt, ac, sc):
+def fixup_addresses(validator, dt, ac, sc):
     for k, v in dt.items():
         if isinstance(v, dict):
             if '#address-cells' in dt:
                 ac = _get_cells_size(dt,'#address-cells')
             if '#size-cells' in dt:
                 sc = _get_cells_size(dt, '#size-cells')
-            fixup_addresses(v, ac, sc)
-        elif k == 'reg':
+            fixup_addresses(validator, v, ac, sc)
+        elif 'address' in validator.property_get_type(k):
             i = 0
             dt[k] = []
             val = v[0]
             while i < len(val):
                 dt[k] += [val[i:i + ac + sc]]
                 i += ac + sc
         elif k in {'ranges', 'dma-ranges'} and not isinstance(v, bool):
@@ -472,12 +483,12 @@
 
     offset = fdt.first_subnode(-1, QUIET_NOTFOUND)
     dt = fdt_scan_node(validator, fdt, '/', offset)
 
     #print(phandle_loc)
     fixup_gpios(dt)
     fixup_interrupts(dt, 1)
-    fixup_addresses(dt, 2, 1)
+    fixup_addresses(validator, dt, 2, 1)
     fixup_phandles(validator, dt)
 
 #    pprint.pprint(dt, compact=True)
     return dt
```

### Comparing `dtschema-2024.2/dtschema/dtb2py.py` & `dtschema-2024.4/dtschema/dtb2py.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/dtb_validate.py` & `dtschema-2024.4/dtschema/dtb_validate.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import glob
 
 import dtschema
 
 verbose = False
 show_unmatched = False
 match_schema_file = None
+compatible_match = False
 
 
 class schema_group():
     def __init__(self, schema_file=""):
         if schema_file != "" and not os.path.exists(schema_file):
             exit(-1)
 
@@ -26,15 +27,16 @@
         # Hack to save some time validating examples
         if 'example-0' in node or 'example-' in nodename:
             return
 
         node['$nodename'] = [nodename]
 
         try:
-            for error in self.validator.iter_errors(node, filter=match_schema_file):
+            for error in self.validator.iter_errors(node, filter=match_schema_file,
+                                                    compatible_match=compatible_match):
 
                 # Disabled nodes might not have all the required
                 # properties filled in, such as a regulator or a
                 # GPIO meant to be filled at the DTS level on
                 # boards using that particular node. Thus, if the
                 # node is marked as disabled, let's just ignore
                 # any error message reporting a missing property.
@@ -89,35 +91,39 @@
             self.check_subtree(dt, subtree, False, "/", "/", filename)
 
 
 def main():
     global verbose
     global show_unmatched
     global match_schema_file
+    global compatible_match
 
     ap = argparse.ArgumentParser(fromfile_prefix_chars='@',
         epilog='Arguments can also be passed in a file prefixed with a "@" character.')
     ap.add_argument("dtbs", nargs='*',
                     help="Filename or directory of devicetree DTB input file(s)")
     ap.add_argument('-s', '--schema', help="preparsed schema file or path to schema files")
     ap.add_argument('-p', '--preparse', help="preparsed schema file (deprecated, use '-s')")
     ap.add_argument('-l', '--limit', help="limit validation to schemas with $id matching LIMIT substring")
+    ap.add_argument('-c', '--compatible-match', action="store_true",
+                    help="limit validation to schema matching nodes' most specific compatible string")
     ap.add_argument('-m', '--show-unmatched',
         help="Print out node 'compatible' strings which don't match any schema.",
         action="store_true")
     ap.add_argument('-n', '--line-number', help="Obsolete", action="store_true")
     ap.add_argument('-v', '--verbose', help="verbose mode", action="store_true")
     ap.add_argument('-u', '--url-path', help="Additional search path for references (deprecated)")
     ap.add_argument('-V', '--version', help="Print version number",
                     action="version", version=dtschema.__version__)
     args = ap.parse_args()
 
     verbose = args.verbose
     show_unmatched = args.show_unmatched
     match_schema_file = args.limit
+    compatible_match = args.compatible_match
 
     # Maintain prior behaviour which accepted file paths by stripping the file path
     if args.url_path and args.limit:
         for d in args.url_path.split(os.path.sep):
             if d and match_schema_file.startswith(d):
                 match_schema_file = match_schema_file[(len(d) + 1):]
```

### Comparing `dtschema-2024.2/dtschema/extract_compatibles.py` & `dtschema-2024.4/dtschema/extract_compatibles.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/extract_example.py` & `dtschema-2024.4/dtschema/extract_example.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/extract_props.py` & `dtschema-2024.4/dtschema/extract_props.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/fixups.py` & `dtschema-2024.4/dtschema/fixups.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,14 +110,16 @@
         return
 
     tmpsch = {}
     if 'minItems' in subschema:
         tmpsch['minItems'] = subschema.pop('minItems')
     if 'maxItems' in subschema:
         tmpsch['maxItems'] = subschema.pop('maxItems')
+    if 'items' in subschema:
+        tmpsch['items'] = subschema.pop('items')
 
     if tmpsch:
         subschema['items'] = tmpsch
         subschema['maxItems'] = 1
 
 def _fixup_remove_empty_items(subschema):
     if 'items' not in subschema:
@@ -247,17 +249,49 @@
     _fixup_string_to_array(schema)
     _fixup_scalar_to_array(schema)
     _fixup_items_size(schema, path=path)
 
     fixup_schema_to_201909(schema)
 
 
+def _fixup_oneOf_to_enum(schema, path=[]):
+    # Convert oneOf/anyOf lists with just 'const' entries into an enum.
+    # This pattern is used to add descriptions on each entry which is not
+    # possible with 'enum', but the error reporting is much worse with
+    # oneOf/anyOf schemas.
+
+    if 'anyOf' in schema:
+        sch_list = schema['anyOf']
+    elif 'oneOf' in schema:
+        sch_list = schema['oneOf']
+    elif 'items' in schema and isinstance(schema['items'], dict):
+        # Sometimes 'items' appears first which isn't really handled by the
+        # fixups, but we can handle it here.
+        _fixup_oneOf_to_enum(schema['items'], path=path + ['items'])
+        return
+    else:
+        return
+
+    const_list = []
+    for l in sch_list:
+        if 'const' not in l or set(l) > {'const', 'description'}:
+            return
+        const_list += [l['const']]
+
+    schema.pop('anyOf', None)
+    schema.pop('oneOf', None)
+    schema['enum'] = const_list
+
+
 def walk_properties(schema, path=[]):
     if not isinstance(schema, dict):
         return
+
+    _fixup_oneOf_to_enum(schema, path=path)
+
     # Recurse until we don't hit a conditional
     # Note we expect to encounter conditionals first.
     # For example, a conditional below 'items' is not supported
     for cond in ['allOf', 'oneOf', 'anyOf']:
         if cond in schema.keys():
             for l in schema[cond]:
                 walk_properties(l, path=path + [cond])
@@ -399,54 +433,29 @@
     return result
 
 
 def add_select_schema(schema):
     '''Get a schema to be used in select tests.
 
     If the provided schema has a 'select' property, then use that as the select schema.
-    If it has a compatible property, then create a select schema from that.
     If it has a $nodename property, then create a select schema from that.
-    If it has none of those, then return a match-nothing schema
     '''
     if "select" in schema:
         return
 
-    if 'properties' not in schema:
-        schema['select'] = False
+    if 'properties' not in schema or 'compatible' in schema['properties']:
         return
 
-    if 'compatible' in schema['properties']:
-        compatible_list = dtschema.extract_node_compatibles(schema['properties']['compatible'])
-
-        if len(compatible_list):
-            try:
-                compatible_list.remove('syscon')
-            except:
-                pass
-            try:
-                compatible_list.remove('simple-mfd')
-            except:
-                pass
-
-            if len(compatible_list) != 0:
-                schema['select'] = {
-                    'required': ['compatible'],
-                    'properties': {'compatible': {'contains': {'enum': sorted(compatible_list)}}}}
-
-                return
-
     if '$nodename' in schema['properties'] and schema['properties']['$nodename'] is not True:
         schema['select'] = {
             'required': ['$nodename'],
             'properties': {'$nodename': convert_to_dict(schema['properties']['$nodename'])}}
 
         return
 
-    schema['select'] = False
-
 
 def fixup_schema(schema):
     # Remove parts not necessary for validation
     schema.pop('examples', None)
     schema.pop('maintainers', None)
     schema.pop('historical', None)
```

### Comparing `dtschema-2024.2/dtschema/lib.py` & `dtschema-2024.4/dtschema/lib.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/meta-schemas/base.yaml` & `dtschema-2024.4/dtschema/meta-schemas/base.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/meta-schemas/cell.yaml` & `dtschema-2024.4/dtschema/meta-schemas/cell.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/meta-schemas/clocks.yaml` & `dtschema-2024.4/dtschema/meta-schemas/clocks.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/meta-schemas/core.yaml` & `dtschema-2024.4/dtschema/meta-schemas/core.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/meta-schemas/gpios.yaml` & `dtschema-2024.4/dtschema/meta-schemas/gpios.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/meta-schemas/interrupts.yaml` & `dtschema-2024.4/dtschema/meta-schemas/interrupts.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/meta-schemas/items.yaml` & `dtschema-2024.4/dtschema/meta-schemas/items.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/meta-schemas/keywords.yaml` & `dtschema-2024.4/dtschema/meta-schemas/keywords.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/meta-schemas/nodes.yaml` & `dtschema-2024.4/dtschema/meta-schemas/nodes.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/meta-schemas/string-array.yaml` & `dtschema-2024.4/dtschema/meta-schemas/string-array.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/meta-schemas/types.yaml` & `dtschema-2024.4/dtschema/meta-schemas/types.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/meta-schemas/vendor-props.yaml` & `dtschema-2024.4/dtschema/meta-schemas/vendor-props.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/mk_schema.py` & `dtschema-2024.4/dtschema/mk_schema.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schema.py` & `dtschema-2024.4/dtschema/schema.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/aliases.yaml` & `dtschema-2024.4/dtschema/schemas/aliases.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/bootph.yaml` & `dtschema-2024.4/dtschema/schemas/bootph.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/bus/qemu,platform.yaml` & `dtschema-2024.4/dtschema/schemas/bus/qemu,platform.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/cache-controller.yaml` & `dtschema-2024.4/dtschema/schemas/cache-controller.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/cache.yaml` & `dtschema-2024.4/dtschema/schemas/cache.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/chosen.yaml` & `dtschema-2024.4/dtschema/schemas/chosen.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -71,18 +71,16 @@
     description:
       This property is set (currently only on PowerPC, and only needed on
       book3e) by some versions of kexec-tools to tell the new kernel that it
       is being booted by kexec, as the booting environment may differ (e.g.
       a different secondary CPU release mechanism).
 
   linux,elfcorehdr:
-    oneOf:
-      - $ref: types.yaml#/definitions/uint32-array
-      - $ref: types.yaml#/definitions/uint64-array
-    maxItems: 2
+    $ref: types.yaml#/definitions/address
+    maxItems: 1
     description: |
       This property holds the memory range, the address and the size, of the
       elf core header which mainly describes the panicked kernel\'s memory
       layout as PT_LOAD segments of elf format.
 
       / {
               chosen {
@@ -91,18 +89,16 @@
       };
 
       While this property does not represent a real hardware, the address
       and the size are expressed in #address-cells and #size-cells,
       respectively, of the root node.
 
   linux,usable-memory-range:
-    oneOf:
-      - $ref: types.yaml#/definitions/uint32-array
-      - $ref: types.yaml#/definitions/uint64-array
-    maxItems: 2
+    $ref: types.yaml#/definitions/address
+    maxItems: 1
     description: |
       This property holds a base address and size, describing a limited region
       in which memory may be considered available for use by the kernel. Memory
       outside of this range is not available for use.
 
       This property describes a limitation: memory within this range is only
       valid when also described through another mechanism that the kernel
@@ -120,26 +116,24 @@
       part of the panicked kernel\'s memory.
 
       While this property does not represent a real hardware, the address
       and the size are expressed in #address-cells and #size-cells,
       respectively, of the root node.
 
   linux,initrd-start:
-    oneOf:
-      - $ref: types.yaml#/definitions/uint32
-      - $ref: types.yaml#/definitions/uint64
+    $ref: types.yaml#/definitions/address
+    maxItems: 1
     description:
       These properties hold the physical start and end address of an initrd that\'s
       loaded by the bootloader. Note that linux,initrd-start is inclusive, but
       linux,initrd-end is exclusive.
 
   linux,initrd-end:
-    oneOf:
-      - $ref: types.yaml#/definitions/uint32
-      - $ref: types.yaml#/definitions/uint64
+    $ref: types.yaml#/definitions/address
+    maxItems: 1
     description:
       These properties hold the physical start and end address of an initrd that\'s
       loaded by the bootloader. Note that linux,initrd-start is inclusive, but
       linux,initrd-end is exclusive.
 
   linux,pci-probe-only:
     $ref: types.yaml#/definitions/uint32
@@ -187,18 +181,16 @@
 
       Implementation note: Linux will look for the property "linux,stdout-path"
       or on PowerPC "stdout" if "stdout-path" is not found.  However, the
       "linux,stdout-path" and "stdout" properties are deprecated. New platforms
       should only use the "stdout-path" property.
 
   linux,ima-kexec-buffer:
-    oneOf:
-      - $ref: types.yaml#/definitions/uint32-array
-      - $ref: types.yaml#/definitions/uint64-array
-    maxItems: 2
+    $ref: types.yaml#/definitions/address
+    maxItems: 1
     description: |
       This property(currently used by powerpc, arm64) holds the memory range,
       "the address and the size", of the Integrity Measurement Architecture(IMA)
       measurement logs that are being carried over to the new kernel.
 
       / {
           chosen {
@@ -206,34 +198,14 @@
           };
       };
 
       This property does not represent real hardware, but the memory allocated for
       carrying the IMA measurement logs. The address and the size are expressed in
       #address-cells and #size-cells, respectively of the root node.
 
-  linux,tpm-kexec-buffer:
-    oneOf:
-      - $ref: types.yaml#/definitions/uint32-array
-      - $ref: types.yaml#/definitions/uint64-array
-    maxItems: 2
-    description: |
-      This property (currently used by powerpc64) holds the memory range,
-      "the address and the size", of the TPM's measurement log that is being
-      carried over to the new kernel.
-
-      / {
-          chosen {
-              linux,tpm-kexec-buffer = <0x9 0x82000000 0x0 0x00008000>;
-          };
-      };
-
-      This property does not represent real hardware, but the memory allocated for
-      carrying the TPM measurement log. The address and the size are expressed in
-      #address-cells and #size-cells, respectively of the root node.
-
   linux,uefi-system-table:
     $ref: types.yaml#/definitions/uint64
     description:
       Physical address of the UEFI System Table.
 
   linux,uefi-mmap-start:
     $ref: types.yaml#/definitions/uint64
```

### Comparing `dtschema-2024.2/dtschema/schemas/clock/clock.yaml` & `dtschema-2024.4/dtschema/schemas/clock/clock.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/cpu-map.yaml` & `dtschema-2024.4/dtschema/schemas/cpu-map.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/cpu.yaml` & `dtschema-2024.4/dtschema/schemas/cpu.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/cpus.yaml` & `dtschema-2024.4/dtschema/schemas/cpus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/dt-core.yaml` & `dtschema-2024.4/dtschema/schemas/dt-core.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/gpio/gpio-consumer.yaml` & `dtschema-2024.4/dtschema/schemas/gpio/gpio-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/gpio/gpio-hog.yaml` & `dtschema-2024.4/dtschema/schemas/gpio/gpio-hog.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/gpio/gpio.yaml` & `dtschema-2024.4/dtschema/schemas/gpio/gpio.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/graph.yaml` & `dtschema-2024.4/dtschema/schemas/graph.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/hwlock/hwlock-consumer.yaml` & `dtschema-2024.4/dtschema/schemas/hwlock/hwlock-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/i2c/i2c-controller.yaml` & `dtschema-2024.4/dtschema/schemas/i2c/i2c-controller.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/iio/iio-consumer.yaml` & `dtschema-2024.4/dtschema/schemas/iio/iio-consumer.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -27,23 +27,29 @@
   io-channels:
     $ref: /schemas/types.yaml#/definitions/phandle-array
     description: >
       List of phandle and IIO specifier pairs, one pair for each IIO input
       to the device. Note: if the IIO provider specifies '0' for
       #io-channel-cells, then only the phandle portion of the pair will appear.
 
+  io-channel-names:
+    $ref: /schemas/types.yaml#/definitions/string-array
+
   io-backends:
     $ref: /schemas/types.yaml#/definitions/phandle-array
     description:
       List of phandles for IIO backends. IIO backends are devices connected to
       another IIO devices (consumers of the backends) providing services so
       that the consumer IIO device can be fully functional. One typical example
       of such an Hardware arrangement would be an high speed ADC that is
       connected to an FPGA IP core (through a serial data interface as LVDS)
       capable of handling the high sample rates. Examples of the provided
       services would be channel enablement/disablement.
 
+  io-backend-names:
+    $ref: /schemas/types.yaml#/definitions/string-array
+
 dependencies:
   io-channel-names: [io-channels]
   io-backend-names: [io-backends]
 
 additionalProperties: true
```

### Comparing `dtschema-2024.2/dtschema/schemas/iio/iio.yaml` & `dtschema-2024.4/dtschema/schemas/iio/iio.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/interrupt-controller.yaml` & `dtschema-2024.4/dtschema/schemas/interrupt-controller.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/interrupts.yaml` & `dtschema-2024.4/dtschema/schemas/interrupts.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/iommu/iommu.yaml` & `dtschema-2024.4/dtschema/schemas/iommu/iommu.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/isa/isa-bridge.yaml` & `dtschema-2024.4/dtschema/schemas/isa/isa-bridge.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/isa/isa-bus.yaml` & `dtschema-2024.4/dtschema/schemas/isa/isa-bus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/mbox/mbox-consumer.yaml` & `dtschema-2024.4/dtschema/schemas/mbox/mbox-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/memory.yaml` & `dtschema-2024.4/dtschema/schemas/memory.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/msi-consumer.yaml` & `dtschema-2024.4/dtschema/schemas/msi-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/numa-distance-map-v1.yaml` & `dtschema-2024.4/dtschema/schemas/numa-distance-map-v1.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/opp/opp.yaml` & `dtschema-2024.4/dtschema/schemas/opp/opp.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/options/u-boot.yaml` & `dtschema-2024.4/dtschema/schemas/options/u-boot.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/options.yaml` & `dtschema-2024.4/dtschema/schemas/options.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/pci/pci-bus-common.yaml` & `dtschema-2024.4/dtschema/schemas/pci/pci-bus-common.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/pci/pci-bus.yaml` & `dtschema-2024.4/dtschema/schemas/pci/pci-bus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/pci/pci-device.yaml` & `dtschema-2024.4/dtschema/schemas/pci/pci-device.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/pci/pci-host-bridge.yaml` & `dtschema-2024.4/dtschema/schemas/pci/pci-host-bridge.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/pci/pci-iommu.yaml` & `dtschema-2024.4/dtschema/schemas/pci/pci-iommu.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/pci/pci-pci-bridge.yaml` & `dtschema-2024.4/dtschema/schemas/pci/pci-pci-bridge.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 
   supports-d3:
     description:
       If present, this property specifies that the bridge supports transitioning
       to D3 states.
     type: boolean
 
-unevaluatedProperties: false
+additionalProperties: true
```

### Comparing `dtschema-2024.2/dtschema/schemas/phy/phy-consumer.yaml` & `dtschema-2024.4/dtschema/schemas/phy/phy-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/phy/phy-provider.yaml` & `dtschema-2024.4/dtschema/schemas/phy/phy-provider.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/pinctrl/pinctrl-consumer.yaml` & `dtschema-2024.4/dtschema/schemas/pinctrl/pinctrl-consumer.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 
 # always select the core schema
 select: true
 
 properties:
   pinctrl-0: true
 
-  pinctrl-names: true
+  pinctrl-names:
+    $ref: /schemas/types.yaml#/definitions/string-array
 
 patternProperties:
   "^pinctrl-[0-9]+$":
     $ref: /schemas/types.yaml#/definitions/phandle-array
 
 dependencies:
   pinctrl-names: [ pinctrl-0 ]
```

### Comparing `dtschema-2024.2/dtschema/schemas/power-domain/power-domain-consumer.yaml` & `dtschema-2024.4/dtschema/schemas/power-domain/power-domain-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/property-units.yaml` & `dtschema-2024.4/dtschema/schemas/property-units.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/pwm/pwm-consumer.yaml` & `dtschema-2024.4/dtschema/schemas/pwm/pwm-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/reg.yaml` & `dtschema-2024.4/dtschema/schemas/reg.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
   ranges:
     oneOf:
       - $ref: types.yaml#/definitions/flag
       - $ref: types.yaml#/definitions/uint32-matrix
 
   reg:
-    $ref: types.yaml#/definitions/uint32-matrix
+    $ref: types.yaml#/definitions/address
 
   reg-io-width:
     $ref: types.yaml#/definitions/uint32
     minimum: 1
     maximum: 0xf
     description:
       Typically, a single set bit indicating the access size, but some uses treat
```

### Comparing `dtschema-2024.2/dtschema/schemas/reserved-memory/framebuffer.yaml` & `dtschema-2024.4/dtschema/schemas/reserved-memory/framebuffer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/reserved-memory/memory-region.yaml` & `dtschema-2024.4/dtschema/schemas/reserved-memory/memory-region.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/reserved-memory/reserved-memory.yaml` & `dtschema-2024.4/dtschema/schemas/reserved-memory/reserved-memory.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/reserved-memory/shared-dma-pool.yaml` & `dtschema-2024.4/dtschema/schemas/reserved-memory/shared-dma-pool.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/reset/reset.yaml` & `dtschema-2024.4/dtschema/schemas/reset/reset.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/root-node.yaml` & `dtschema-2024.4/dtschema/schemas/root-node.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/simple-bus.yaml` & `dtschema-2024.4/dtschema/schemas/simple-bus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/thermal/thermal.yaml` & `dtschema-2024.4/dtschema/schemas/thermal/thermal.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/dtschema/schemas/types.yaml` & `dtschema-2024.4/dtschema/schemas/types.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -345,7 +345,13 @@
               type: integer
               minimum: 1
               maximum: 0xffffffff
             - type: integer
               const: 0
       additionalItems:
         $ref: "#/definitions/cell"
+
+  address:
+    $ref: "#/definitions/uint32-matrix"
+    items:
+      minItems: 1
+      maxItems: 5 # At most 3 address cells and 2 size cells
```

### Comparing `dtschema-2024.2/dtschema/validator.py` & `dtschema-2024.4/dtschema/validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         if maximum == 1:
             minimum = 1
         d.insert(i, (minimum, maximum))
 
     return tuple(d)
 
 
-type_re = re.compile('(flag|u?int(8|16|32|64)(-(array|matrix))?|string(-array)?|phandle(-array)?)')
+type_re = re.compile('(address|flag|u?int(8|16|32|64)(-(array|matrix))?|string(-array)?|phandle(-array)?)')
 
 
 def _extract_prop_type(props, schema, propname, subschema, is_pattern):
     if propname.startswith('$'):
         return
 
     if not isinstance(subschema, dict):
@@ -235,15 +235,15 @@
                c.startswith('^') and c.endswith('$'):
                 compat_sch += [{'pattern': c}]
         else:
             compat_sch[0]['enum'].append(c)
 
     compat_sch[0]['enum'].sort()
     schemas['generated-compatibles'] = {
-        '$id': 'http://devicetree.org/schemas/generated-compatibles',
+        '$id': 'generated-compatibles',
         '$filename': 'Generated schema of documented compatible strings',
         'select': True,
         'properties': {
             'compatible': {
                 'items': {
                     'anyOf': compat_sch
                 }
@@ -265,17 +265,14 @@
     except jsonschema.SchemaError as exc:
         print(f"{filename}: ignoring, error in schema: " + ': '.join(str(x) for x in exc.path),
               file=sys.stderr)
         #print(exc.message)
         return
 
     schema = dtsch.fixup()
-    if 'select' not in schema:
-        print(f"{filename}: warning: no 'select' found in schema found", file=sys.stderr)
-        return
 
     schema["type"] = "object"
     schema["$filename"] = filename
     return schema
 
 
 def _add_schema(schemas, filename):
@@ -355,25 +352,18 @@
                     except:
                         print("preprocessed schema file is not valid JSON or YAML\n", file=sys.stderr)
                         raise
 
             # Ensure the cache is a processed schema and not just a single schema file
             if '$id' in schema_cache:
                 schema_cache = None
+            elif schema_cache.pop('version', None) != dtschema.__version__:
+                raise Exception(f"Processed schema out of date, delete and retry: {os.path.abspath(schema_files[0])}")
 
         if schema_cache:
-            # Convert old format to new
-            if isinstance(schema_cache, list):
-                d = {}
-                for sch in schema_cache:
-                    if not isinstance(sch, dict):
-                        return None
-                    d[sch['$id']] = sch
-                schema_cache = d
-
             if 'generated-types' in schema_cache:
                 self.props = schema_cache['generated-types']['properties']
             if 'generated-pattern-types' in schema_cache:
                 self.pat_props = copy.deepcopy(schema_cache['generated-pattern-types']['properties'])
                 for k in self.pat_props:
                     self.pat_props[k][0]['regex'] = re.compile(k)
 
@@ -381,14 +371,30 @@
         else:
             self.schemas = process_schemas(schema_files)
             self.make_property_type_cache()
             make_compatible_schema(self.schemas)
             for k in self.pat_props:
                 self.pat_props[k][0]['regex'] = re.compile(k)
 
+        # Speed up iterating thru schemas in validation by saving a list of schemas
+        # to always apply and a map of compatible strings to schema.
+        self.always_schemas = []
+        self.compat_map = {}
+        for sch in self.schemas.values():
+            if 'select' in sch:
+                if sch['select'] is not False:
+                    self.always_schemas += [sch['$id']]
+            elif 'properties' in sch and 'compatible' in sch['properties']:
+                compatibles = dtschema.extract_node_compatibles(sch['properties']['compatible'])
+                compatibles = set(compatibles) - {'syscon', 'simple-mfd'}
+                for c in compatibles:
+                    self.compat_map[c] = sch['$id']
+
+        self.schemas['version'] = dtschema.__version__
+
     def http_handler(self, uri):
         '''Custom handler for http://devicetree.org references'''
         try:
             uri += '#'
             if uri in self.schemas:
                 return self.schemas[uri]
             else:
@@ -399,25 +405,39 @@
             raise RefResolutionError('Error in referenced schema matching $id: ' + uri)
 
     def annotate_error(self, id, error):
         error.schema_file = id
         error.linecol = -1, -1
         error.note = None
 
-    def iter_errors(self, instance, filter=None):
-        for id, schema in self.schemas.items():
-            if 'select' not in schema:
-                continue
-            if filter and filter not in id:
+    def iter_errors(self, instance, filter=None, compatible_match=False):
+        if 'compatible' in instance:
+            inst_compat = instance['compatible'][0]
+            if inst_compat in self.compat_map:
+                schema_id = self.compat_map[inst_compat]
+                if not filter or filter in schema_id:
+                    schema = self.schemas[schema_id]
+                    for error in self.DtValidator(schema,
+                                                  resolver=self.resolver,
+                                                  ).iter_errors(instance):
+                        self.annotate_error(schema['$id'], error)
+                        yield error
+
+        if compatible_match:
+            return
+
+        for schema_id in self.always_schemas:
+            if filter and filter not in schema_id:
                 continue
-            sch = {'if': schema['select'], 'then': schema}
-            for error in self.DtValidator(sch,
+            schema = {'if': self.schemas[schema_id]['select'],
+                      'then': self.schemas[schema_id]}
+            for error in self.DtValidator(schema,
                                           resolver=self.resolver,
                                           ).iter_errors(instance):
-                self.annotate_error(id, error)
+                self.annotate_error(schema_id, error)
                 yield error
 
     def validate(self, instance, filter=None):
         for error in self.iter_errors(instance, filter=filter):
             raise error
 
     def get_undocumented_compatibles(self, compatible_list):
```

### Comparing `dtschema-2024.2/dtschema.egg-info/PKG-INFO` & `dtschema-2024.4/dtschema.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtschema
-Version: 2024.2
+Version: 2024.4
 Summary: DeviceTree validation schema and tools
 Author-email: Rob Herring <robh@kernel.org>
 License: Copyright 2018-2019 Linaro Ltd.
         Copyright 2018-2020 Arm Ltd.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -41,15 +41,15 @@
 Requires-Dist: rfc3987
 Requires-Dist: pylibfdt
 
 # Devicetree Schema Tools
 
 The dtschema module contains tools and schema data for Devicetree
 schema validation using the
-[json-schema](http://json-schema.org/documentation.html) vocabulary.
+[json-schema](https://json-schema.org) vocabulary.
 The tools validate Devicetree files using DT binding schema files. The
 tools also validate the DT binding schema files. Schema files are
 written in a JSON compatible subset of YAML to be both human and machine
 readable.
 
 ## Data Model
```

### Comparing `dtschema-2024.2/dtschema.egg-info/SOURCES.txt` & `dtschema-2024.4/dtschema.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 dtschema/schemas/interconnects.yaml
 dtschema/schemas/interrupt-controller.yaml
 dtschema/schemas/interrupts.yaml
 dtschema/schemas/memory.yaml
 dtschema/schemas/msi-consumer.yaml
 dtschema/schemas/numa-distance-map-v1.yaml
 dtschema/schemas/options.yaml
+dtschema/schemas/post-init-providers.yaml
 dtschema/schemas/property-units.yaml
 dtschema/schemas/reg.yaml
 dtschema/schemas/root-node.yaml
 dtschema/schemas/serial.yaml
 dtschema/schemas/simple-bus.yaml
 dtschema/schemas/types.yaml
 dtschema/schemas/bus/qemu,platform.yaml
```

### Comparing `dtschema-2024.2/example-schema.yaml` & `dtschema-2024.4/example-schema.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/pyproject.toml` & `dtschema-2024.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/test/child-node-fail.dts` & `dtschema-2024.4/test/child-node-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/test/child-node.dts` & `dtschema-2024.4/test/child-node.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/test/conditionals-allof-fail.dts` & `dtschema-2024.4/test/conditionals-allof-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/test/conditionals-allof-pass.dts` & `dtschema-2024.4/test/conditionals-allof-pass.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/test/conditionals-single-fail.dts` & `dtschema-2024.4/test/conditionals-single-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/test/device-fail.dts` & `dtschema-2024.4/test/device-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/test/device.dts` & `dtschema-2024.4/test/device.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/test/schemas/bad-example.yaml` & `dtschema-2024.4/test/schemas/bad-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/test/schemas/child-node-example.yaml` & `dtschema-2024.4/test/schemas/child-node-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/test/schemas/conditionals-allof-example.yaml` & `dtschema-2024.4/test/schemas/conditionals-allof-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/test/schemas/conditionals-single-example.yaml` & `dtschema-2024.4/test/schemas/conditionals-single-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/test/schemas/good-example.yaml` & `dtschema-2024.4/test/schemas/good-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/test/simple-bus-pass.dts` & `dtschema-2024.4/test/simple-bus-pass.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/test/test-dt-validate.py` & `dtschema-2024.4/test/test-dt-validate.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/tools/dt-prop-populate` & `dtschema-2024.4/tools/dt-prop-populate`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/tools/yaml-format` & `dtschema-2024.4/tools/yaml-format`

 * *Files identical despite different names*

### Comparing `dtschema-2024.2/tools/yaml2json` & `dtschema-2024.4/tools/yaml2json`

 * *Files identical despite different names*

