# Steam-Error
Process:               steam_osx [1037]
Path:                  /Applications/Steam.app/Contents/MacOS/steam_osx
Identifier:            com.valvesoftware.steam
Version:               1.5
Code Type:             X86 (Native)
Parent Process:        ??? [1]
Responsible:           steam_osx [1037]
User ID:               502

Date/Time:             2018-01-24 14:27:21.137 -0500
OS Version:            Mac OS X 10.13.3 (17D47)
Report Version:        12
Anonymous UUID:        8735419C-1B11-0F06-9A01-F531D4B9C7AE

Sleep/Wake UUID:       0CA95D1D-81E7-4A7F-8D39-ED41F360CDF7

Time Awake Since Boot: 11000 seconds
Time Since Wake:       520 seconds

System Integrity Protection: enabled

Crashed Thread:        0

Exception Type:        EXC_BAD_ACCESS (SIGBUS)
Exception Codes:       KERN_MEMORY_ERROR at 0x00000000a088b014
Exception Note:        EXC_CORPSE_NOTIFY

Termination Signal:    Bus error: 10
Termination Reason:    Namespace SIGNAL, Code 0xa
Terminating Process:   exc handler [0]

VM Regions Near 0xa088b014:
    __LINKEDIT             000000000043c000-0000000000456000 [  104K] r--/rwx SM=COW  /usr/lib/dyld
--> Submap                 0000000090000000-00000000b0000000 [512.0M] r--/rwx SM=SHM  machine-wide VM submap
    mapped file            0000000090000000-0000000090298000 [ 2656K] r-x/r-x SM=COW  

Application Specific Information:
dyld: launch, loading dependent libraries
/System/Library/PrivateFrameworks/DesktopServicesPriv.framework/Versions/A/DesktopServicesPriv

Thread 0 Crashed:
0   dyld                          	0x003e06ce ImageLoaderMachO::sniffLoadCommands(macho_header const*, char const*, bool, bool*, unsigned int*, unsigned int*, ImageLoader::LinkContext const&, linkedit_data_command const**, encryption_info_command const**) + 40
1   dyld                          	0x003e1a56 ImageLoaderMachO::instantiateFromCache(macho_header const*, char const*, long, stat const&, ImageLoader::LinkContext const&) + 48
2   dyld                          	0x003d75cb dyld::loadPhase5(char const*, char const*, dyld::LoadContext const&, unsigned int&, std::__1::vector<char const*, std::__1::allocator<char const*> >*) + 721
3   dyld                          	0x003d72e3 dyld::loadPhase4(char const*, char const*, dyld::LoadContext const&, unsigned int&, std::__1::vector<char const*, std::__1::allocator<char const*> >*) + 155
4   dyld                          	0x003d70a2 dyld::loadPhase3(char const*, char const*, dyld::LoadContext const&, unsigned int&, std::__1::vector<char const*, std::__1::allocator<char const*> >*) + 1451
5   dyld                          	0x003d6879 dyld::loadPhase1(char const*, char const*, dyld::LoadContext const&, unsigned int&, std::__1::vector<char const*, std::__1::allocator<char const*> >*) + 139
6   dyld                          	0x003d082b dyld::loadPhase0(char const*, char const*, dyld::LoadContext const&, unsigned int&, std::__1::vector<char const*, std::__1::allocator<char const*> >*) + 187
7   dyld                          	0x003d04b2 dyld::load(char const*, dyld::LoadContext const&, unsigned int&) + 194
8   dyld                          	0x003d7ed3 dyld::libraryLocator(char const*, bool, char const*, ImageLoader::RPathChain const*, unsigned int&) + 65
9   dyld                          	0x003dec72 ImageLoader::recursiveLoadLibraries(ImageLoader::LinkContext const&, bool, ImageLoader::RPathChain const&, char const*) + 666
10  dyld                          	0x003dee63 ImageLoader::recursiveLoadLibraries(ImageLoader::LinkContext const&, bool, ImageLoader::RPathChain const&, char const*) + 1163
11  dyld                          	0x003dee63 ImageLoader::recursiveLoadLibraries(ImageLoader::LinkContext const&, bool, ImageLoader::RPathChain const&, char const*) + 1163
12  dyld                          	0x003dee63 ImageLoader::recursiveLoadLibraries(ImageLoader::LinkContext const&, bool, ImageLoader::RPathChain const&, char const*) + 1163
13  dyld                          	0x003ddf63 ImageLoader::link(ImageLoader::LinkContext const&, bool, bool, bool, ImageLoader::RPathChain const&, char const*) + 93
14  dyld                          	0x003d202d dyld::link(ImageLoader*, bool, bool, ImageLoader::RPathChain const&, unsigned int) + 177
15  dyld                          	0x003d42bb dyld::_main(macho_header const*, unsigned long, int, char const**, char const**, char const**, unsigned long*) + 7029
16  dyld                          	0x003ce427 dyldbootstrap::start(macho_header const*, int, char const**, long, macho_header const*, unsigned long*) + 374
17  dyld                          	0x003ce277 _dyld_start + 71

Thread 0 crashed with X86 Thread State (32-bit):
  eax: 0x00000000  ebx: 0xbffd1bfb  ecx: 0xbffd1bf4  edx: 0xa088b000
  edi: 0xbffd1be8  esi: 0xbffd1bf0  ebp: 0xbffd1ba8  esp: 0xbffd1b30
   ss: 0x00000023  efl: 0x00010246  eip: 0x003e06ce   cs: 0x0000001b
   ds: 0x00000023   es: 0x00000023   fs: 0x00000000   gs: 0x0000000f
  cr2: 0xa088b014
  
Logical CPU:     1
Error Code:      0x00000004
Trap Number:     14


Binary Images:
   0x2d000 -   0x293fc3 +com.valvesoftware.steam (1.5) <080E1C9B-4DE9-3F59-924D-2B65BF76DEE5> /Applications/Steam.app/Contents/MacOS/steam_osx
  0x3cd000 -   0x412fdf  dyld (519.2.2) <7B7B05B7-204A-38FF-BD32-4CBB51752DD4> /usr/lib/dyld
0x90298000 - 0x90298fff  com.apple.Accelerate (1.11 - Accelerate 1.11) <F4A138F5-290D-3413-AD17-ECD395935FF3> /System/Library/Frameworks/Accelerate.framework/Versions/A/Accelerate
0x902b0000 - 0x909f1fdf  com.apple.vImage (8.1 - ???) <591C941E-6475-347E-89DA-F541E88F949A> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vImage.framework/Versions/A/vImage
0x909f2000 - 0x90b2dff7  libBLAS.dylib (1211.30.1) <A850E0E2-3A72-3916-9907-AF1E7ECC95F0> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libBLAS.dylib
0x90b2e000 - 0x90b5bffb  libBNNS.dylib (37) <C29094A0-5C89-3C5E-AB37-510C28588E2E> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libBNNS.dylib
0x90b5c000 - 0x90ecffff  libLAPACK.dylib (1211.30.1) <2DDDE838-0FF1-3679-8E62-9C09923ECB7E> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libLAPACK.dylib
0x90ed0000 - 0x90ee6ffb  libLinearAlgebra.dylib (1211.30.1) <8A120E75-CAF4-3CAE-BBE6-E2F5FAE44DB8> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libLinearAlgebra.dylib
0x90ee7000 - 0x90f00ff7  libSparseBLAS.dylib (1211.30.1) <0C5E0EF4-E9A5-3FC4-B7A3-1FE59DB4A2AA> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libSparseBLAS.dylib
0x90f01000 - 0x9105ffc7  libvDSP.dylib (622.20.8) <C5F16300-061F-3DF0-B91E-8BD0D2173351> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libvDSP.dylib
0x91060000 - 0x9113effb  libvMisc.dylib (622.20.8) <1C8D5D80-F32C-3853-8309-57C8A82B7DA5> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libvMisc.dylib
0x9113f000 - 0x9113ffff  com.apple.Accelerate.vecLib (3.11 - vecLib 3.11) <7A0D5DD6-C302-390D-9178-0B2EA94BB5ED> /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/vecLib
0x91333000 - 0x920f4ffb  com.apple.AppKit (6.9 - 1561.20.106) <12E4548C-75C1-366C-A7A1-BD2701C5B67C> /System/Library/Frameworks/AppKit.framework/Versions/C/AppKit
0x92146000 - 0x92146fff  com.apple.ApplicationServices (48 - 50) <BFE7FB45-365B-341F-A8FC-B9483AE87709> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/ApplicationServices
0x92147000 - 0x921adff3  com.apple.ApplicationServices.ATS (377 - 445) <CD3D5685-2BB9-3A7B-AC97-2A74A81CB7CC> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/ATS.framework/Versions/A/ATS
0x921b0000 - 0x922d4ff3  libFontParser.dylib (222.1.2) <8F7D388A-299C-3C6D-9864-40EC0914A96B> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/ATS.framework/Versions/A/Resources/libFontParser.dylib
0x922d5000 - 0x92321ffb  libFontRegistry.dylib (221) <8D81FDCF-F05D-3556-AB6D-090F9508C25E> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/ATS.framework/Versions/A/Resources/libFontRegistry.dylib
0x9240f000 - 0x92414fff  com.apple.ColorSyncLegacy (4.13.0 - 1) <AB5CE7D2-8BE5-35C8-A9D5-ED0FB5BAB7D1> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/ColorSyncLegacy.framework/Versions/A/ColorSyncLegacy
0x924be000 - 0x92515ff7  com.apple.HIServices (1.22 - 622) <8544026A-17BE-301D-BA2A-782F3AD864DA> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/HIServices.framework/Versions/A/HIServices
0x92516000 - 0x92525ff7  com.apple.LangAnalysis (1.7.0 - 1.7.0) <E3245701-039B-353F-923D-F81B2242842C> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/LangAnalysis.framework/Versions/A/LangAnalysis
0x92526000 - 0x9257effb  com.apple.print.framework.PrintCore (13 - 503) <FD0F7A18-6F78-34C9-B067-B3AB76C3D4C8> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/PrintCore.framework/Versions/A/PrintCore
0x9257f000 - 0x92615ffb  com.apple.QD (3.12 - 403) <372AFF26-17D1-3C6F-9E47-17C955C2045B> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/QD.framework/Versions/A/QD
0x92616000 - 0x92622ff3  com.apple.speech.synthesis.framework (7.4.1 - 7.4.1) <3AE4F801-4A2D-3AB3-AA31-B27F7A7131F4> /System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/SpeechSynthesis.framework/Versions/A/SpeechSynthesis
0x92623000 - 0x9286ffff  com.apple.audio.toolbox.AudioToolbox (1.14 - 1.14) <E4585EFD-C3B6-327F-88E4-B3BADDA6B08D> /System/Library/Frameworks/AudioToolbox.framework/Versions/A/AudioToolbox
0x92b8f000 - 0x92efcffb  com.apple.CFNetwork (893.13.1 - 893.13.1) <63A5C550-5F0F-3FF1-9061-55E1766B3512> /System/Library/Frameworks/CFNetwork.framework/Versions/A/CFNetwork
0x92f11000 - 0x92f11fff  com.apple.Carbon (158 - 158) <1545E2E8-F562-33D6-8DA7-5FD34045B314> /System/Library/Frameworks/Carbon.framework/Versions/A/Carbon
0x92f12000 - 0x92f1bff3  com.apple.audio.SoundManager (4.2 - 4.2) <83AE7AA9-8661-3449-99F4-291A42640692> /System/Library/Frameworks/Carbon.framework/Versions/A/Frameworks/CarbonSound.framework/Versions/A/CarbonSound
0x92f1c000 - 0x92f20fff  com.apple.CommonPanels (1.2.6 - 98) <DA1D99A4-53F6-31AF-964D-86739FA74B52> /System/Library/Frameworks/Carbon.framework/Versions/A/Frameworks/CommonPanels.framework/Versions/A/CommonPanels
0x92f21000 - 0x932b7ffb  com.apple.HIToolbox (2.1.1 - 910.4) <7BBA4C0C-AB6B-3FBD-BB54-5346BEC2DF58> /System/Library/Frameworks/Carbon.framework/Versions/A/Frameworks/HIToolbox.framework/Versions/A/HIToolbox
0x932b8000 - 0x9330cffb  com.apple.htmlrendering (77 - 1.1.4) <BAF5C846-FF50-3C80-97F5-71F1399CA85C> /System/Library/Frameworks/Carbon.framework/Versions/A/Frameworks/HTMLRendering.framework/Versions/A/HTMLRendering
0x9330d000 - 0x93310fff  com.apple.help (1.3.8 - 64) <1E913488-5D7B-388E-904D-64EF8C99E704> /System/Library/Frameworks/Carbon.framework/Versions/A/Frameworks/Help.framework/Versions/A/Help
0x93311000 - 0x93316ffb  com.apple.ImageCapture (9.0 - 9.0) <1887749B-D641-3057-B91F-3C2D8E990115> /System/Library/Frameworks/Carbon.framework/Versions/A/Frameworks/ImageCapture.framework/Versions/A/ImageCapture
0x93317000 - 0x933b1ffb  com.apple.ink.framework (10.9 - 220) <5340E055-BD3D-35AD-9797-F22E1ECEDAC6> /System/Library/Frameworks/Carbon.framework/Versions/A/Frameworks/Ink.framework/Versions/A/Ink
0x933b2000 - 0x933ecfff  com.apple.NavigationServices (3.8 - 227) <6B1000C3-9C00-33F5-88D5-62F6BD5DD7F8> /System/Library/Frameworks/Carbon.framework/Versions/A/Frameworks/NavigationServices.framework/Versions/A/NavigationServices
0x933ed000 - 0x93408ffb  com.apple.openscripting (1.7 - 174) <CD281A8D-54C8-3201-B9F7-DE2439088302> /System/Library/Frameworks/Carbon.framework/Versions/A/Frameworks/OpenScripting.framework/Versions/A/OpenScripting
0x93409000 - 0x9340efff  com.apple.print.framework.Print (12 - 267) <F7BEF8BA-7D1F-34A2-97B8-D49F20886644> /System/Library/Frameworks/Carbon.framework/Versions/A/Frameworks/Print.framework/Versions/A/Print
0x9340f000 - 0x93411fff  com.apple.securityhi (9.0 - 55006) <E9FF8254-B8E1-312A-8FC3-2B4EA8CE9AEA> /System/Library/Frameworks/Carbon.framework/Versions/A/Frameworks/SecurityHI.framework/Versions/A/SecurityHI
0x93412000 - 0x93418fff  com.apple.speech.recognition.framework (6.0.3 - 6.0.3) <1C27FB7B-A467-3171-A73B-8C9B403028E1> /System/Library/Frameworks/Carbon.framework/Versions/A/Frameworks/SpeechRecognition.framework/Versions/A/SpeechRecognition
0x93426000 - 0x934e5ff7  com.apple.ColorSync (4.13.0 - 546) <DACC5623-8E37-3134-9562-4E8601127F67> /System/Library/Frameworks/ColorSync.framework/Versions/A/ColorSync
0x934e6000 - 0x93581fff  com.apple.audio.CoreAudio (4.3.0 - 4.3.0) <ABA90687-71A6-3431-94A1-0E7E74FE407C> /System/Library/Frameworks/CoreAudio.framework/Versions/A/CoreAudio
0x935e5000 - 0x938c5fff  com.apple.CoreData (120 - 849.2) <B8011F5E-7A2B-349B-AFF1-17EC8D8465AB> /System/Library/Frameworks/CoreData.framework/Versions/A/CoreData
0x938c6000 - 0x938ccff3  com.apple.CoreDisplay (1.0 - 81.7) <E6BFD0F5-A45B-3FE3-BA26-14D2CD970CFF> /System/Library/Frameworks/CoreDisplay.framework/Versions/A/CoreDisplay
0x938cd000 - 0x93d56ff7  com.apple.CoreFoundation (6.9 - 1451) <727B43E3-A1AC-31EC-97A4-F179FE11D04A> /System/Library/Frameworks/CoreFoundation.framework/Versions/A/CoreFoundation
0x93d58000 - 0x94387ffb  com.apple.CoreGraphics (2.0 - 1129.5) <20752785-E9DA-3CC6-ACDD-5A82AD344209> /System/Library/Frameworks/CoreGraphics.framework/Versions/A/CoreGraphics
0x94389000 - 0x945ffffb  com.apple.CoreImage (13.0.0 - 579.2.9) <2498F44C-7350-397B-A075-206A91D75ABB> /System/Library/Frameworks/CoreImage.framework/Versions/A/CoreImage
0x947f1000 - 0x947f1fff  com.apple.CoreServices (822.19 - 822.19) <6B5DC8C1-4237-3ADA-B8C8-F926943E6101> /System/Library/Frameworks/CoreServices.framework/Versions/A/CoreServices
0x947f2000 - 0x94864ff3  com.apple.AE (735.1 - 735.1) <3E1B0CED-0AC3-3252-AEDD-5D8F91E3AAA7> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/AE.framework/Versions/A/AE
0x94865000 - 0x94b43ffb  com.apple.CoreServices.CarbonCore (1178.2 - 1178.2) <E61EA71D-294F-3C8B-95BD-0CDBA0FFC907> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/CarbonCore.framework/Versions/A/CarbonCore
0x94b44000 - 0x94b78ff3  com.apple.DictionaryServices (1.2 - 284) <56BEF6B8-50D2-38A0-9EF2-D7093E9AAB56> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/DictionaryServices.framework/Versions/A/DictionaryServices
0x94b79000 - 0x94b81fff  com.apple.CoreServices.FSEvents (1239 - 1239) <CABC21F7-E3AB-3954-ACBE-B8066A37516A> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/FSEvents.framework/Versions/A/FSEvents
0x94b82000 - 0x94ce0fff  com.apple.LaunchServices (822.19 - 822.19) <AC40752F-0F99-3EB1-8D25-2C65F9BAC226> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/LaunchServices.framework/Versions/A/LaunchServices
0x94ce1000 - 0x94d8dff7  com.apple.Metadata (10.7.0 - 1191.2.6) <6CE69880-6AF3-3A1A-A8E0-F89FC750EE4C> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/Metadata.framework/Versions/A/Metadata
0x94d8e000 - 0x94decff7  com.apple.CoreServices.OSServices (822.19 - 822.19) <38B64F72-5CAE-374A-8BBC-0EAB7C6A6777> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/OSServices.framework/Versions/A/OSServices
0x94ded000 - 0x94e5eff3  com.apple.SearchKit (1.4.0 - 1.4.0) <FAD60011-970B-3889-B6BD-3715CCF599CA> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/SearchKit.framework/Versions/A/SearchKit
0x94e5f000 - 0x94e82fff  com.apple.coreservices.SharedFileList (71.4 - 71.4) <CD97E31D-0354-36AB-9997-C4FAF3221D30> /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/SharedFileList.framework/Versions/A/SharedFileList
0x94e83000 - 0x94fceffb  com.apple.CoreText (352.0 - 578.12) <6389222B-6B26-3F46-93C2-ABE07168227F> /System/Library/Frameworks/CoreText.framework/Versions/A/CoreText
0x94fcf000 - 0x95009ff3  com.apple.CoreVideo (1.8 - 279.2) <0D75C395-3C86-3539-9206-C7A330BE3551> /System/Library/Frameworks/CoreVideo.framework/Versions/A/CoreVideo
0x952e4000 - 0x952edff7  com.apple.DiskArbitration (2.7 - 2.7) <E3552A79-57A4-36AE-8B54-5FE2EB5193DA> /System/Library/Frameworks/DiskArbitration.framework/Versions/A/DiskArbitration
0x952fe000 - 0x9566dffb  com.apple.Foundation (6.9 - 1451) <E815D5AF-B627-3BF4-8156-4F514FCFD765> /System/Library/Frameworks/Foundation.framework/Versions/C/Foundation
0x956ae000 - 0x956ddff3  com.apple.GSS (4.0 - 2.0) <78C94D11-21DF-34C6-B4E8-88564551D67E> /System/Library/Frameworks/GSS.framework/Versions/A/GSS
0x95888000 - 0x95929ffb  com.apple.framework.IOKit (2.0.2 - 1445.40.1) <EDA5B2F5-12B4-39EF-B5EF-899587AACDC5> /System/Library/Frameworks/IOKit.framework/Versions/A/IOKit
0x9592b000 - 0x95932fff  com.apple.IOSurface (209.2.2 - 209.2.2) <0CCA9904-FCBB-3278-96A1-714BDB961D8A> /System/Library/Frameworks/IOSurface.framework/Versions/A/IOSurface
0x95987000 - 0x95b0bff3  com.apple.ImageIO.framework (3.3.0 - 1713) <28D21D61-3526-33ED-92DC-08D4D67445CB> /System/Library/Frameworks/ImageIO.framework/Versions/A/ImageIO
0x95b0c000 - 0x95b10ffb  libGIF.dylib (1713) <47A6BFCC-6651-3AAE-A70C-7BA3717B13BB> /System/Library/Frameworks/ImageIO.framework/Versions/A/Resources/libGIF.dylib
0x95b11000 - 0x95c02fff  libJP2.dylib (1713) <D1075C88-406B-3EAF-9270-9B3762D97803> /System/Library/Frameworks/ImageIO.framework/Versions/A/Resources/libJP2.dylib
0x95c03000 - 0x95c25ff7  libJPEG.dylib (1713) <EFD86068-C17E-32AD-B4A5-79C20BC93411> /System/Library/Frameworks/ImageIO.framework/Versions/A/Resources/libJPEG.dylib
0x95f06000 - 0x95f2cff7  libPng.dylib (1713) <A10259A1-2581-3642-946D-5B3F101615EC> /System/Library/Frameworks/ImageIO.framework/Versions/A/Resources/libPng.dylib
0x95f2d000 - 0x95f2fffb  libRadiance.dylib (1713) <EE872547-4C9F-397B-B41B-C79FEEE68267> /System/Library/Frameworks/ImageIO.framework/Versions/A/Resources/libRadiance.dylib
0x95f30000 - 0x95f7afff  libTIFF.dylib (1713) <7A56E3C4-9965-3471-8E98-5F6B28D68FBF> /System/Library/Frameworks/ImageIO.framework/Versions/A/Resources/libTIFF.dylib
0x96897000 - 0x968affff  com.apple.Kerberos (3.0 - 1) <8A399DB7-5440-3EC0-A241-3DD10E82DDB2> /System/Library/Frameworks/Kerberos.framework/Versions/A/Kerberos
0x96f27000 - 0x96f9dfff  com.apple.Metal (124.7 - 124.7) <2617CDD0-32C6-358C-A61F-063737F916B3> /System/Library/Frameworks/Metal.framework/Versions/A/Metal
0x96f9f000 - 0x96fabfff  com.apple.NetFS (6.0 - 4.0) <F37A4DA0-AAB6-3F0B-BA18-E322BFA52CC4> /System/Library/Frameworks/NetFS.framework/Versions/A/NetFS
0x99c78000 - 0x99cc3fff  com.apple.opencl (2.8.12 - 2.8.12) <9AC78C72-CBBC-3D29-B553-AACC28014AEC> /System/Library/Frameworks/OpenCL.framework/Versions/A/OpenCL
0x99cc4000 - 0x99ce0fff  com.apple.CFOpenDirectory (10.13 - 207) <255284C6-7BDD-3A0B-A4A2-E43206611B91> /System/Library/Frameworks/OpenDirectory.framework/Versions/A/Frameworks/CFOpenDirectory.framework/Versions/A/CFOpenDirectory
0x99ce1000 - 0x99cecfff  com.apple.OpenDirectory (10.13 - 207) <ECB33DA6-A0A3-3378-AB7A-2C10D395904E> /System/Library/Frameworks/OpenDirectory.framework/Versions/A/OpenDirectory
0x9aef6000 - 0x9aef7fff  libCVMSPluginSupport.dylib (16.4.2) <909D788E-692E-3FF1-AFF0-2AB4609C53D7> /System/Library/Frameworks/OpenGL.framework/Versions/A/Libraries/libCVMSPluginSupport.dylib
0x9aef8000 - 0x9aefcfff  libCoreFSCache.dylib (162.4) <D53B0D41-0774-3C6A-BB59-8BA7DB8A8374> /System/Library/Frameworks/OpenGL.framework/Versions/A/Libraries/libCoreFSCache.dylib
0x9aefd000 - 0x9af01fff  libCoreVMClient.dylib (162.4) <19767FEB-6A89-3892-8F18-1F9E73463050> /System/Library/Frameworks/OpenGL.framework/Versions/A/Libraries/libCoreVMClient.dylib
0x9af02000 - 0x9af0aff7  libGFXShared.dylib (16.4.2) <F62281F1-9495-3589-A576-75D84880D42D> /System/Library/Frameworks/OpenGL.framework/Versions/A/Libraries/libGFXShared.dylib
0x9af0b000 - 0x9af17fff  libGL.dylib (16.4.2) <028B909B-DD19-388B-8113-1850DFAD3DCA> /System/Library/Frameworks/OpenGL.framework/Versions/A/Libraries/libGL.dylib
0x9af18000 - 0x9af53ffb  libGLImage.dylib (16.4.2) <AE5E3974-656A-3F88-956E-F28192BA98C3> /System/Library/Frameworks/OpenGL.framework/Versions/A/Libraries/libGLImage.dylib
0x9b0cd000 - 0x9b10fff7  libGLU.dylib (16.4.2) <9E1283AA-A7E0-37BA-BDEB-EE5256D677C7> /System/Library/Frameworks/OpenGL.framework/Versions/A/Libraries/libGLU.dylib
0x9bab6000 - 0x9bac4fff  com.apple.opengl (16.4.2 - 16.4.2) <40645026-52DC-3CFC-8308-EFA2FA79D5A0> /System/Library/Frameworks/OpenGL.framework/Versions/A/OpenGL
0x9c829000 - 0x9ca5fff7  com.apple.QuartzCore (1.11 - 584.8.102) <960628B2-C498-36C9-B0D4-F27D49DE029F> /System/Library/Frameworks/QuartzCore.framework/Versions/A/QuartzCore
0x9cef8000 - 0x9d225ff3  com.apple.security (7.0 - 58286.41.2) <F64D64CD-4E80-3384-92F0-56D2A464F7B4> /System/Library/Frameworks/Security.framework/Versions/A/Security
0x9d226000 - 0x9d2adff3  com.apple.securityfoundation (6.0 - 55185.30.4) <632548B9-3E24-32F4-BF50-F6BF71713363> /System/Library/Frameworks/SecurityFoundation.framework/Versions/A/SecurityFoundation
0x9d2d9000 - 0x9d2ddfff  com.apple.xpc.ServiceManagement (1.0 - 1) <B09C1309-46A2-3081-B489-DCE549A8BA46> /System/Library/Frameworks/ServiceManagement.framework/Versions/A/ServiceManagement
0x9d408000 - 0x9d478ff3  com.apple.SystemConfiguration (1.17 - 1.17) <318C287A-BB41-3F72-9095-9DFF0382CB77> /System/Library/Frameworks/SystemConfiguration.framework/Versions/A/SystemConfiguration
0x9f26e000 - 0x9f305ff7  com.apple.APFS (1.0 - 1) <1B119C37-9A4C-3204-9BE2-E4E00E657037> /System/Library/PrivateFrameworks/APFS.framework/Versions/A/APFS
0x9fa4b000 - 0x9fa88ff3  com.apple.AppleJPEG (1.0 - 1) <E87393BB-6140-389C-BF53-36B3985A56D3> /System/Library/PrivateFrameworks/AppleJPEG.framework/Versions/A/AppleJPEG
0x9fbdb000 - 0x9fbe2fff  com.apple.coreservices.BackgroundTaskManagement (1.0 - 57.1) <71FD5EA2-8D0B-3E21-94E4-6D5BD45005E7> /System/Library/PrivateFrameworks/BackgroundTaskManagement.framework/Versions/A/BackgroundTaskManagement
0x9fdb2000 - 0x9fdbbffb  com.apple.CommonAuth (4.0 - 2.0) <424B8D39-396A-3A78-84C1-5161B54A8F5B> /System/Library/PrivateFrameworks/CommonAuth.framework/Versions/A/CommonAuth
0xa022d000 - 0xa023dff7  com.apple.CoreEmoji (1.0 - 69.3) <165A133F-DED4-3B24-A9BF-6EA6F3F7A152> /System/Library/PrivateFrameworks/CoreEmoji.framework/Versions/A/CoreEmoji
0xa0490000 - 0xa05b6fe3  com.apple.coreui (2.1 - 492.2) <4B915963-6D32-3D89-B585-94094ACCF2E8> /System/Library/PrivateFrameworks/CoreUI.framework/Versions/A/CoreUI
0xa0c96000 - 0xa10c6ff7  com.apple.vision.FaceCore (3.3.2 - 3.3.2) <B2288C3D-E67F-3AAE-A652-E920CD19F267> /System/Library/PrivateFrameworks/FaceCore.framework/Versions/A/FaceCore
0xa3a6a000 - 0xa3addff3  com.apple.Heimdal (4.0 - 2.0) <560C8A98-E261-39C9-9862-3340EC6ABC9C> /System/Library/PrivateFrameworks/Heimdal.framework/Versions/A/Heimdal
0xa3d8f000 - 0xa3d95fff  com.apple.IOAccelerator (376.6 - 376.6) <4EFED596-8863-35F6-8EA3-CB11C5D9D157> /System/Library/PrivateFrameworks/IOAccelerator.framework/Versions/A/IOAccelerator
0xa3d96000 - 0xa3daeffb  com.apple.IOPresentment (1.0 - 32.1) <EBD4DB8D-03D3-3136-B431-969A2E5E1B91> /System/Library/PrivateFrameworks/IOPresentment.framework/Versions/A/IOPresentment
0xa3e62000 - 0xa3f56ff7  com.apple.LanguageModeling (1.0 - 159.3.1) <AA880B14-031D-33FB-9B48-0A8AAB7342C6> /System/Library/PrivateFrameworks/LanguageModeling.framework/Versions/A/LanguageModeling
0xa3f57000 - 0xa3f98ff7  com.apple.Lexicon-framework (1.0 - 33.2) <13FAB8A2-507A-3AEA-A571-27BDDFD96B31> /System/Library/PrivateFrameworks/Lexicon.framework/Versions/A/Lexicon
0xa3f9c000 - 0xa3fa2ff3  com.apple.LinguisticData (1.0 - 238.3) <C47B3EB0-0463-3613-8A09-344F1639EE92> /System/Library/PrivateFrameworks/LinguisticData.framework/Versions/A/LinguisticData
0xa4346000 - 0xa436fffb  com.apple.MultitouchSupport.framework (1204.13 - 1204.13) <01BDF9A5-8C83-3611-A999-F43F9121A173> /System/Library/PrivateFrameworks/MultitouchSupport.framework/Versions/A/MultitouchSupport
0xa448e000 - 0xa4498fff  com.apple.NetAuth (6.2 - 6.2) <52F67DC1-8C96-3944-8E54-C02DD51FD9FC> /System/Library/PrivateFrameworks/NetAuth.framework/Versions/A/NetAuth
0xa4849000 - 0xa48ceffb  com.apple.SkyLight (1.600.0 - 312.23.4) <27154D6B-3C0F-383F-AA7B-F602C1F397CC> /System/Library/PrivateFrameworks/SkyLight.framework/Versions/A/SkyLight
0xa4cac000 - 0xa4cb3fff  com.apple.TCC (1.0 - 1) <4B76752A-36A0-3175-87C7-CB42E33CCB5A> /System/Library/PrivateFrameworks/TCC.framework/Versions/A/TCC
0xa544d000 - 0xa544ffff  com.apple.loginsupport (1.0 - 1) <086FAE1B-87E2-324A-AE76-E6EC0B5F1517> /System/Library/PrivateFrameworks/login.framework/Versions/A/Frameworks/loginsupport.framework/Versions/A/loginsupport
0xa54da000 - 0xa550dff7  libclosured.dylib (519.2.2) <E0E52FC3-51A9-385F-953D-23A7CA8D5666> /usr/lib/closure/libclosured.dylib
0xa555d000 - 0xa5594ff3  libCRFSuite.dylib (41) <7F584902-74F1-3362-935D-95F5E735F5E7> /usr/lib/libCRFSuite.dylib
0xa5595000 - 0xa559fffb  libChineseTokenizer.dylib (28) <1FF5A32D-E012-3E76-B738-FAC26AD2A39B> /usr/lib/libChineseTokenizer.dylib
0xa563b000 - 0xa563cfff  libDiagnosticMessagesClient.dylib (104) <6829B180-2556-3A7E-A2E6-BD4859DF30A7> /usr/lib/libDiagnosticMessagesClient.dylib
0xa566e000 - 0xa5858ff7  libFosl_dynamic.dylib (17.7) <DBE4D720-8A46-3879-AD2D-F9A8CE3E7476> /usr/lib/libFosl_dynamic.dylib
0xa5860000 - 0xa5860fff  libOpenScriptingUtil.dylib (174) <B7CEDC30-2D17-3896-9EFC-64DB3D11DF00> /usr/lib/libOpenScriptingUtil.dylib
0xa58af000 - 0xa58b0fff  libSystem.B.dylib (1252) <D7139382-C03A-377B-9F91-DAC2C5296343> /usr/lib/libSystem.B.dylib
0xa58bf000 - 0xa58d4ff7  libapple_nghttp2.dylib (1.24) <480C0C04-2533-3D44-8232-006B6CBA7758> /usr/lib/libapple_nghttp2.dylib
0xa58d5000 - 0xa5900fff  libarchive.2.dylib (54) <D55C5F86-251D-3C33-A617-0C623D4F512E> /usr/lib/libarchive.2.dylib
0xa5a54000 - 0xa5a54ff3  libauto.dylib (187) <CE2A78CC-670F-3E07-9539-822DCD2F6084> /usr/lib/libauto.dylib
0xa5a55000 - 0xa5a65fff  libbsm.0.dylib (39) <067E9003-0673-32A3-9B40-492323182C5C> /usr/lib/libbsm.0.dylib
0xa5a66000 - 0xa5a72ff7  libbz2.1.0.dylib (38) <77C24A36-BE84-3702-A786-935C597A0A86> /usr/lib/libbz2.1.0.dylib
0xa5a73000 - 0xa5accffb  libc++.1.dylib (400.9) <AD612EEF-6CE3-315D-82C2-58248BE13431> /usr/lib/libc++.1.dylib
0xa5acd000 - 0xa5aeefff  libc++abi.dylib (400.7) <41323E53-C7EA-3E9A-BD30-38E82399F843> /usr/lib/libc++abi.dylib
0xa5af0000 - 0xa5b01ff7  libcmph.dylib (6) <EC7664F1-B5A1-37F4-B7DC-F6AC10587E35> /usr/lib/libcmph.dylib
0xa5b02000 - 0xa5b15ff7  libcompression.dylib (47) <F80DDFC1-F96A-3BAD-967D-C1E24253273A> /usr/lib/libcompression.dylib
0xa5b16000 - 0xa5b2dffb  libcoretls.dylib (155) <F66FAEBC-4B6E-31E0-ACA8-C8ACBC7689DD> /usr/lib/libcoretls.dylib
0xa5b2e000 - 0xa5b2ffff  libcoretls_cfhelpers.dylib (155) <8B8ABC2C-F251-3C80-9747-88C05A2CBE64> /usr/lib/libcoretls_cfhelpers.dylib
0xa6017000 - 0xa606efff  libcups.2.dylib (462.1) <0180AE97-A19F-3D49-9838-06995E73F572> /usr/lib/libcups.2.dylib
0xa6184000 - 0xa6184fff  libenergytrace.dylib (16) <34FC43C7-D9B6-3C01-8B65-E49059D31279> /usr/lib/libenergytrace.dylib
0xa61b8000 - 0xa61bcfff  libheimdal-asn1.dylib (520.30.1) <DEA7E913-118F-333E-BE08-5B4F19B33B9A> /usr/lib/libheimdal-asn1.dylib
0xa61e8000 - 0xa62d8ff3  libiconv.2.dylib (51) <FE6D05A5-18DB-3FD8-A52F-B7BADB232C78> /usr/lib/libiconv.2.dylib
0xa62d9000 - 0xa64fbff7  libicucore.A.dylib (59152.0.1) <35D52BFF-C74C-3519-AEAC-7371E3C7E4BD> /usr/lib/libicucore.A.dylib
0xa6543000 - 0xa6544fff  liblangid.dylib (128) <120FE992-47E4-3A73-A039-1B401F5696DC> /usr/lib/liblangid.dylib
0xa6545000 - 0xa655dff7  liblzma.5.dylib (10) <8A5C9679-430A-3A19-AF68-9D21BAC442C7> /usr/lib/liblzma.5.dylib
0xa655e000 - 0xa6573fff  libmarisa.dylib (9) <805453EE-B829-3DA5-8DF3-5132D03D5B74> /usr/lib/libmarisa.dylib
0xa6628000 - 0xa6845fff  libmecabra.dylib (779.7.6) <3C7F6A43-B17C-3673-A0AC-14FFE08370D4> /usr/lib/libmecabra.dylib
0xa6a0c000 - 0xa6ae0fff  libnetwork.dylib (1229.30.11) <E4008EDE-F873-33FF-BD96-7DB14FA4F364> /usr/lib/libnetwork.dylib
0xa6ae1000 - 0xa6ec10fb  libobjc.A.dylib (723) <4AF346B8-C1A8-3199-B1BB-ADEDD64D5C1A> /usr/lib/libobjc.A.dylib
0xa6ec5000 - 0xa6ec8fff  libpam.2.dylib (22) <7106F43C-84DD-3F26-905A-B52780AFEB3E> /usr/lib/libpam.2.dylib
0xa6ecb000 - 0xa6efcfff  libpcap.A.dylib (79.20.1) <154889CF-5F83-3012-953E-0FC8FEE50FF8> /usr/lib/libpcap.A.dylib
0xa6f3a000 - 0xa6f55ffb  libresolv.9.dylib (65) <65A43F5B-CF88-3948-AE5C-D7CA02D814A1> /usr/lib/libresolv.9.dylib
0xa6fa0000 - 0xa712aff7  libsqlite3.dylib (274.5) <B09AF63F-4F1A-3481-9B61-6EBB64D12EB9> /usr/lib/libsqlite3.dylib
0xa72ce000 - 0xa7308ffb  libusrtcp.dylib (1229.30.11) <39D76669-A48B-3BAC-8F45-1D6CA87E9B4B> /usr/lib/libusrtcp.dylib
0xa7309000 - 0xa730cff7  libutil.dylib (51.20.1) <86BD9675-16A2-345D-9B8D-E8A3397F2365> /usr/lib/libutil.dylib
0xa730d000 - 0xa731bff7  libxar.1.dylib (400) <4B664A7E-EC05-34AD-ACC6-C879B69DBA7C> /usr/lib/libxar.1.dylib
0xa731c000 - 0xa73faff7  libxml2.2.dylib (31.7) <3E1F9E3D-6C44-3437-AB2B-E5ACE1927F81> /usr/lib/libxml2.2.dylib
0xa73fb000 - 0xa7423ff3  libxslt.1.dylib (15.10) <1A3DC7B8-7C92-3D73-BF82-D60E64BC3DF0> /usr/lib/libxslt.1.dylib
0xa7424000 - 0xa7433ff7  libz.1.dylib (70) <588F445F-0065-3D77-8002-BA9411DA1D70> /usr/lib/libz.1.dylib
0xa746d000 - 0xa7471fff  libcache.dylib (80) <5D011637-CADA-38A1-A695-CE049657FD9D> /usr/lib/system/libcache.dylib
0xa7472000 - 0xa747cfff  libcommonCrypto.dylib (60118.30.2) <38B2C15B-D27F-3106-A337-F72F29844825> /usr/lib/system/libcommonCrypto.dylib
0xa747d000 - 0xa7482fff  libcompiler_rt.dylib (62) <FA07FEE2-CEFE-3CC0-A82F-E601AA2CCB36> /usr/lib/system/libcompiler_rt.dylib
0xa7483000 - 0xa748cff3  libcopyfile.dylib (146.30.2) <F3A05833-AD1C-3E3A-8100-847297C882FC> /usr/lib/system/libcopyfile.dylib
0xa748d000 - 0xa74f5ff7  libcorecrypto.dylib (562.30.10) <0D8A61F8-2D7D-31F1-93AB-0597D80CCA85> /usr/lib/system/libcorecrypto.dylib
0xa7560000 - 0xa7595fff  libdispatch.dylib (913.30.4) <D1812254-DE85-3A5B-AD7B-5CE23BB8C9E1> /usr/lib/system/libdispatch.dylib
0xa7596000 - 0xa75b3fff  libdyld.dylib (519.2.2) <A79B6A65-DDAA-31C5-B66B-95FB343125BE> /usr/lib/system/libdyld.dylib
0xa75b4000 - 0xa75b4fff  libkeymgr.dylib (28) <C448ACFC-DD1B-3F08-B4C3-D2B69D1210B1> /usr/lib/system/libkeymgr.dylib
0xa75b5000 - 0xa75c1ff7  libkxld.dylib (4570.41.2) <C01D2E6F-B29E-3795-9258-55445BF8F933> /usr/lib/system/libkxld.dylib
0xa75c2000 - 0xa75c2fff  liblaunch.dylib (1205.30.29) <0F3BF17D-FCFA-3692-8A6E-FDE5C58DB3B7> /usr/lib/system/liblaunch.dylib
0xa75c3000 - 0xa75c8fff  libmacho.dylib (900.0.1) <F1F0BC1D-A2D9-39F9-9A11-263F8392CB3B> /usr/lib/system/libmacho.dylib
0xa75c9000 - 0xa75cbfff  libquarantine.dylib (86) <68DE2EB2-7911-304D-89D6-1517CA689001> /usr/lib/system/libquarantine.dylib
0xa75cc000 - 0xa75cdfff  libremovefile.dylib (45) <BEF76B44-53EA-3970-AB50-2296DC7F097F> /usr/lib/system/libremovefile.dylib
0xa75ce000 - 0xa75e5ff7  libsystem_asl.dylib (356.1.1) <F96973B5-C36B-3037-8AEC-3BF7147D79E2> /usr/lib/system/libsystem_asl.dylib
0xa75e6000 - 0xa75e6fff  libsystem_blocks.dylib (67) <32CE9BB7-E047-3568-981E-4EA94D3DCBB5> /usr/lib/system/libsystem_blocks.dylib
0xa75e7000 - 0xa7673fff  libsystem_c.dylib (1244.30.3) <8BCBF89D-5CE7-3950-884A-86E37DBF2660> /usr/lib/system/libsystem_c.dylib
0xa7674000 - 0xa7677fff  libsystem_configuration.dylib (963.30.1) <0F30DC5A-F39F-32C9-BA01-05AAC699713A> /usr/lib/system/libsystem_configuration.dylib
0xa7678000 - 0xa767bfff  libsystem_coreservices.dylib (51) <C3D75760-EED5-3C5C-8245-FBD3D9FD60FD> /usr/lib/system/libsystem_coreservices.dylib
0xa767c000 - 0xa767dfff  libsystem_darwin.dylib (1244.30.3) <83B1D06A-9FA5-3F0B-A223-0659F4248E51> /usr/lib/system/libsystem_darwin.dylib
0xa767e000 - 0xa7684ff3  libsystem_dnssd.dylib (878.30.4) <3C4400C4-C531-3653-872B-E22892D7B29A> /usr/lib/system/libsystem_dnssd.dylib
0xa7685000 - 0xa76d4ffb  libsystem_info.dylib (517.30.1) <A8E62937-32F9-373C-8150-B6B442227226> /usr/lib/system/libsystem_info.dylib
0xa76d5000 - 0xa76f8ff7  libsystem_kernel.dylib (4570.41.2) <649BB7E7-6378-3D2C-BBC6-ED2577E551B9> /usr/lib/system/libsystem_kernel.dylib
0xa76f9000 - 0xa7748fdb  libsystem_m.dylib (3146) <DBE0AACD-3665-3EEB-BADA-A435E591C54B> /usr/lib/system/libsystem_m.dylib
0xa7749000 - 0xa7763fff  libsystem_malloc.dylib (140.40.1) <968EF31E-50B0-3BFD-96B8-8FD513BDCB3C> /usr/lib/system/libsystem_malloc.dylib
0xa7764000 - 0xa7801ffb  libsystem_network.dylib (1229.30.11) <84B584A7-7583-31E7-8A39-64B4A5AD643B> /usr/lib/system/libsystem_network.dylib
0xa7802000 - 0xa780cfff  libsystem_networkextension.dylib (767.40.1) <EB81FB6B-A725-3F87-991A-DD55F0ED540A> /usr/lib/system/libsystem_networkextension.dylib
0xa780d000 - 0xa7815ff3  libsystem_notify.dylib (172) <63E3CF8C-4F15-3D45-84A6-1218352031E9> /usr/lib/system/libsystem_notify.dylib
0xa7816000 - 0xa781cffb  libsystem_platform.dylib (161.20.1) <82782E0E-7264-3CB4-AE69-571EDB5E7A24> /usr/lib/system/libsystem_platform.dylib
0xa781d000 - 0xa7827ff3  libsystem_pthread.dylib (301.30.1) <7409C1E5-F3BA-3AB3-ADC1-9DCD356C6C13> /usr/lib/system/libsystem_pthread.dylib
0xa7828000 - 0xa782bff3  libsystem_sandbox.dylib (765.40.2) <07D6B9E4-5A9D-300F-8D65-E218EDE85477> /usr/lib/system/libsystem_sandbox.dylib
0xa782c000 - 0xa782efff  libsystem_secinit.dylib (30) <CE2C90DE-27A4-3546-8A05-96B743861DD0> /usr/lib/system/libsystem_secinit.dylib
0xa782f000 - 0xa7837ff7  libsystem_symptoms.dylib (820.30.7) <0283BDB3-16A2-371E-A25C-A26F076C24A5> /usr/lib/system/libsystem_symptoms.dylib
0xa7838000 - 0xa784afff  libsystem_trace.dylib (829.30.14) <79446DE0-89F6-3979-B14C-7B463AD70351> /usr/lib/system/libsystem_trace.dylib
0xa784c000 - 0xa7852fff  libunwind.dylib (35.3) <642BBA03-0411-3FAA-A421-D79A9156AB1C> /usr/lib/system/libunwind.dylib
0xa7853000 - 0xa787bff7  libxpc.dylib (1205.30.29) <CD44097B-4B65-3F75-AB7F-52228229FFB5> /usr/lib/system/libxpc.dylib

External Modification Summary:
  Calls made by other processes targeting this process:
    task_for_pid: 0
    thread_create: 0
    thread_set_state: 0
  Calls made by this process:
    task_for_pid: 0
    thread_create: 0
    thread_set_state: 0
  Calls made by all processes on this machine:
    task_for_pid: 4837
    thread_create: 0
    thread_set_state: 0

VM Region Summary:
ReadOnly portion of Libraries: Total=190.2M resident=0K(0%) swapped_out_or_unallocated=190.2M(100%)
Writable regions: Total=8444K written=0K(0%) resident=0K(0%) swapped_out=0K(0%) unallocated=8444K(100%)
 
                                VIRTUAL   REGION 
REGION TYPE                        SIZE    COUNT (non-coalesced) 
===========                     =======  ======= 
Stack                             8192K        2 
Stack Guard                       56.0M        2 
__DATA                            8748K      177 
__FONT_DATA                          4K        2 
__LINKEDIT                        74.2M        4 
__OBJC                            2680K       54 
__TEXT                           115.9M      181 
__UNICODE                          560K        2 
mapped file                      293.5M      145 
shared memory                        8K        3 
===========                     =======  ======= 
TOTAL                            559.4M      562 

Model: MacBookPro6,2, BootROM MBP61.005A.B00, 2 processors, Intel Core i7, 2.66 GHz, 8 GB, SMC 1.58f17
Graphics: Intel HD Graphics, Intel HD Graphics, Built-In
Graphics: NVIDIA GeForce GT 330M, NVIDIA GeForce GT 330M, PCIe, 512 MB
Memory Module: BANK 0/DIMM0, 4 GB, DDR3, 1067 MHz, 0x029E, 0x434D5341344758334D314131303636433720
Memory Module: BANK 1/DIMM0, 4 GB, DDR3, 1067 MHz, 0x029E, 0x434D5341344758334D314131303636433720
AirPort: spairport_wireless_card_type_airport_extreme (0x14E4, 0x93), Broadcom BCM43xx 1.0 (5.106.98.102.30)
Bluetooth: Version 6.0.2f2, 3 services, 27 devices, 1 incoming serial ports
Network Service: Wi-Fi, AirPort, en1
Serial ATA Device: Hitachi HTS545050B9SA02, 500.11 GB
Serial ATA Device: MATSHITADVD-R   UJ-898
USB Device: USB 2.0 Bus
USB Device: Hub
USB Device: IR Receiver
USB Device: Built-in iSight
USB Device: USB 2.0 Bus
USB Device: Hub
USB Device: USB Receiver
USB Device: Internal Memory Card Reader
USB Device: Apple Internal Keyboard / Trackpad
USB Device: BRCM2070 Hub
USB Device: Bluetooth USB Host Controller
Thunderbolt Bus: 
