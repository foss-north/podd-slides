---
title: Permissive Software Licenses
subtitle: foss-north pod
author: foss-north
license: CC-BY-SA 3.0
header-includes: |
    \usepackage{xcolor}
    \definecolor{fossorange}{HTML}{ffcc33}
    \setbeamercolor{background canvas}{bg=black}
    \setbeamercolor{section in head/foot}{bg=black,fg=fossorange}
    \setbeamercolor{subsection in head/foot}{bg=fossorange,fg=black}
    \setbeamercolor{normal text}{fg=fossorange}
    \setbeamercolor{block title}{fg=black,bg=fossorange}
    \setbeamercolor{titlelike}{fg=fossorange}
    \setbeamercolor{itemize item}{fg=fossorange}
    \setbeamercolor{itemize subitem}{fg=fossorange}
    \setbeamerfont{caption}{size=\tiny}
    \setbeamerfont{footnote}{size=\tiny}
    \setbeamerfont{footnote mark}{size=\tiny}
theme: Malmoe
aspectratio: 169

---

# Background
## BSD History
- BSD was based on Research Unix by AT&T[^1]
- Early versions subject to AT&T license
- Networking code first released under BSD license 1989
- Rest of BSD rewritten to remove all AT&T code 1991

[^1]: https://en.wikipedia.org/wiki/History_of_the_Berkeley_Software_Distribution

## BSD History
- AT&T sued[^AT&T]
- Slowed development, helped Linux gain popularity[^LinuxBSD]
- BSD 4.4 released afterwards
    - FreeBSD, OpenBSD, NetBSD etc

[^AT&T]: https://en.wikipedia.org/wiki/USL_v._BSDi
[^LinuxBSD]: https://gondwanaland.com/meta/history/interview.html

## MIT history
- MIT, IBM and DEC (now HP) collaboration
    - X window system
    - Kerberos
- Wanted to make it public domain - IBM didn't like that[^IBM]
- New license created with MIT lawyers[^MITLawyer]
- X license and MIT license not the same but very similar

[^IBM]: https://opensource.com/article/19/4/history-mit-license
[^MITLawyer]: https://twitter.com/JimGettys/status/1112782559937789953

## Why permissive?
- Allows proprietary changes
- Usually allows relicensing as proprietary
- Easier to understand
- Highly compatible (allow further restrictions)

![FOSS license flow: CC-BY-SA 3.0 (C) 2017 David Wheeler https://dwheeler.com/essays/floss-license-slide.html](license-flow.png){ width=50% }

# BSD licenses and friends

## Original BSD license
- 4 clauses
    - Source distribution requires copyright notice
    - Binary distribution requires copyright notice in documentation
    - Advertisement material requires acknowledgement of original authors
    - May not use original authors as promotion
- Incompatible with GPL - imposes extra restrictions

## New BSD license
- 3 clauses
- Advertisement clause removed
- Used by CMake, tcpdump, XMonad

## Simplified BSD license
- 2 clauses
- Non-endorsement clause removed
- Used by FreeBSD, OpenH264

## Other BSD
:::::::::::::: {.columns}
::: {.column width="45%"}
### Zero-clause BSD
- Used by ToyBox
- Busybox is GPL-licensed
:::
::: {.column width="45%"}
### ISC license
- Similar to BSD
- OpenBSD
:::
::::::::::::::

## MIT license
- Also known as the Expat license
- Very similar to the simplified BSD license
- Used by .NET Core, Rails

# Modern permissive licenses

## Apache License 2.0
- Can't relicense unmodified parts
- Need to state what's been changed in changed files
- Grants a license to any patent
    - OpenBSD doesn't like this![^BSDCopy]
- Used by Kubernetes and PDF.js

[^BSDCopy]: http://www.openbsd.org/policy.html

## Other permissive licenses
:::::: {.columns}
::: {.column width="45%"}
### Satirical licenses
- WTFPL
- Beerware

### Permissive with reservations
- Commons clause (controversial!)
:::
::: {.column width="45%"}
### Public domain-ish
- Unlicense
- CC-0

### Zlib license
- Zlib and libpng
- Require license notice in source distributions
- May not be misrepresented
:::
::::::


## Mozilla Public License 2.0
- Grants patent rights, just like Apache license
- A weak copyleft license
    - "File-level copyleft"
    - Combined works may be proprietary
    - But original MPL licensed works must be freely available
- Explicitly compatible with the GPLs

- Used by Firefox, Syncthing, LibreOffice
