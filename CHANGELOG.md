# v1.3.1
- Removed not working background mode for xmrigMiner/xmrigDaemon on *nix systems -> use screen/tmux or systemd service instead
- Added cpu socket to client Id tooltip on dashboard
- Fixed notification when sending command is successful or error
- Fixed #16 FreeBSD build
- Fixed miner to keep sending status to server when its not temp unavailable
- Fixed #10 CCServer spontaneously freezes and holds CPU 100%
- Merged latest xmrig master
# v1.3.0
- Fixed Soft-aes modes (av=3, av=4) Bug: #11
- Added static build for linux with old libc (CentOs 5/6, debian, ...)
- Added notification to Dashboard when miner went offline with toggleswitch
- Added multi config editor to Dashboard to modify config of multiple miners at once
- Fixed MSV_VER for latest Visual Studio builds
# v1.2.2
- Added select/deselect all to dashboard
- Fixed memory leaks in XmrigCCServer
# v1.2.1
- Refactored Dashboard to send one command to multiple miners and "beautified" dashboard
- Miner now publishs own config to XMRigCCServer on startup
- Added command to trigger miner to upload config to XMRigCCServer
- Added threads to miner info tooltip on client id
# v1.2.0
- Added configurability for thread based doublehash mode which helps you to use more of your l3 cache
- Memory optimizations / speed improvements
- Updated to latest XMRig (2.4.3) with ARM support
# v1.1.1
- Fixed table sorting for client id column on Dashboard
- Fixed Windows compilation with msys2 (gcc)
- Added ability to do static build of xmrigDaemon and xmrigMiner
- Added client version to Dashboard client id tooltip
- Added update checker to Dashboard with notification bar 
# v1.1.0
- Added option to hide offline miners from Dashboard
- Added online status indicator to Dashboard client id column (green:red)
- JSON-Protocol changes to send miner info to XMRigCC server
- Added Tooltip to Dashboard column id containing new miner info (CPU, CPU flags, Cores, Threads, Memory, External IP, ...)
- Moved CCClient to own thread and changed ControlCommand processing to async to improve performance
# v1.0.9
- Integrated cpp-httplib as libcurl replacement 
- Removed libcurl dependicies
- Fixed round of avgTime in Dashboard
- Removed subrepo dependencies for easier building
# v1.0.8
- Extracted common CC files to subrepo (xmrigCC-common)
- Added sum row to Dashboard
- Added dialogs (success/error) to all dashboard actions
# v1.0.7
- CCClient status update interval is now configurable
- Updated to latest head of xmrig (Optimized soft aes)
# v1.0.6
- Fixed launch in folder containing spaces (Win)
# v1.0.5
- Merged latest changes of XMRig
- Added current algo to dashboard
- Added editor for client configs to dashboard
- some cosmetics on dashboard
# v1.0.4
- Updated XMRig to 2.4.2
- Fixed "--background" not working for xmrigCCServer on Windows
# v1.0.3
- Integrated build for Windows x64
# v1.0.2
- Reenabled restart in daemon for win/linux
# v1.0.1
- Fixed windows build
# v1.0.0
- Initial public release based on xmrig version 2.4.1
