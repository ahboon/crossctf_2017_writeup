# CrossCTF_2017: Sky Pillar 1

**Category:** Reverse Engineering
**Points:** 100
**Description:**

>192.168.0.31:1350 [File here](skypillar)

## Write-up
Looking in `levelone()`, we find our hex-encoded passphrase in little endian, so we need to deal with that.

    0x40772049
    0x20406e6e
    0x74206562
    0x76206568
    0x20797265
    0x74736562

    V

    49207740
    6e6e4020
    62652074
    68652076
    65727920
    62657374

Decoding it yields `I w@nn@ be the very best`.

Therefore, the flag is `I w@nn@ be the very best`.
