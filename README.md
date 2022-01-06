## TON wallet address for donations: <br />
__EQAvRnuckR42aEE29_WCDCTOwEci1ZKo8a5ul4ncYWaqxA2q__

## This is improved official custom miner for TON
* As base legacy code is used, which is currently works on all GPUs
* Added some cool OpenCL optimizations and now we have ~1.8x boost on AMD and NVidia cards
* And works on all platforms 

## "Soft" Pull Request rules

* Thou shall not merge your own PRs, at least one person should review the PR and merge it (4-eyes rule)
* Thou shall make sure that workflows are cleanly completed for your PR before considering merge

## Workflows responsibility
If a CI workflow fails not because of your changes but workflow issues, try to fix it yourself or contact one of the persons listed below via Telegram messenger:

* **C/C++ CI (ccpp-linux.yml)**: TBD
* **C/C++ CI Win64 Compile (ccpp-win64.yml)**: TBD

## GPU POW miner

GPU pow-miner located at `crypto/util`, check [pow-miner.md](crypto/util/pow-miner.md) and [pow-miner-howto.md](crypto/util/pow-miner-howto.md) for details.

TONLIB CLI with embedded GPU-miner located at `tonlib/tonlib`, check [pow-miner-howto.md](crypto/util/pow-miner-howto.md#tonlib-cli-wrapper-with-embedded-gpu-miner) for details.

GPU miner executable files for Windows can be downloaded from https://github.com/sunnyhellious/pow-miner-gpu-improved/releases, check [pow-miner-windows-howto.md](crypto/util/pow-miner-windows-howto.md) for details.

HW Supported:
- Nvidia: nVidia GT640+ or newer, Quadro series with Kepler chip or newer (FX not supported)
- Radeon HD78xx series and newer, AMD GPU GCN 1.0+
- HD4000 or newer

Tested on:

| GPU | Hashrate |
|-----|:---------|
NVIDIA GTX1070 | 9.0e+08
AMD Radeon 4890 | 5.5e+07
