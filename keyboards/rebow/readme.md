# The rebow keyboard

```sh
make rebow/rev1:default
```

Example of flashing this keyboard:

```sh
make rebow/rev1:default:avrdude
```

```
                              +-----+
                   +----------| USB |----------+
                   |          +-----+          |
                   | [ ]D3      ___     RAW[ ] |
                   | [ ]D2     / P \    GND[x] |  -> TRRS/LED
                   | [ ]GND   /  R  \   RST[ ] |
                   | [ ]GND   |  O  |   VCC[x] |  -> TRRS/LED
           TRRS <- | [x]D1    |     |    F4[ ] |
           TRRS <- | [x]D0    |  M  |    F5[x] |  -> COL0
            LED <- | [x]D4    |  I  |    F6[x] |  -> COL1
           ROW0 <- | [x]C6    |  C  |    F7[x] |  -> COL2
           ROW1 <- | [x]D7    |  R  |    B1[x] |  -> COL3
           ROW2 <- | [x]E6    \  O  /    B3[x] |  -> COL4
           ROW3 <- | [x]B4     \_ _/     B2[x] |  -> COL5
           ROW4 <- | [x]B5       	 B6[x] |  -> COL6
                   |             	       |
                   | Pro Micro		       |
                   +---------------------------+
```

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).
