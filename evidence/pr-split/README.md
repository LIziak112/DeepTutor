# Historical local acceptance evidence for the desktop split

This evidence branch is **not a merge candidate**. Its parent is the exact previously local integration commit `c21133a98bcf845b6e8845032b6282fbd315a063` (tree `1c0c008fc16795468cd167f739736b14d20e62cb`), now reachable through this branch. It combines prerequisite, sidebar, startup, placement and zoom, but **does not include the menu redesign** or the later review fixes. No signing keys, generated runtime bundle, user workspace, or installer binary are committed here.

- `sidebar-*-598dcf045.png`: Playwright on the production Web build on Windows, 1440/390px. This is browser coverage, not native Electron acceptance.
- `startup-c21133a98.png`, `zoom-*-c21133a98.png`: actual Windows portable application at 125% scaling, cold profile and fresh process relaunch. Screenshots show the private startup page or live application contents, not a full native-frame recording. The JSON gives measured shell/content zoom; screenshots alone cannot prove those factors. Largest-overlap geometry is not certified by these images.
- `menu-titlebar-f53a8e411.png`: actual private shell with native menu popup interaction, isolated no-seed profile. This does not establish editing shortcuts or live settings with a packaged core.

The source commits in the filenames identify the observations. These are historical local results, not CI results and not certification of later corrected HEADs. Native 100%/150%, mixed-DPI crossing, unplugging, native frame flash, and macOS menu acceptance remain incomplete. The initial NSIS trial timed out on chat-editor readiness; an unchanged-installer diagnostic rerun passed. Do not replace pending gates with these images.
