karthikeyan6379
===============

Crashed several times

qBittorrent version: v3.0.11
Libtorrent version: 0.16.10.0
Qt version: 4.8.5
Boost version: 1.54.0


```
#  0 qbittorrent.exe      0x00e5fb00  straceWin::getBacktrace()
#  1 qbittorrent.exe      0x00e60e6f  sigsegvHandler(__formal)
#  2 qbittorrent.exe      0x014c5af5  _XcptFilter(xcptnum, pxcptinfoptrs)
#  3 qbittorrent.exe      0x014b55bd  __tmainCRTStartup()
#  4 qbittorrent.exe      0x014c6de0  _EH4_CallFilterFunc()
#  5 qbittorrent.exe      0x014b678e  _except_handler4(ExceptionRecord, EstablisherFrame, ContextRecord, DispatcherContext)
#  6 ntdll.dll            0x771c71f9  RtlRaiseStatus()
#  7 ntdll.dll            0x771c71cb  RtlRaiseStatus()
#  8 ntdll.dll            0x771c7057  KiUserExceptionDispatcher()
#  9 ntdll.dll            0x771d2ce8  RtlFreeHeap()
# 10 kernel32.dll         0x755ec3d4  HeapFree()
# 11 qbittorrent.exe      0x014b364b  free(pBlock)
# 12 qbittorrent.exe      0x0128f3e3  QVectorData::free()
# 13 qbittorrent.exe      0x00fb694e  QVector::~QVector()
# 14 qbittorrent.exe      0x0102429f  QRegion::cleanUp()
# 15 qbittorrent.exe      0x010242d0  QRegion::~QRegion()
# 16 qbittorrent.exe      0x00f30f4b  QWidgetPrivate::paintSiblingsRecursive()
# 17 qbittorrent.exe      0x00f30a14  QWidgetPrivate::drawWidget()
# 18 qbittorrent.exe      0x00f30f3f  QWidgetPrivate::paintSiblingsRecursive()
# 19 qbittorrent.exe      0x00f30a14  QWidgetPrivate::drawWidget()
# 20 qbittorrent.exe      0x00f30f3f  QWidgetPrivate::paintSiblingsRecursive()
# 21 qbittorrent.exe      0x00f30a14  QWidgetPrivate::drawWidget()
# 22 qbittorrent.exe      0x00f30f3f  QWidgetPrivate::paintSiblingsRecursive()
# 23 qbittorrent.exe      0x00f30a14  QWidgetPrivate::drawWidget()
# 24 qbittorrent.exe      0x00f30f3f  QWidgetPrivate::paintSiblingsRecursive()
# 25 qbittorrent.exe      0x00f30a14  QWidgetPrivate::drawWidget()
# 26 qbittorrent.exe      0x0106c2a3  QWidgetBackingStore::sync()
# 27 qbittorrent.exe      0x00f2c371  QWidgetPrivate::syncBackingStore()
# 28 qbittorrent.exe      0x00f3440d  QWidget::event()
# 29 qbittorrent.exe      0x0101e478  QMainWindow::event()
# 30 qbittorrent.exe      0x00e78a98  MainWindow::event(e)
# 31 qbittorrent.exe      0x00f23d97  QApplicationPrivate::notify_helper()
# 32 qbittorrent.exe      0x00f2275f  QApplication::notify()
# 33 qbittorrent.exe      0x00e8611a  SessionApplication::notify(receiver, event)
# 34 qbittorrent.exe      0x0128a377  QCoreApplication::notifyInternal()
# 35 qbittorrent.exe      0x00f266db  QCoreApplication::sendEvent()
# 36 qbittorrent.exe      0x0128a9b9  QCoreApplicationPrivate::sendPostedEvents()
# 37 qbittorrent.exe      0x012de41c  qt_internal_proc()
# 38 USER32.dll           0x765dc4e7  gapfnScSendMessage()
# 39 USER32.dll           0x765dc5e7  gapfnScSendMessage()
# 40 USER32.dll           0x765dcc19  gapfnScSendMessage()
# 41 USER32.dll           0x765dcc70  DispatchMessageW()
# 42 qbittorrent.exe      0x012deefc  QEventDispatcherWin32::processEvents()
# 43 qbittorrent.exe      0x0103ec8c  QGuiEventDispatcherWin32::processEvents()
# 44 qbittorrent.exe      0x012d6bce  QEventLoop::processEvents()
# 45 qbittorrent.exe      0x012d6cb4  QEventLoop::exec()
# 46 qbittorrent.exe      0x0128a5a4  QCoreApplication::exec()
# 47 qbittorrent.exe      0x00e61f10  main(argc, argv)
# 48 qbittorrent.exe      0x01312924  WinMain()
# 49 qbittorrent.exe      0x014b5594  __tmainCRTStartup()
# 50 kernel32.dll         0x755eed6c  BaseThreadInitThunk()
# 51 ntdll.dll            0x771e37eb  RtlInitializeExceptionChain()
# 52 ntdll.dll            0x771e37be  RtlInitializeExceptionChain()


List of linked Modules:
qbittorrent    0x00dd0000    Image: C:\Program Files\qBittorrent\qbittorrent.exe
                                    .\qbittorrent.pdb
ntdll          0x77180000    Image: C:\Windows\SYSTEM32\ntdll.dll
kernel32       0x755a0000    Image: C:\Windows\system32\kernel32.dll
KERNELBASE     0x75250000    Image: C:\Windows\system32\KERNELBASE.dll
dbghelp        0x67e30000    Image: C:\Windows\system32\dbghelp.dll
msvcrt         0x766e0000    Image: C:\Windows\system32\msvcrt.dll
ADVAPI32       0x76dc0000    Image: C:\Windows\system32\ADVAPI32.dll
sechost        0x75580000    Image: C:\Windows\SYSTEM32\sechost.dll
RPCRT4         0x76a10000    Image: C:\Windows\system32\RPCRT4.dll
SHELL32        0x75880000    Image: C:\Windows\system32\SHELL32.dll
SHLWAPI        0x77330000    Image: C:\Windows\system32\SHLWAPI.dll
GDI32          0x764d0000    Image: C:\Windows\system32\GDI32.dll
USER32         0x765c0000    Image: C:\Windows\system32\USER32.dll
LPK            0x772c0000    Image: C:\Windows\system32\LPK.dll
USP10          0x76520000    Image: C:\Windows\system32\USP10.dll
POWRPROF       0x74500000    Image: C:\Windows\system32\POWRPROF.dll
SETUPAPI       0x76c20000    Image: C:\Windows\system32\SETUPAPI.dll
CFGMGR32       0x752a0000    Image: C:\Windows\system32\CFGMGR32.dll
OLEAUT32       0x76ac0000    Image: C:\Windows\system32\OLEAUT32.dll
ole32          0x77020000    Image: C:\Windows\system32\ole32.dll
DEVOBJ         0x754a0000    Image: C:\Windows\system32\DEVOBJ.dll
COMDLG32       0x76950000    Image: C:\Windows\system32\COMDLG32.dll
COMCTL32       0x73ba0000    Image: C:\Windows\WinSxS\x86_microsoft.windows.common-controls_6595b64144ccf1df_6.0.7601.17514_none_41e6975e2bd6f2b2\COMCTL32.dll
IMM32          0x772d0000    Image: C:\Windows\system32\IMM32.dll
MSCTF          0x76b50000    Image: C:\Windows\system32\MSCTF.dll
WINMM          0x73690000    Image: C:\Windows\system32\WINMM.dll
WS2_32         0x769d0000    Image: C:\Windows\system32\WS2_32.dll
NSI            0x77390000    Image: C:\Windows\system32\NSI.dll
MSWSOCK        0x74c00000    Image: C:\Windows\system32\MSWSOCK.dll
CRYPT32        0x75370000    Image: C:\Windows\system32\CRYPT32.dll
MSASN1         0x75230000    Image: C:\Windows\system32\MSASN1.dll
SspiCli        0x750d0000    Image: C:\Windows\system32\SspiCli.dll
uxtheme        0x73ad0000    Image: C:\Windows\system32\uxtheme.dll
spCapBtn       0x03040000    Image: C:\PROGRA~1\KASPER~1\KASPER~1\KASPER~2\MODULE~1\spCapBtn.dll
msimg32        0x6c590000    Image: C:\Windows\system32\msimg32.dll
version        0x746c0000    Image: C:\Windows\system32\version.dll
wininet        0x76e60000    Image: C:\Windows\system32\wininet.dll
api-ms-win-downlevel-user32-l1- 0x752d0000    Image: C:\Windows\system32\api-ms-win-downlevel-user32-l1-1-0.dll
api-ms-win-downlevel-advapi32-l 0x754f0000    Image: C:\Windows\system32\api-ms-win-downlevel-advapi32-l1-1-0.dll
api-ms-win-downlevel-shlwapi-l1 0x75500000    Image: C:\Windows\system32\api-ms-win-downlevel-shlwapi-l1-1-0.dll
api-ms-win-downlevel-version-l1 0x75510000    Image: C:\Windows\system32\api-ms-win-downlevel-version-l1-1-0.dll
api-ms-win-downlevel-normaliz-l 0x75490000    Image: C:\Windows\system32\api-ms-win-downlevel-normaliz-l1-1-0.dll
normaliz       0x772f0000    Image: C:\Windows\system32\normaliz.DLL
iertutil       0x75680000    Image: C:\Windows\system32\iertutil.dll
dwmapi         0x73380000    Image: C:\Windows\system32\dwmapi.dll
ntmarta        0x73f80000    Image: C:\Windows\system32\ntmarta.dll
WLDAP32        0x76690000    Image: C:\Windows\system32\WLDAP32.dll
PSAPI          0x773a0000    Image: C:\Windows\system32\PSAPI.dll
CRYPTBASE      0x75140000    Image: C:\Windows\system32\CRYPTBASE.dll
userenv        0x74820000    Image: C:\Windows\system32\userenv.dll
profapi        0x751c0000    Image: C:\Windows\system32\profapi.dll
CRYPTSP        0x74c40000    Image: C:\Windows\system32\CRYPTSP.dll
rsaenh         0x749e0000    Image: C:\Windows\system32\rsaenh.dll
wship6         0x74bf0000    Image: C:\Windows\System32\wship6.dll
wshqos         0x730f0000    Image: C:\Windows\System32\wshqos.dll
wshtcpip       0x74750000    Image: C:\Windows\system32\wshtcpip.DLL
DNSAPI         0x74ac0000    Image: C:\Windows\system32\DNSAPI.dll
mdnsNSP        0x16080000    Image: C:\Program Files\Bonjour\mdnsNSP.dll
Iphlpapi       0x73630000    Image: C:\Windows\system32\Iphlpapi.DLL
WINNSI         0x737c0000    Image: C:\Windows\system32\WINNSI.DLL
rasadhlp       0x70430000    Image: C:\Windows\system32\rasadhlp.dll
fwpuclnt       0x73650000    Image: C:\Windows\System32\fwpuclnt.dll
RpcRtRemote    0x75150000    Image: C:\Windows\system32\RpcRtRemote.dll
comctl32       0x6ed30000    Image: C:\Windows\WinSxS\x86_microsoft.windows.common-controls_6595b64144ccf1df_5.82.7601.17514_none_ec83dffa859149af\comctl32.dll
```
