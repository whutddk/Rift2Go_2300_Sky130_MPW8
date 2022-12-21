# Rift2Core

## Rift2300

This is the simplest version of [Rift2Core](https://github.com/whutddk/Rift2Core/tree/develop).
Commit: b95a1555aeb79d975e8b273d412f0e6df42d0322 (Almost...)


----------------------------



The configuration is as followed, and IF2 is mixed with **IF2NCache**
```
class Rift2300 extends Config((site, here, up) => {
  case RiftParamsKey => RiftSetting(
    hasL2  = false,
    hasDebugger = true,
    hasPreFetch = false,
    hasuBTB = false,
    ftChn = 4,
    rnChn = 1,
    opChn = 1,
    wbChn = 1,
    cm_chn = 1,
    pmpNum = 0,
    regNum = 34,
    hpmNum  = 0,
    l1BeatBits = 64,
    memBeatBits = 64,
    tlbEntry = 2,
    l1DW = 128,
    ifetchParameters = IFParameters(
      uBTB_entry = 2,
      // uBTB_tag_w = 16,
      btb_cl = 0,
      bim_cl = 2,
      ras_dp = 0,
      // tage_table = 6, 
    ),
    icacheParameters = IcacheParameters(
      bk = 1,
      cb = 1,
      cl = 2,
    ),
    dcacheParameters = DcacheParameters(
      bk = 1,
      cb = 1,
      cl = 2,
      sbEntry = 1,
      stEntry = 2,
    ),

    dptEntry = 1,
    fpuNum = 0,
    mulNum = 0,

    isMinArea = true,
    isLowPower = false,
  )
})

```


