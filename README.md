# DETOX/EXPO issue (tested only on iOS)

Hello i create this repository to share my issue when i create a fresh clean app from expo getting started, detach this app and install detox.

### ERROR

My app work fine, but an error appear and say element/device is not defined
i found many issue :
- https://github.com/wix/detox/issues/795
- https://github.com/wix/detox/issues/893
- https://github.com/wix/detox/issues/670


### MY CONFIGURATION

| Program       | Version  |
| ------------- | -------- |
| Node          | v8.11.3  |
| React         | v16.3.1  |
| React Native  | v0.53.0  |
| Expo          | v29.0.0  |
| ExpoKit       | v2.7.0   |
| Detox         | v8.2.3   |
| Xcode         | v9.4.1   |

### SETUP

You should follow the simple Detox getting started ( only Step 1 ) to setup detox in global and work in simulator
https://github.com/wix/detox/blob/master/docs/Introduction.GettingStarted.md

```sh
  git clone https://github.com/GuillaumeSarfati/detox-expo-issue.git
  cd detox-expo-issue
  npm install
```

### EXPERIMENT MY ISSUE

```sh
  npm run test:e2e
```

### OUTPUT

```sh
detox build && detox test
xcodebuild -workspace ios/detox-expo-issue.xcworkspace -scheme detox-expo-issue -configuration Debug -sdk iphonesimulator -derivedDataPath ios/build
User defaults from command line:
    IDEDerivedDataPathOverride = /Volumes/Guillaume/Projects/detox-expo-issue/ios/build

Build settings from command line:
    SDKROOT = iphonesimulator11.4

=== BUILD TARGET Bolts OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET AppAuth OF PROJECT Pods WITH CONFIGURATION Debug ===
Check dependencies

=== BUILD TARGET EXCore OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET Branch OF PROJECT Pods WITH CONFIGURATION Debug ===
Check dependencies

=== BUILD TARGET Analytics OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET DoubleConversion OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET CocoaLumberjack OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET Amplitude-iOS OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET EXCamera OF PROJECT Pods WITH CONFIGURATION Debug ===
Check dependencies

=== BUILD TARGET EXConstants OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET EXFileSystem OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET EXGL-CPP OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET EXPermissions OF PROJECT Pods WITH CONFIGURATION Debug ===
Check dependencies

=== BUILD TARGET glog OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET yoga OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET EXSMS OF PROJECT Pods WITH CONFIGURATION Debug ===
Check dependencies

=== BUILD TARGET EXSensors OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET FBSDKCoreKit OF PROJECT Pods WITH CONFIGURATION Debug ===
Check dependencies

=== BUILD TARGET EXGL OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET GPUImage OF PROJECT Pods WITH CONFIGURATION Debug ===
Check dependencies

=== BUILD TARGET Google-Maps-iOS-Utils OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET JKBigInteger2 OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET lottie-ios OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET Folly OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET React OF PROJECT Pods WITH CONFIGURATION Debug ===
Check dependencies

=== BUILD TARGET FBSDKLoginKit OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET FBSDKShareKit OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET EXReactNativeAdapter OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET ExpoKit OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies
warning: no rule to process file '/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/ExpoKit/template-files/keys.json' of type text.json for architecture x86_64

=== BUILD TARGET Pods-detox-expo-issue OF PROJECT Pods WITH CONFIGURATION Debug ===

Check dependencies

=== BUILD TARGET detox-expo-issue OF PROJECT detox-expo-issue WITH CONFIGURATION Debug ===

Check dependencies

PhaseScriptExecution Prepare\ Expo build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/Script-B5722AD01DFB7E3F0084848F.sh
    cd /Volumes/Guillaume/Projects/detox-expo-issue/ios
    export ACTION=build
    export AD_HOC_CODE_SIGNING_ALLOWED=YES
    export ALTERNATE_GROUP=staff
    export ALTERNATE_MODE=u+w,go-w,a+rX
    export ALTERNATE_OWNER=guillaumesarfati
    export ALWAYS_EMBED_SWIFT_STANDARD_LIBRARIES=NO
    export ALWAYS_SEARCH_USER_PATHS=NO
    export ALWAYS_USE_SEPARATE_HEADERMAPS=NO
    export APPLE_INTERNAL_DEVELOPER_DIR=/AppleInternal/Developer
    export APPLE_INTERNAL_DIR=/AppleInternal
    export APPLE_INTERNAL_DOCUMENTATION_DIR=/AppleInternal/Documentation
    export APPLE_INTERNAL_LIBRARY_DIR=/AppleInternal/Library
    export APPLE_INTERNAL_TOOLS=/AppleInternal/Developer/Tools
    export APPLICATION_EXTENSION_API_ONLY=NO
    export APPLY_RULES_IN_COPY_FILES=NO
    export ARCHS=x86_64
    export ARCHS_STANDARD="i386 x86_64"
    export ARCHS_STANDARD_32_64_BIT="i386 x86_64"
    export ARCHS_STANDARD_32_BIT=i386
    export ARCHS_STANDARD_64_BIT=x86_64
    export ARCHS_STANDARD_INCLUDING_64_BIT="i386 x86_64"
    export ARCHS_UNIVERSAL_IPHONE_OS="i386 x86_64"
    export ASSETCATALOG_COMPILER_APPICON_NAME=AppIcon
    export AVAILABLE_PLATFORMS="appletvos appletvsimulator iphoneos iphonesimulator macosx watchos watchsimulator"
    export BITCODE_GENERATION_MODE=marker
    export BUILD_ACTIVE_RESOURCES_ONLY=YES
    export BUILD_COMPONENTS="headers build"
    export BUILD_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products
    export BUILD_ROOT=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products
    export BUILD_STYLE=
    export BUILD_VARIANTS=normal
    export BUILT_PRODUCTS_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator
    export CACHE_ROOT=/var/folders/w4/5vpc45vd3z1f_cqbncywlvgw0000gn/C/com.apple.DeveloperTools/9.4.1-9F2000/Xcode
    export CCHROOT=/var/folders/w4/5vpc45vd3z1f_cqbncywlvgw0000gn/C/com.apple.DeveloperTools/9.4.1-9F2000/Xcode
    export CHMOD=/bin/chmod
    export CHOWN=/usr/sbin/chown
    export CLANG_ANALYZER_NONNULL=YES
    export CLANG_CXX_LANGUAGE_STANDARD=gnu++0x
    export CLANG_CXX_LIBRARY=libc++
    export CLANG_ENABLE_MODULES=YES
    export CLANG_ENABLE_OBJC_ARC=YES
    export CLANG_MODULES_AUTOLINK=YES
    export CLANG_MODULES_BUILD_SESSION_FILE=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/ModuleCache.noindex/Session.modulevalidation
    export CLANG_WARN_BLOCK_CAPTURE_AUTORELEASING=YES
    export CLANG_WARN_BOOL_CONVERSION=YES
    export CLANG_WARN_COMMA=YES
    export CLANG_WARN_CONSTANT_CONVERSION=YES
    export CLANG_WARN_DIRECT_OBJC_ISA_USAGE=YES_ERROR
    export CLANG_WARN_DOCUMENTATION_COMMENTS=YES
    export CLANG_WARN_EMPTY_BODY=YES
    export CLANG_WARN_ENUM_CONVERSION=YES
    export CLANG_WARN_INFINITE_RECURSION=YES
    export CLANG_WARN_INT_CONVERSION=YES
    export CLANG_WARN_NON_LITERAL_NULL_CONVERSION=YES
    export CLANG_WARN_OBJC_LITERAL_CONVERSION=YES
    export CLANG_WARN_OBJC_ROOT_CLASS=YES_ERROR
    export CLANG_WARN_RANGE_LOOP_ANALYSIS=YES
    export CLANG_WARN_STRICT_PROTOTYPES=YES
    export CLANG_WARN_SUSPICIOUS_MOVE=YES
    export CLANG_WARN_SUSPICIOUS_MOVES=YES
    export CLANG_WARN_UNREACHABLE_CODE=YES
    export CLANG_WARN__DUPLICATE_METHOD_MATCH=YES
    export CLASS_FILE_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/JavaClasses
    export CLEAN_PRECOMPS=YES
    export CLONE_HEADERS=NO
    export CODESIGNING_FOLDER_PATH=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/detox-expo-issue.app
    export CODE_SIGNING_ALLOWED=YES
    export CODE_SIGNING_REQUIRED=YES
    export CODE_SIGN_CONTEXT_CLASS=XCiPhoneSimulatorCodeSignContext
    export CODE_SIGN_IDENTITY=-
    export CODE_SIGN_INJECT_BASE_ENTITLEMENTS=YES
    export COLOR_DIAGNOSTICS=YES
    export COMBINE_HIDPI_IMAGES=NO
    export COMMAND_MODE=legacy
    export COMPILER_INDEX_STORE_ENABLE=Default
    export COMPOSITE_SDK_DIRS=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/CompositeSDKs
    export COMPRESS_PNG_FILES=YES
    export CONFIGURATION=Debug
    export CONFIGURATION_BUILD_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator
    export CONFIGURATION_TEMP_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator
    export CONTENTS_FOLDER_PATH=detox-expo-issue.app
    export COPYING_PRESERVES_HFS_DATA=NO
    export COPY_HEADERS_RUN_UNIFDEF=NO
    export COPY_PHASE_STRIP=NO
    export COPY_RESOURCES_FROM_STATIC_FRAMEWORKS=YES
    export CORRESPONDING_DEVICE_PLATFORM_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform
    export CORRESPONDING_DEVICE_PLATFORM_NAME=iphoneos
    export CORRESPONDING_DEVICE_SDK_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/SDKs/iPhoneOS11.4.sdk
    export CORRESPONDING_DEVICE_SDK_NAME=iphoneos11.4
    export CP=/bin/cp
    export CREATE_INFOPLIST_SECTION_IN_BINARY=NO
    export CURRENT_ARCH=x86_64
    export CURRENT_VARIANT=normal
    export DEAD_CODE_STRIPPING=YES
    export DEBUGGING_SYMBOLS=YES
    export DEBUG_INFORMATION_FORMAT=dwarf
    export DEFAULT_COMPILER=com.apple.compilers.llvm.clang.1_0
    export DEFAULT_KEXT_INSTALL_PATH=/System/Library/Extensions
    export DEFINES_MODULE=NO
    export DEPLOYMENT_LOCATION=NO
    export DEPLOYMENT_POSTPROCESSING=NO
    export DEPLOYMENT_TARGET_CLANG_ENV_NAME=IPHONEOS_DEPLOYMENT_TARGET
    export DEPLOYMENT_TARGET_CLANG_FLAG_NAME=mios-simulator-version-min
    export DEPLOYMENT_TARGET_CLANG_FLAG_PREFIX=-mios-simulator-version-min=
    export DEPLOYMENT_TARGET_SETTING_NAME=IPHONEOS_DEPLOYMENT_TARGET
    export DEPLOYMENT_TARGET_SUGGESTED_VALUES="8.0 8.1 8.2 8.3 8.4 9.0 9.1 9.2 9.3 10.0 10.1 10.2 10.3 11.0 11.1 11.2 11.3 11.4"
    export DERIVED_FILES_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/DerivedSources
    export DERIVED_FILE_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/DerivedSources
    export DERIVED_SOURCES_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/DerivedSources
    export DEVELOPER_APPLICATIONS_DIR=/Applications/Xcode.app/Contents/Developer/Applications
    export DEVELOPER_BIN_DIR=/Applications/Xcode.app/Contents/Developer/usr/bin
    export DEVELOPER_DIR=/Applications/Xcode.app/Contents/Developer
    export DEVELOPER_FRAMEWORKS_DIR=/Applications/Xcode.app/Contents/Developer/Library/Frameworks
    export DEVELOPER_FRAMEWORKS_DIR_QUOTED=/Applications/Xcode.app/Contents/Developer/Library/Frameworks
    export DEVELOPER_LIBRARY_DIR=/Applications/Xcode.app/Contents/Developer/Library
    export DEVELOPER_SDK_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs
    export DEVELOPER_TOOLS_DIR=/Applications/Xcode.app/Contents/Developer/Tools
    export DEVELOPER_USR_DIR=/Applications/Xcode.app/Contents/Developer/usr
    export DEVELOPMENT_LANGUAGE=English
    export DEVELOPMENT_TEAM=C8D8QTF339
    export DOCUMENTATION_FOLDER_PATH=detox-expo-issue.app/English.lproj/Documentation
    export DO_HEADER_SCANNING_IN_JAM=NO
    export DSTROOT=/tmp/detox-expo-issue.dst
    export DT_TOOLCHAIN_DIR=/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain
    export DWARF_DSYM_FILE_NAME=detox-expo-issue.app.dSYM
    export DWARF_DSYM_FILE_SHOULD_ACCOMPANY_PRODUCT=NO
    export DWARF_DSYM_FOLDER_PATH=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator
    export EFFECTIVE_PLATFORM_NAME=-iphonesimulator
    export EMBEDDED_CONTENT_CONTAINS_SWIFT=NO
    export EMBED_ASSET_PACKS_IN_PRODUCT_BUNDLE=NO
    export ENABLE_BITCODE=NO
    export ENABLE_DEFAULT_HEADER_SEARCH_PATHS=YES
    export ENABLE_HEADER_DEPENDENCIES=YES
    export ENABLE_ON_DEMAND_RESOURCES=YES
    export ENABLE_STRICT_OBJC_MSGSEND=YES
    export ENABLE_TESTABILITY=YES
    export ENTITLEMENTS_REQUIRED=YES
    export EXCLUDED_INSTALLSRC_SUBDIRECTORY_PATTERNS=".DS_Store .svn .git .hg CVS"
    export EXCLUDED_RECURSIVE_SEARCH_PATH_SUBDIRECTORIES="*.nib *.lproj *.framework *.gch *.xcode* *.xcassets (*) .DS_Store CVS .svn .git .hg *.pbproj *.pbxproj"
    export EXECUTABLES_FOLDER_PATH=detox-expo-issue.app/Executables
    export EXECUTABLE_FOLDER_PATH=detox-expo-issue.app
    export EXECUTABLE_NAME=detox-expo-issue
    export EXECUTABLE_PATH=detox-expo-issue.app/detox-expo-issue
    export EXPANDED_CODE_SIGN_IDENTITY=-
    export EXPANDED_CODE_SIGN_IDENTITY_NAME=-
    export EXPANDED_PROVISIONING_PROFILE=
    export FILE_LIST=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/Objects/LinkFileList
    export FIXED_FILES_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/FixedFiles
    export FRAMEWORKS_FOLDER_PATH=detox-expo-issue.app/Frameworks
    export FRAMEWORK_FLAG_PREFIX=-framework
    export FRAMEWORK_SEARCH_PATHS="/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator  \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Crashlytics/iOS\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/FBAudienceNetwork\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Fabric/iOS\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Google-Mobile-Ads-SDK/Frameworks/frameworks\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/GoogleAppUtilities/Frameworks/frameworks\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/GoogleAuthUtilities/Frameworks/frameworks\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/GoogleMaps/Base/Frameworks\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/GoogleMaps/Maps/Frameworks\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/GoogleNetworkingUtilities/Frameworks/frameworks\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/GoogleSymbolUtilities/Frameworks/frameworks\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/GoogleUtilities/Frameworks/frameworks\""
    export FRAMEWORK_VERSION=A
    export FULL_PRODUCT_NAME=detox-expo-issue.app
    export GCC3_VERSION=3.3
    export GCC_C_LANGUAGE_STANDARD=gnu99
    export GCC_DYNAMIC_NO_PIC=NO
    export GCC_INLINES_ARE_PRIVATE_EXTERN=YES
    export GCC_NO_COMMON_BLOCKS=YES
    export GCC_OBJC_LEGACY_DISPATCH=YES
    export GCC_OPTIMIZATION_LEVEL=0
    export GCC_PFE_FILE_C_DIALECTS="c objective-c c++ objective-c++"
    export GCC_PREPROCESSOR_DEFINITIONS="DEBUG=1  COCOAPODS=1"
    export GCC_SYMBOLS_PRIVATE_EXTERN=NO
    export GCC_TREAT_WARNINGS_AS_ERRORS=NO
    export GCC_VERSION=com.apple.compilers.llvm.clang.1_0
    export GCC_VERSION_IDENTIFIER=com_apple_compilers_llvm_clang_1_0
    export GCC_WARN_64_TO_32_BIT_CONVERSION=YES
    export GCC_WARN_ABOUT_RETURN_TYPE=YES_ERROR
    export GCC_WARN_UNDECLARED_SELECTOR=YES
    export GCC_WARN_UNINITIALIZED_AUTOS=YES_AGGRESSIVE
    export GCC_WARN_UNUSED_FUNCTION=YES
    export GCC_WARN_UNUSED_VARIABLE=YES
    export GENERATE_MASTER_OBJECT_FILE=NO
    export GENERATE_PKGINFO_FILE=YES
    export GENERATE_PROFILING_CODE=NO
    export GENERATE_TEXT_BASED_STUBS=NO
    export GID=20
    export GROUP=staff
    export HEADERMAP_INCLUDES_FLAT_ENTRIES_FOR_TARGET_BEING_BUILT=YES
    export HEADERMAP_INCLUDES_FRAMEWORK_ENTRIES_FOR_ALL_PRODUCT_TYPES=YES
    export HEADERMAP_INCLUDES_NONPUBLIC_NONPRIVATE_HEADERS=YES
    export HEADERMAP_INCLUDES_PROJECT_HEADERS=YES
    export HEADERMAP_USES_FRAMEWORK_PREFIX_ENTRIES=YES
    export HEADERMAP_USES_VFS=NO
    export HEADER_SEARCH_PATHS="/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/include  \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Amplitude-iOS\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Analytics\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/AppAuth\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Bolts\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Branch\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/CocoaLumberjack\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Crashlytics\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/DoubleConversion\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCamera\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCameraInterface\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXConstants\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXConstantsInterface\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCore\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFaceDetectorInterface\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFileSystem\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFileSystemInterface\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXGL\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXGL-CPP\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXPermissions\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXPermissionsInterface\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXReactNativeAdapter\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSMS\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSensors\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSensorsInterface\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/ExpoKit\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBAudienceNetwork\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKCoreKit\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKLoginKit\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKShareKit\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Fabric\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Folly\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GPUImage\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Google-Maps-iOS-Utils\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Google-Mobile-Ads-SDK\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleAppUtilities\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleAuthUtilities\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleMaps\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleNetworkingUtilities\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleSignIn\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleSymbolUtilities\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleUtilities\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/JKBigInteger2\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/React\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/boost-for-react-native\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/glog\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/lottie-ios\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/yoga\""
    export HIDE_BITCODE_SYMBOLS=YES
    export HOME=/Users/guillaumesarfati
    export ICONV=/usr/bin/iconv
    export INFOPLIST_EXPAND_BUILD_SETTINGS=YES
    export INFOPLIST_FILE=/Volumes/Guillaume/Projects/detox-expo-issue/ios/detox-expo-issue/Supporting/Info.plist
    export INFOPLIST_OUTPUT_FORMAT=binary
    export INFOPLIST_PATH=detox-expo-issue.app/Info.plist
    export INFOPLIST_PREPROCESS=NO
    export INFOSTRINGS_PATH=detox-expo-issue.app/English.lproj/InfoPlist.strings
    export INLINE_PRIVATE_FRAMEWORKS=NO
    export INSTALLHDRS_COPY_PHASE=NO
    export INSTALLHDRS_SCRIPT_PHASE=NO
    export INSTALL_DIR=/tmp/detox-expo-issue.dst/Applications
    export INSTALL_GROUP=staff
    export INSTALL_MODE_FLAG=u+w,go-w,a+rX
    export INSTALL_OWNER=guillaumesarfati
    export INSTALL_PATH=/Applications
    export INSTALL_ROOT=/tmp/detox-expo-issue.dst
    export IPHONEOS_DEPLOYMENT_TARGET=9.0
    export JAVAC_DEFAULT_FLAGS="-J-Xms64m -J-XX:NewSize=4M -J-Dfile.encoding=UTF8"
    export JAVA_APP_STUB=/System/Library/Frameworks/JavaVM.framework/Resources/MacOS/JavaApplicationStub
    export JAVA_ARCHIVE_CLASSES=YES
    export JAVA_ARCHIVE_TYPE=JAR
    export JAVA_COMPILER=/usr/bin/javac
    export JAVA_FOLDER_PATH=detox-expo-issue.app/Java
    export JAVA_FRAMEWORK_RESOURCES_DIRS=Resources
    export JAVA_JAR_FLAGS=cv
    export JAVA_SOURCE_SUBDIR=.
    export JAVA_USE_DEPENDENCIES=YES
    export JAVA_ZIP_FLAGS=-urg
    export JIKES_DEFAULT_FLAGS="+E +OLDCSO"
    export KEEP_PRIVATE_EXTERNS=NO
    export LD_DEPENDENCY_INFO_FILE=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/Objects-normal/x86_64/detox-expo-issue_dependency_info.dat
    export LD_GENERATE_MAP_FILE=NO
    export LD_MAP_FILE_PATH=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/detox-expo-issue-LinkMap-normal-x86_64.txt
    export LD_NO_PIE=NO
    export LD_QUOTE_LINKER_ARGUMENTS_FOR_COMPILER_DRIVER=YES
    export LD_RUNPATH_SEARCH_PATHS=" @executable_path/Frameworks"
    export LEGACY_DEVELOPER_DIR=/Applications/Xcode.app/Contents/PlugIns/Xcode3Core.ideplugin/Contents/SharedSupport/Developer
    export LEX=lex
    export LIBRARY_FLAG_NOSPACE=YES
    export LIBRARY_FLAG_PREFIX=-l
    export LIBRARY_KEXT_INSTALL_PATH=/Library/Extensions
    export LIBRARY_SEARCH_PATHS="/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator  \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/Amplitude-iOS\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/Analytics\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/AppAuth\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/Bolts\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/Branch\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/CocoaLumberjack\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/DoubleConversion\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXCamera\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXConstants\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXCore\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXFileSystem\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXGL\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXGL-CPP\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXPermissions\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXReactNativeAdapter\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXSMS\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXSensors\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/ExpoKit\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/FBSDKCoreKit\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/FBSDKLoginKit\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/FBSDKShareKit\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/Folly\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/GPUImage\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/Google-Maps-iOS-Utils\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/JKBigInteger2\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/React\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/glog\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/lottie-ios\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/yoga\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/GoogleSignIn/Libraries\""
    export LINKER_DISPLAYS_MANGLED_NAMES=NO
    export LINK_FILE_LIST_normal_x86_64=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/Objects-normal/x86_64/detox-expo-issue.LinkFileList
    export LINK_WITH_STANDARD_LIBRARIES=YES
    export LOCALIZABLE_CONTENT_DIR=
    export LOCALIZED_RESOURCES_FOLDER_PATH=detox-expo-issue.app/English.lproj
    export LOCALIZED_STRING_MACRO_NAMES="NSLocalizedString CFLocalizedString"
    export LOCAL_ADMIN_APPS_DIR=/Applications/Utilities
    export LOCAL_APPS_DIR=/Applications
    export LOCAL_DEVELOPER_DIR=/Library/Developer
    export LOCAL_LIBRARY_DIR=/Library
    export LOCROOT=
    export LOCSYMROOT=
    export MACH_O_TYPE=mh_execute
    export MAC_OS_X_PRODUCT_BUILD_VERSION=17G65
    export MAC_OS_X_VERSION_ACTUAL=101306
    export MAC_OS_X_VERSION_MAJOR=101300
    export MAC_OS_X_VERSION_MINOR=1306
    export METAL_LIBRARY_FILE_BASE=default
    export METAL_LIBRARY_OUTPUT_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/detox-expo-issue.app
    export MODULE_CACHE_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/ModuleCache.noindex
    export MTL_ENABLE_DEBUG_INFO=YES
    export NATIVE_ARCH=i386
    export NATIVE_ARCH_32_BIT=i386
    export NATIVE_ARCH_64_BIT=x86_64
    export NATIVE_ARCH_ACTUAL=x86_64
    export NO_COMMON=YES
    export OBJC_ABI_VERSION=2
    export OBJECT_FILE_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/Objects
    export OBJECT_FILE_DIR_normal=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/Objects-normal
    export OBJROOT=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex
    export ONLY_ACTIVE_ARCH=YES
    export OS=MACOS
    export OSAC=/usr/bin/osacompile
    export OTHER_CFLAGS=" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Amplitude-iOS\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Analytics\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/AppAuth\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Bolts\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Branch\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/CocoaLumberjack\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Crashlytics\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/DoubleConversion\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCamera\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCameraInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXConstants\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXConstantsInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCore\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFaceDetectorInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFileSystem\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFileSystemInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXGL\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXGL-CPP\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXPermissions\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXPermissionsInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXReactNativeAdapter\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSMS\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSensors\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSensorsInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/ExpoKit\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBAudienceNetwork\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKCoreKit\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKLoginKit\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKShareKit\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Fabric\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Folly\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GPUImage\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Google-Maps-iOS-Utils\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Google-Mobile-Ads-SDK\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleAppUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleAuthUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleMaps\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleNetworkingUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleSignIn\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleSymbolUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/JKBigInteger2\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/React\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/boost-for-react-native\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/glog\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/lottie-ios\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/yoga\""
    export OTHER_CPLUSPLUSFLAGS=" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Amplitude-iOS\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Analytics\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/AppAuth\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Bolts\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Branch\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/CocoaLumberjack\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Crashlytics\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/DoubleConversion\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCamera\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCameraInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXConstants\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXConstantsInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCore\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFaceDetectorInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFileSystem\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFileSystemInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXGL\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXGL-CPP\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXPermissions\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXPermissionsInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXReactNativeAdapter\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSMS\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSensors\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSensorsInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/ExpoKit\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBAudienceNetwork\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKCoreKit\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKLoginKit\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKShareKit\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Fabric\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Folly\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GPUImage\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Google-Maps-iOS-Utils\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Google-Mobile-Ads-SDK\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleAppUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleAuthUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleMaps\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleNetworkingUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleSignIn\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleSymbolUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/JKBigInteger2\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/React\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/boost-for-react-native\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/glog\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/lottie-ios\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/yoga\""
    export OTHER_LDFLAGS=" -ObjC -l\"Amplitude-iOS\" -l\"Analytics\" -l\"AppAuth\" -l\"Bolts\" -l\"Branch\" -l\"CocoaLumberjack\" -l\"DoubleConversion\" -l\"EXCamera\" -l\"EXConstants\" -l\"EXCore\" -l\"EXFileSystem\" -l\"EXGL\" -l\"EXGL-CPP\" -l\"EXPermissions\" -l\"EXReactNativeAdapter\" -l\"EXSMS\" -l\"EXSensors\" -l\"ExpoKit\" -l\"FBSDKCoreKit\" -l\"FBSDKLoginKit\" -l\"FBSDKShareKit\" -l\"Folly\" -l\"GIPNSURL+FIFE_external\" -l\"GPUImage\" -l\"Google-Maps-iOS-Utils\" -l\"JKBigInteger2\" -l\"React\" -l\"SignIn_external\" -l\"c++\" -l\"glog\" -l\"lottie-ios\" -l\"sqlite3.0\" -l\"stdc++\" -l\"xml2\" -l\"yoga\" -l\"z\" -framework \"AVFoundation\" -framework \"Accelerate\" -framework \"AdSupport\" -framework \"AddressBook\" -framework \"AudioToolbox\" -framework \"CoreData\" -framework \"CoreGraphics\" -framework \"CoreImage\" -framework \"CoreLocation\" -framework \"CoreMedia\" -framework \"CoreMotion\" -framework \"CoreTelephony\" -framework \"CoreText\" -framework \"CoreVideo\" -framework \"Crashlytics\" -framework \"FBAudienceNetwork\" -framework \"Fabric\" -framework \"Foundation\" -framework \"GLKit\" -framework \"GoogleAppUtilities\" -framework \"GoogleAuthUtilities\" -framework \"GoogleMaps\" -framework \"GoogleMapsBase\" -framework \"GoogleMapsCore\" -framework \"GoogleMobileAds\" -framework \"GoogleNetworkingUtilities\" -framework \"GoogleSymbolUtilities\" -framework \"GoogleUtilities\" -framework \"ImageIO\" -framework \"JavaScriptCore\" -framework \"MediaPlayer\" -framework \"MessageUI\" -framework \"MobileCoreServices\" -framework \"OpenGLES\" -framework \"QuartzCore\" -framework \"SafariServices\" -framework \"Security\" -framework \"StoreKit\" -framework \"SystemConfiguration\" -framework \"UIKit\" -weak_framework \"Accounts\" -weak_framework \"AdSupport\" -weak_framework \"AudioToolbox\" -weak_framework \"CoreGraphics\" -weak_framework \"CoreLocation\" -weak_framework \"CoreMotion\" -weak_framework \"Foundation\" -weak_framework \"JavaScriptCore\" -weak_framework \"QuartzCore\" -weak_framework \"SafariServices\" -weak_framework \"Security\" -weak_framework \"Social\" -weak_framework \"UIKit\" -weak_framework \"WebKit\""
    export PACKAGE_TYPE=com.apple.package-type.wrapper.application
    export PASCAL_STRINGS=YES
    export PATH="/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin:/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/local/bin:/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/libexec:/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/usr/bin:/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/usr/local/bin:/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/usr/bin:/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/usr/local/bin:/Applications/Xcode.app/Contents/Developer/usr/bin:/Applications/Xcode.app/Contents/Developer/usr/local/bin:/Applications/Xcode.app/Contents/Developer/Tools:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin"
    export PATH_PREFIXES_EXCLUDED_FROM_HEADER_DEPENDENCIES="/usr/include /usr/local/include /System/Library/Frameworks /System/Library/PrivateFrameworks /Applications/Xcode.app/Contents/Developer/Headers /Applications/Xcode.app/Contents/Developer/SDKs /Applications/Xcode.app/Contents/Developer/Platforms"
    export PBDEVELOPMENTPLIST_PATH=detox-expo-issue.app/pbdevelopment.plist
    export PFE_FILE_C_DIALECTS=objective-c
    export PKGINFO_FILE_PATH=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/PkgInfo
    export PKGINFO_PATH=detox-expo-issue.app/PkgInfo
    export PLATFORM_DEVELOPER_APPLICATIONS_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/Applications
    export PLATFORM_DEVELOPER_BIN_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/usr/bin
    export PLATFORM_DEVELOPER_LIBRARY_DIR=/Applications/Xcode.app/Contents/PlugIns/Xcode3Core.ideplugin/Contents/SharedSupport/Developer/Library
    export PLATFORM_DEVELOPER_SDK_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/SDKs
    export PLATFORM_DEVELOPER_TOOLS_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/Tools
    export PLATFORM_DEVELOPER_USR_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/usr
    export PLATFORM_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform
    export PLATFORM_DISPLAY_NAME="iOS Simulator"
    export PLATFORM_NAME=iphonesimulator
    export PLATFORM_PREFERRED_ARCH=x86_64
    export PLIST_FILE_OUTPUT_FORMAT=binary
    export PLUGINS_FOLDER_PATH=detox-expo-issue.app/PlugIns
    export PODS_BUILD_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products
    export PODS_CONFIGURATION_BUILD_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator
    export PODS_PODFILE_DIR_PATH=/Volumes/Guillaume/Projects/detox-expo-issue/ios/.
    export PODS_ROOT=/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods
    export PRECOMPS_INCLUDE_HEADERS_FROM_BUILT_PRODUCTS_DIR=YES
    export PRECOMP_DESTINATION_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/PrefixHeaders
    export PRESERVE_DEAD_CODE_INITS_AND_TERMS=NO
    export PRIVATE_HEADERS_FOLDER_PATH=detox-expo-issue.app/PrivateHeaders
    export PRODUCT_BUNDLE_IDENTIFIER=com.detox.issue
    export PRODUCT_MODULE_NAME=detox_expo_issue
    export PRODUCT_NAME=detox-expo-issue
    export PRODUCT_SETTINGS_PATH=/Volumes/Guillaume/Projects/detox-expo-issue/ios/detox-expo-issue/Supporting/Info.plist
    export PRODUCT_TYPE=com.apple.product-type.application
    export PROFILING_CODE=NO
    export PROJECT=detox-expo-issue
    export PROJECT_DERIVED_FILE_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/DerivedSources
    export PROJECT_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios
    export PROJECT_FILE_PATH=/Volumes/Guillaume/Projects/detox-expo-issue/ios/detox-expo-issue.xcodeproj
    export PROJECT_NAME=detox-expo-issue
    export PROJECT_TEMP_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build
    export PROJECT_TEMP_ROOT=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex
    export PUBLIC_HEADERS_FOLDER_PATH=detox-expo-issue.app/Headers
    export RECURSIVE_SEARCH_PATHS_FOLLOW_SYMLINKS=YES
    export REMOVE_CVS_FROM_RESOURCES=YES
    export REMOVE_GIT_FROM_RESOURCES=YES
    export REMOVE_HEADERS_FROM_EMBEDDED_BUNDLES=YES
    export REMOVE_HG_FROM_RESOURCES=YES
    export REMOVE_SVN_FROM_RESOURCES=YES
    export REZ_COLLECTOR_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/ResourceManagerResources
    export REZ_OBJECTS_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/ResourceManagerResources/Objects
    export REZ_SEARCH_PATHS="/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator "
    export SCAN_ALL_SOURCE_FILES_FOR_INCLUDES=NO
    export SCRIPTS_FOLDER_PATH=detox-expo-issue.app/Scripts
    export SCRIPT_INPUT_FILE_COUNT=0
    export SCRIPT_OUTPUT_FILE_COUNT=0
    export SDKROOT=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/SDKs/iPhoneSimulator11.4.sdk
    export SDK_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/SDKs/iPhoneSimulator11.4.sdk
    export SDK_DIR_iphonesimulator11_4=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/SDKs/iPhoneSimulator11.4.sdk
    export SDK_NAME=iphonesimulator11.4
    export SDK_NAMES=iphonesimulator11.4
    export SDK_PRODUCT_BUILD_VERSION=15F79
    export SDK_VERSION=11.4
    export SDK_VERSION_ACTUAL=110400
    export SDK_VERSION_MAJOR=110000
    export SDK_VERSION_MINOR=400
    export SED=/usr/bin/sed
    export SEPARATE_STRIP=NO
    export SEPARATE_SYMBOL_EDIT=NO
    export SET_DIR_MODE_OWNER_GROUP=YES
    export SET_FILE_MODE_OWNER_GROUP=NO
    export SHALLOW_BUNDLE=YES
    export SHARED_DERIVED_FILE_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/DerivedSources
    export SHARED_FRAMEWORKS_FOLDER_PATH=detox-expo-issue.app/SharedFrameworks
    export SHARED_PRECOMPS_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/PrecompiledHeaders
    export SHARED_SUPPORT_FOLDER_PATH=detox-expo-issue.app/SharedSupport
    export SKIP_INSTALL=NO
    export SOURCE_ROOT=/Volumes/Guillaume/Projects/detox-expo-issue/ios
    export SRCROOT=/Volumes/Guillaume/Projects/detox-expo-issue/ios
    export STRINGS_FILE_OUTPUT_ENCODING=binary
    export STRIP_BITCODE_FROM_COPIED_FILES=NO
    export STRIP_INSTALLED_PRODUCT=YES
    export STRIP_STYLE=all
    export STRIP_SWIFT_SYMBOLS=YES
    export SUPPORTED_DEVICE_FAMILIES=1,2
    export SUPPORTED_PLATFORMS="iphonesimulator iphoneos"
    export SUPPORTS_TEXT_BASED_API=NO
    export SWIFT_PLATFORM_TARGET_PREFIX=ios
    export SYMROOT=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products
    export SYSTEM_ADMIN_APPS_DIR=/Applications/Utilities
    export SYSTEM_APPS_DIR=/Applications
    export SYSTEM_CORE_SERVICES_DIR=/System/Library/CoreServices
    export SYSTEM_DEMOS_DIR=/Applications/Extras
    export SYSTEM_DEVELOPER_APPS_DIR=/Applications/Xcode.app/Contents/Developer/Applications
    export SYSTEM_DEVELOPER_BIN_DIR=/Applications/Xcode.app/Contents/Developer/usr/bin
    export SYSTEM_DEVELOPER_DEMOS_DIR="/Applications/Xcode.app/Contents/Developer/Applications/Utilities/Built Examples"
    export SYSTEM_DEVELOPER_DIR=/Applications/Xcode.app/Contents/Developer
    export SYSTEM_DEVELOPER_DOC_DIR="/Applications/Xcode.app/Contents/Developer/ADC Reference Library"
    export SYSTEM_DEVELOPER_GRAPHICS_TOOLS_DIR="/Applications/Xcode.app/Contents/Developer/Applications/Graphics Tools"
    export SYSTEM_DEVELOPER_JAVA_TOOLS_DIR="/Applications/Xcode.app/Contents/Developer/Applications/Java Tools"
    export SYSTEM_DEVELOPER_PERFORMANCE_TOOLS_DIR="/Applications/Xcode.app/Contents/Developer/Applications/Performance Tools"
    export SYSTEM_DEVELOPER_RELEASENOTES_DIR="/Applications/Xcode.app/Contents/Developer/ADC Reference Library/releasenotes"
    export SYSTEM_DEVELOPER_TOOLS=/Applications/Xcode.app/Contents/Developer/Tools
    export SYSTEM_DEVELOPER_TOOLS_DOC_DIR="/Applications/Xcode.app/Contents/Developer/ADC Reference Library/documentation/DeveloperTools"
    export SYSTEM_DEVELOPER_TOOLS_RELEASENOTES_DIR="/Applications/Xcode.app/Contents/Developer/ADC Reference Library/releasenotes/DeveloperTools"
    export SYSTEM_DEVELOPER_USR_DIR=/Applications/Xcode.app/Contents/Developer/usr
    export SYSTEM_DEVELOPER_UTILITIES_DIR=/Applications/Xcode.app/Contents/Developer/Applications/Utilities
    export SYSTEM_DOCUMENTATION_DIR=/Library/Documentation
    export SYSTEM_KEXT_INSTALL_PATH=/System/Library/Extensions
    export SYSTEM_LIBRARY_DIR=/System/Library
    export TAPI_VERIFY_MODE=ErrorsOnly
    export TARGETED_DEVICE_FAMILY=1,2
    export TARGETNAME=detox-expo-issue
    export TARGET_BUILD_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator
    export TARGET_DEVICE_IDENTIFIER="dvtdevice-DVTiOSDeviceSimulatorPlaceholder-iphonesimulator:placeholder"
    export TARGET_NAME=detox-expo-issue
    export TARGET_TEMP_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build
    export TEMP_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build
    export TEMP_FILES_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build
    export TEMP_FILE_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build
    export TEMP_ROOT=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex
    export TOOLCHAINS=com.apple.dt.toolchain.XcodeDefault
    export TOOLCHAIN_DIR=/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain
    export TREAT_MISSING_BASELINES_AS_TEST_FAILURES=NO
    export UID=501
    export UNLOCALIZED_RESOURCES_FOLDER_PATH=detox-expo-issue.app
    export UNSTRIPPED_PRODUCT=NO
    export USER=guillaumesarfati
    export USER_APPS_DIR=/Users/guillaumesarfati/Applications
    export USER_LIBRARY_DIR=/Users/guillaumesarfati/Library
    export USE_DYNAMIC_NO_PIC=YES
    export USE_HEADERMAP=YES
    export USE_HEADER_SYMLINKS=NO
    export VALIDATE_PRODUCT=NO
    export VALID_ARCHS="i386 x86_64"
    export VERBOSE_PBXCP=NO
    export VERSIONPLIST_PATH=detox-expo-issue.app/version.plist
    export VERSION_INFO_BUILDER=guillaumesarfati
    export VERSION_INFO_FILE=detox-expo-issue_vers.c
    export VERSION_INFO_STRING="\"@(#)PROGRAM:detox-expo-issue  PROJECT:detox-expo-issue-\""
    export WRAPPER_EXTENSION=app
    export WRAPPER_NAME=detox-expo-issue.app
    export WRAPPER_SUFFIX=.app
    export WRAP_ASSET_PACKS_IN_SEPARATE_DIRECTORIES=NO
    export XCODE_APP_SUPPORT_DIR=/Applications/Xcode.app/Contents/Developer/Library/Xcode
    export XCODE_PRODUCT_BUILD_VERSION=9F2000
    export XCODE_VERSION_ACTUAL=0941
    export XCODE_VERSION_MAJOR=0900
    export XCODE_VERSION_MINOR=0940
    export XPCSERVICES_FOLDER_PATH=detox-expo-issue.app/XPCServices
    export YACC=yacc
    export arch=x86_64
    export diagnostic_message_length=87
    export variant=normal
    /bin/sh -c /Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/Script-B5722AD01DFB7E3F0084848F.sh
/Volumes/Guillaume/Projects/detox-expo-issue /Volumes/Guillaume/Projects/detox-expo-issue/ios
Preparing iOS build at /Volumes/Guillaume/Projects/detox-expo-issue/ios...
/Volumes/Guillaume/Projects/detox-expo-issue/ios

CopyPlistFile build/Build/Products/Debug-iphonesimulator/detox-expo-issue.app/EXBuildConstants.plist detox-expo-issue/Supporting/EXBuildConstants.plist
    cd /Volumes/Guillaume/Projects/detox-expo-issue/ios
    export PATH="/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/usr/bin:/Applications/Xcode.app/Contents/Developer/usr/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin"
    builtin-copyPlist --convert binary1 --outdir /Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/detox-expo-issue.app -- detox-expo-issue/Supporting/EXBuildConstants.plist

PhaseScriptExecution [CP]\ Embed\ Pods\ Frameworks build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/Script-8D34C7FE3D99F20E5EA1B18A.sh
    cd /Volumes/Guillaume/Projects/detox-expo-issue/ios
    /bin/sh -c /Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/Script-8D34C7FE3D99F20E5EA1B18A.sh
mkdir -p /Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/detox-expo-issue.app/Frameworks

PhaseScriptExecution Bundle\ Expo\ Assets build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/Script-19D233B7204FDD7D0087ED51.sh
    cd /Volumes/Guillaume/Projects/detox-expo-issue/ios
    export ACTION=build
    export AD_HOC_CODE_SIGNING_ALLOWED=YES
    export ALTERNATE_GROUP=staff
    export ALTERNATE_MODE=u+w,go-w,a+rX
    export ALTERNATE_OWNER=guillaumesarfati
    export ALWAYS_EMBED_SWIFT_STANDARD_LIBRARIES=NO
    export ALWAYS_SEARCH_USER_PATHS=NO
    export ALWAYS_USE_SEPARATE_HEADERMAPS=NO
    export APPLE_INTERNAL_DEVELOPER_DIR=/AppleInternal/Developer
    export APPLE_INTERNAL_DIR=/AppleInternal
    export APPLE_INTERNAL_DOCUMENTATION_DIR=/AppleInternal/Documentation
    export APPLE_INTERNAL_LIBRARY_DIR=/AppleInternal/Library
    export APPLE_INTERNAL_TOOLS=/AppleInternal/Developer/Tools
    export APPLICATION_EXTENSION_API_ONLY=NO
    export APPLY_RULES_IN_COPY_FILES=NO
    export ARCHS=x86_64
    export ARCHS_STANDARD="i386 x86_64"
    export ARCHS_STANDARD_32_64_BIT="i386 x86_64"
    export ARCHS_STANDARD_32_BIT=i386
    export ARCHS_STANDARD_64_BIT=x86_64
    export ARCHS_STANDARD_INCLUDING_64_BIT="i386 x86_64"
    export ARCHS_UNIVERSAL_IPHONE_OS="i386 x86_64"
    export ASSETCATALOG_COMPILER_APPICON_NAME=AppIcon
    export AVAILABLE_PLATFORMS="appletvos appletvsimulator iphoneos iphonesimulator macosx watchos watchsimulator"
    export BITCODE_GENERATION_MODE=marker
    export BUILD_ACTIVE_RESOURCES_ONLY=YES
    export BUILD_COMPONENTS="headers build"
    export BUILD_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products
    export BUILD_ROOT=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products
    export BUILD_STYLE=
    export BUILD_VARIANTS=normal
    export BUILT_PRODUCTS_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator
    export CACHE_ROOT=/var/folders/w4/5vpc45vd3z1f_cqbncywlvgw0000gn/C/com.apple.DeveloperTools/9.4.1-9F2000/Xcode
    export CCHROOT=/var/folders/w4/5vpc45vd3z1f_cqbncywlvgw0000gn/C/com.apple.DeveloperTools/9.4.1-9F2000/Xcode
    export CHMOD=/bin/chmod
    export CHOWN=/usr/sbin/chown
    export CLANG_ANALYZER_NONNULL=YES
    export CLANG_CXX_LANGUAGE_STANDARD=gnu++0x
    export CLANG_CXX_LIBRARY=libc++
    export CLANG_ENABLE_MODULES=YES
    export CLANG_ENABLE_OBJC_ARC=YES
    export CLANG_MODULES_AUTOLINK=YES
    export CLANG_MODULES_BUILD_SESSION_FILE=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/ModuleCache.noindex/Session.modulevalidation
    export CLANG_WARN_BLOCK_CAPTURE_AUTORELEASING=YES
    export CLANG_WARN_BOOL_CONVERSION=YES
    export CLANG_WARN_COMMA=YES
    export CLANG_WARN_CONSTANT_CONVERSION=YES
    export CLANG_WARN_DIRECT_OBJC_ISA_USAGE=YES_ERROR
    export CLANG_WARN_DOCUMENTATION_COMMENTS=YES
    export CLANG_WARN_EMPTY_BODY=YES
    export CLANG_WARN_ENUM_CONVERSION=YES
    export CLANG_WARN_INFINITE_RECURSION=YES
    export CLANG_WARN_INT_CONVERSION=YES
    export CLANG_WARN_NON_LITERAL_NULL_CONVERSION=YES
    export CLANG_WARN_OBJC_LITERAL_CONVERSION=YES
    export CLANG_WARN_OBJC_ROOT_CLASS=YES_ERROR
    export CLANG_WARN_RANGE_LOOP_ANALYSIS=YES
    export CLANG_WARN_STRICT_PROTOTYPES=YES
    export CLANG_WARN_SUSPICIOUS_MOVE=YES
    export CLANG_WARN_SUSPICIOUS_MOVES=YES
    export CLANG_WARN_UNREACHABLE_CODE=YES
    export CLANG_WARN__DUPLICATE_METHOD_MATCH=YES
    export CLASS_FILE_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/JavaClasses
    export CLEAN_PRECOMPS=YES
    export CLONE_HEADERS=NO
    export CODESIGNING_FOLDER_PATH=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/detox-expo-issue.app
    export CODE_SIGNING_ALLOWED=YES
    export CODE_SIGNING_REQUIRED=YES
    export CODE_SIGN_CONTEXT_CLASS=XCiPhoneSimulatorCodeSignContext
    export CODE_SIGN_IDENTITY=-
    export CODE_SIGN_INJECT_BASE_ENTITLEMENTS=YES
    export COLOR_DIAGNOSTICS=YES
    export COMBINE_HIDPI_IMAGES=NO
    export COMMAND_MODE=legacy
    export COMPILER_INDEX_STORE_ENABLE=Default
    export COMPOSITE_SDK_DIRS=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/CompositeSDKs
    export COMPRESS_PNG_FILES=YES
    export CONFIGURATION=Debug
    export CONFIGURATION_BUILD_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator
    export CONFIGURATION_TEMP_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator
    export CONTENTS_FOLDER_PATH=detox-expo-issue.app
    export COPYING_PRESERVES_HFS_DATA=NO
    export COPY_HEADERS_RUN_UNIFDEF=NO
    export COPY_PHASE_STRIP=NO
    export COPY_RESOURCES_FROM_STATIC_FRAMEWORKS=YES
    export CORRESPONDING_DEVICE_PLATFORM_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform
    export CORRESPONDING_DEVICE_PLATFORM_NAME=iphoneos
    export CORRESPONDING_DEVICE_SDK_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/SDKs/iPhoneOS11.4.sdk
    export CORRESPONDING_DEVICE_SDK_NAME=iphoneos11.4
    export CP=/bin/cp
    export CREATE_INFOPLIST_SECTION_IN_BINARY=NO
    export CURRENT_ARCH=x86_64
    export CURRENT_VARIANT=normal
    export DEAD_CODE_STRIPPING=YES
    export DEBUGGING_SYMBOLS=YES
    export DEBUG_INFORMATION_FORMAT=dwarf
    export DEFAULT_COMPILER=com.apple.compilers.llvm.clang.1_0
    export DEFAULT_KEXT_INSTALL_PATH=/System/Library/Extensions
    export DEFINES_MODULE=NO
    export DEPLOYMENT_LOCATION=NO
    export DEPLOYMENT_POSTPROCESSING=NO
    export DEPLOYMENT_TARGET_CLANG_ENV_NAME=IPHONEOS_DEPLOYMENT_TARGET
    export DEPLOYMENT_TARGET_CLANG_FLAG_NAME=mios-simulator-version-min
    export DEPLOYMENT_TARGET_CLANG_FLAG_PREFIX=-mios-simulator-version-min=
    export DEPLOYMENT_TARGET_SETTING_NAME=IPHONEOS_DEPLOYMENT_TARGET
    export DEPLOYMENT_TARGET_SUGGESTED_VALUES="8.0 8.1 8.2 8.3 8.4 9.0 9.1 9.2 9.3 10.0 10.1 10.2 10.3 11.0 11.1 11.2 11.3 11.4"
    export DERIVED_FILES_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/DerivedSources
    export DERIVED_FILE_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/DerivedSources
    export DERIVED_SOURCES_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/DerivedSources
    export DEVELOPER_APPLICATIONS_DIR=/Applications/Xcode.app/Contents/Developer/Applications
    export DEVELOPER_BIN_DIR=/Applications/Xcode.app/Contents/Developer/usr/bin
    export DEVELOPER_DIR=/Applications/Xcode.app/Contents/Developer
    export DEVELOPER_FRAMEWORKS_DIR=/Applications/Xcode.app/Contents/Developer/Library/Frameworks
    export DEVELOPER_FRAMEWORKS_DIR_QUOTED=/Applications/Xcode.app/Contents/Developer/Library/Frameworks
    export DEVELOPER_LIBRARY_DIR=/Applications/Xcode.app/Contents/Developer/Library
    export DEVELOPER_SDK_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs
    export DEVELOPER_TOOLS_DIR=/Applications/Xcode.app/Contents/Developer/Tools
    export DEVELOPER_USR_DIR=/Applications/Xcode.app/Contents/Developer/usr
    export DEVELOPMENT_LANGUAGE=English
    export DEVELOPMENT_TEAM=C8D8QTF339
    export DOCUMENTATION_FOLDER_PATH=detox-expo-issue.app/English.lproj/Documentation
    export DO_HEADER_SCANNING_IN_JAM=NO
    export DSTROOT=/tmp/detox-expo-issue.dst
    export DT_TOOLCHAIN_DIR=/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain
    export DWARF_DSYM_FILE_NAME=detox-expo-issue.app.dSYM
    export DWARF_DSYM_FILE_SHOULD_ACCOMPANY_PRODUCT=NO
    export DWARF_DSYM_FOLDER_PATH=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator
    export EFFECTIVE_PLATFORM_NAME=-iphonesimulator
    export EMBEDDED_CONTENT_CONTAINS_SWIFT=NO
    export EMBED_ASSET_PACKS_IN_PRODUCT_BUNDLE=NO
    export ENABLE_BITCODE=NO
    export ENABLE_DEFAULT_HEADER_SEARCH_PATHS=YES
    export ENABLE_HEADER_DEPENDENCIES=YES
    export ENABLE_ON_DEMAND_RESOURCES=YES
    export ENABLE_STRICT_OBJC_MSGSEND=YES
    export ENABLE_TESTABILITY=YES
    export ENTITLEMENTS_REQUIRED=YES
    export EXCLUDED_INSTALLSRC_SUBDIRECTORY_PATTERNS=".DS_Store .svn .git .hg CVS"
    export EXCLUDED_RECURSIVE_SEARCH_PATH_SUBDIRECTORIES="*.nib *.lproj *.framework *.gch *.xcode* *.xcassets (*) .DS_Store CVS .svn .git .hg *.pbproj *.pbxproj"
    export EXECUTABLES_FOLDER_PATH=detox-expo-issue.app/Executables
    export EXECUTABLE_FOLDER_PATH=detox-expo-issue.app
    export EXECUTABLE_NAME=detox-expo-issue
    export EXECUTABLE_PATH=detox-expo-issue.app/detox-expo-issue
    export EXPANDED_CODE_SIGN_IDENTITY=-
    export EXPANDED_CODE_SIGN_IDENTITY_NAME=-
    export EXPANDED_PROVISIONING_PROFILE=
    export FILE_LIST=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/Objects/LinkFileList
    export FIXED_FILES_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/FixedFiles
    export FRAMEWORKS_FOLDER_PATH=detox-expo-issue.app/Frameworks
    export FRAMEWORK_FLAG_PREFIX=-framework
    export FRAMEWORK_SEARCH_PATHS="/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator  \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Crashlytics/iOS\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/FBAudienceNetwork\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Fabric/iOS\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Google-Mobile-Ads-SDK/Frameworks/frameworks\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/GoogleAppUtilities/Frameworks/frameworks\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/GoogleAuthUtilities/Frameworks/frameworks\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/GoogleMaps/Base/Frameworks\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/GoogleMaps/Maps/Frameworks\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/GoogleNetworkingUtilities/Frameworks/frameworks\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/GoogleSymbolUtilities/Frameworks/frameworks\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/GoogleUtilities/Frameworks/frameworks\""
    export FRAMEWORK_VERSION=A
    export FULL_PRODUCT_NAME=detox-expo-issue.app
    export GCC3_VERSION=3.3
    export GCC_C_LANGUAGE_STANDARD=gnu99
    export GCC_DYNAMIC_NO_PIC=NO
    export GCC_INLINES_ARE_PRIVATE_EXTERN=YES
    export GCC_NO_COMMON_BLOCKS=YES
    export GCC_OBJC_LEGACY_DISPATCH=YES
    export GCC_OPTIMIZATION_LEVEL=0
    export GCC_PFE_FILE_C_DIALECTS="c objective-c c++ objective-c++"
    export GCC_PREPROCESSOR_DEFINITIONS="DEBUG=1  COCOAPODS=1"
    export GCC_SYMBOLS_PRIVATE_EXTERN=NO
    export GCC_TREAT_WARNINGS_AS_ERRORS=NO
    export GCC_VERSION=com.apple.compilers.llvm.clang.1_0
    export GCC_VERSION_IDENTIFIER=com_apple_compilers_llvm_clang_1_0
    export GCC_WARN_64_TO_32_BIT_CONVERSION=YES
    export GCC_WARN_ABOUT_RETURN_TYPE=YES_ERROR
    export GCC_WARN_UNDECLARED_SELECTOR=YES
    export GCC_WARN_UNINITIALIZED_AUTOS=YES_AGGRESSIVE
    export GCC_WARN_UNUSED_FUNCTION=YES
    export GCC_WARN_UNUSED_VARIABLE=YES
    export GENERATE_MASTER_OBJECT_FILE=NO
    export GENERATE_PKGINFO_FILE=YES
    export GENERATE_PROFILING_CODE=NO
    export GENERATE_TEXT_BASED_STUBS=NO
    export GID=20
    export GROUP=staff
    export HEADERMAP_INCLUDES_FLAT_ENTRIES_FOR_TARGET_BEING_BUILT=YES
    export HEADERMAP_INCLUDES_FRAMEWORK_ENTRIES_FOR_ALL_PRODUCT_TYPES=YES
    export HEADERMAP_INCLUDES_NONPUBLIC_NONPRIVATE_HEADERS=YES
    export HEADERMAP_INCLUDES_PROJECT_HEADERS=YES
    export HEADERMAP_USES_FRAMEWORK_PREFIX_ENTRIES=YES
    export HEADERMAP_USES_VFS=NO
    export HEADER_SEARCH_PATHS="/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/include  \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Amplitude-iOS\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Analytics\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/AppAuth\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Bolts\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Branch\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/CocoaLumberjack\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Crashlytics\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/DoubleConversion\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCamera\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCameraInterface\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXConstants\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXConstantsInterface\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCore\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFaceDetectorInterface\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFileSystem\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFileSystemInterface\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXGL\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXGL-CPP\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXPermissions\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXPermissionsInterface\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXReactNativeAdapter\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSMS\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSensors\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSensorsInterface\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/ExpoKit\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBAudienceNetwork\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKCoreKit\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKLoginKit\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKShareKit\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Fabric\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Folly\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GPUImage\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Google-Maps-iOS-Utils\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Google-Mobile-Ads-SDK\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleAppUtilities\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleAuthUtilities\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleMaps\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleNetworkingUtilities\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleSignIn\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleSymbolUtilities\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleUtilities\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/JKBigInteger2\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/React\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/boost-for-react-native\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/glog\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/lottie-ios\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/yoga\""
    export HIDE_BITCODE_SYMBOLS=YES
    export HOME=/Users/guillaumesarfati
    export ICONV=/usr/bin/iconv
    export INFOPLIST_EXPAND_BUILD_SETTINGS=YES
    export INFOPLIST_FILE=/Volumes/Guillaume/Projects/detox-expo-issue/ios/detox-expo-issue/Supporting/Info.plist
    export INFOPLIST_OUTPUT_FORMAT=binary
    export INFOPLIST_PATH=detox-expo-issue.app/Info.plist
    export INFOPLIST_PREPROCESS=NO
    export INFOSTRINGS_PATH=detox-expo-issue.app/English.lproj/InfoPlist.strings
    export INLINE_PRIVATE_FRAMEWORKS=NO
    export INSTALLHDRS_COPY_PHASE=NO
    export INSTALLHDRS_SCRIPT_PHASE=NO
    export INSTALL_DIR=/tmp/detox-expo-issue.dst/Applications
    export INSTALL_GROUP=staff
    export INSTALL_MODE_FLAG=u+w,go-w,a+rX
    export INSTALL_OWNER=guillaumesarfati
    export INSTALL_PATH=/Applications
    export INSTALL_ROOT=/tmp/detox-expo-issue.dst
    export IPHONEOS_DEPLOYMENT_TARGET=9.0
    export JAVAC_DEFAULT_FLAGS="-J-Xms64m -J-XX:NewSize=4M -J-Dfile.encoding=UTF8"
    export JAVA_APP_STUB=/System/Library/Frameworks/JavaVM.framework/Resources/MacOS/JavaApplicationStub
    export JAVA_ARCHIVE_CLASSES=YES
    export JAVA_ARCHIVE_TYPE=JAR
    export JAVA_COMPILER=/usr/bin/javac
    export JAVA_FOLDER_PATH=detox-expo-issue.app/Java
    export JAVA_FRAMEWORK_RESOURCES_DIRS=Resources
    export JAVA_JAR_FLAGS=cv
    export JAVA_SOURCE_SUBDIR=.
    export JAVA_USE_DEPENDENCIES=YES
    export JAVA_ZIP_FLAGS=-urg
    export JIKES_DEFAULT_FLAGS="+E +OLDCSO"
    export KEEP_PRIVATE_EXTERNS=NO
    export LD_DEPENDENCY_INFO_FILE=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/Objects-normal/x86_64/detox-expo-issue_dependency_info.dat
    export LD_GENERATE_MAP_FILE=NO
    export LD_MAP_FILE_PATH=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/detox-expo-issue-LinkMap-normal-x86_64.txt
    export LD_NO_PIE=NO
    export LD_QUOTE_LINKER_ARGUMENTS_FOR_COMPILER_DRIVER=YES
    export LD_RUNPATH_SEARCH_PATHS=" @executable_path/Frameworks"
    export LEGACY_DEVELOPER_DIR=/Applications/Xcode.app/Contents/PlugIns/Xcode3Core.ideplugin/Contents/SharedSupport/Developer
    export LEX=lex
    export LIBRARY_FLAG_NOSPACE=YES
    export LIBRARY_FLAG_PREFIX=-l
    export LIBRARY_KEXT_INSTALL_PATH=/Library/Extensions
    export LIBRARY_SEARCH_PATHS="/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator  \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/Amplitude-iOS\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/Analytics\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/AppAuth\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/Bolts\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/Branch\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/CocoaLumberjack\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/DoubleConversion\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXCamera\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXConstants\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXCore\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXFileSystem\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXGL\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXGL-CPP\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXPermissions\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXReactNativeAdapter\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXSMS\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/EXSensors\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/ExpoKit\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/FBSDKCoreKit\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/FBSDKLoginKit\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/FBSDKShareKit\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/Folly\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/GPUImage\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/Google-Maps-iOS-Utils\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/JKBigInteger2\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/React\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/glog\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/lottie-ios\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/yoga\" \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/GoogleSignIn/Libraries\""
    export LINKER_DISPLAYS_MANGLED_NAMES=NO
    export LINK_FILE_LIST_normal_x86_64=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/Objects-normal/x86_64/detox-expo-issue.LinkFileList
    export LINK_WITH_STANDARD_LIBRARIES=YES
    export LOCALIZABLE_CONTENT_DIR=
    export LOCALIZED_RESOURCES_FOLDER_PATH=detox-expo-issue.app/English.lproj
    export LOCALIZED_STRING_MACRO_NAMES="NSLocalizedString CFLocalizedString"
    export LOCAL_ADMIN_APPS_DIR=/Applications/Utilities
    export LOCAL_APPS_DIR=/Applications
    export LOCAL_DEVELOPER_DIR=/Library/Developer
    export LOCAL_LIBRARY_DIR=/Library
    export LOCROOT=
    export LOCSYMROOT=
    export MACH_O_TYPE=mh_execute
    export MAC_OS_X_PRODUCT_BUILD_VERSION=17G65
    export MAC_OS_X_VERSION_ACTUAL=101306
    export MAC_OS_X_VERSION_MAJOR=101300
    export MAC_OS_X_VERSION_MINOR=1306
    export METAL_LIBRARY_FILE_BASE=default
    export METAL_LIBRARY_OUTPUT_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/detox-expo-issue.app
    export MODULE_CACHE_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/ModuleCache.noindex
    export MTL_ENABLE_DEBUG_INFO=YES
    export NATIVE_ARCH=i386
    export NATIVE_ARCH_32_BIT=i386
    export NATIVE_ARCH_64_BIT=x86_64
    export NATIVE_ARCH_ACTUAL=x86_64
    export NO_COMMON=YES
    export OBJC_ABI_VERSION=2
    export OBJECT_FILE_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/Objects
    export OBJECT_FILE_DIR_normal=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/Objects-normal
    export OBJROOT=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex
    export ONLY_ACTIVE_ARCH=YES
    export OS=MACOS
    export OSAC=/usr/bin/osacompile
    export OTHER_CFLAGS=" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Amplitude-iOS\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Analytics\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/AppAuth\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Bolts\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Branch\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/CocoaLumberjack\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Crashlytics\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/DoubleConversion\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCamera\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCameraInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXConstants\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXConstantsInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCore\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFaceDetectorInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFileSystem\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFileSystemInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXGL\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXGL-CPP\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXPermissions\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXPermissionsInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXReactNativeAdapter\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSMS\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSensors\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSensorsInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/ExpoKit\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBAudienceNetwork\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKCoreKit\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKLoginKit\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKShareKit\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Fabric\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Folly\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GPUImage\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Google-Maps-iOS-Utils\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Google-Mobile-Ads-SDK\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleAppUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleAuthUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleMaps\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleNetworkingUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleSignIn\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleSymbolUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/JKBigInteger2\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/React\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/boost-for-react-native\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/glog\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/lottie-ios\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/yoga\""
    export OTHER_CPLUSPLUSFLAGS=" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Amplitude-iOS\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Analytics\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/AppAuth\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Bolts\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Branch\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/CocoaLumberjack\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Crashlytics\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/DoubleConversion\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCamera\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCameraInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXConstants\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXConstantsInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXCore\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFaceDetectorInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFileSystem\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXFileSystemInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXGL\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXGL-CPP\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXPermissions\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXPermissionsInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXReactNativeAdapter\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSMS\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSensors\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/EXSensorsInterface\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/ExpoKit\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBAudienceNetwork\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKCoreKit\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKLoginKit\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/FBSDKShareKit\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Fabric\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Folly\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GPUImage\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Google-Maps-iOS-Utils\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/Google-Mobile-Ads-SDK\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleAppUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleAuthUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleMaps\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleNetworkingUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleSignIn\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleSymbolUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/GoogleUtilities\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/JKBigInteger2\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/React\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/boost-for-react-native\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/glog\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/lottie-ios\" -isystem \"/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods/Headers/Public/yoga\""
    export OTHER_LDFLAGS=" -ObjC -l\"Amplitude-iOS\" -l\"Analytics\" -l\"AppAuth\" -l\"Bolts\" -l\"Branch\" -l\"CocoaLumberjack\" -l\"DoubleConversion\" -l\"EXCamera\" -l\"EXConstants\" -l\"EXCore\" -l\"EXFileSystem\" -l\"EXGL\" -l\"EXGL-CPP\" -l\"EXPermissions\" -l\"EXReactNativeAdapter\" -l\"EXSMS\" -l\"EXSensors\" -l\"ExpoKit\" -l\"FBSDKCoreKit\" -l\"FBSDKLoginKit\" -l\"FBSDKShareKit\" -l\"Folly\" -l\"GIPNSURL+FIFE_external\" -l\"GPUImage\" -l\"Google-Maps-iOS-Utils\" -l\"JKBigInteger2\" -l\"React\" -l\"SignIn_external\" -l\"c++\" -l\"glog\" -l\"lottie-ios\" -l\"sqlite3.0\" -l\"stdc++\" -l\"xml2\" -l\"yoga\" -l\"z\" -framework \"AVFoundation\" -framework \"Accelerate\" -framework \"AdSupport\" -framework \"AddressBook\" -framework \"AudioToolbox\" -framework \"CoreData\" -framework \"CoreGraphics\" -framework \"CoreImage\" -framework \"CoreLocation\" -framework \"CoreMedia\" -framework \"CoreMotion\" -framework \"CoreTelephony\" -framework \"CoreText\" -framework \"CoreVideo\" -framework \"Crashlytics\" -framework \"FBAudienceNetwork\" -framework \"Fabric\" -framework \"Foundation\" -framework \"GLKit\" -framework \"GoogleAppUtilities\" -framework \"GoogleAuthUtilities\" -framework \"GoogleMaps\" -framework \"GoogleMapsBase\" -framework \"GoogleMapsCore\" -framework \"GoogleMobileAds\" -framework \"GoogleNetworkingUtilities\" -framework \"GoogleSymbolUtilities\" -framework \"GoogleUtilities\" -framework \"ImageIO\" -framework \"JavaScriptCore\" -framework \"MediaPlayer\" -framework \"MessageUI\" -framework \"MobileCoreServices\" -framework \"OpenGLES\" -framework \"QuartzCore\" -framework \"SafariServices\" -framework \"Security\" -framework \"StoreKit\" -framework \"SystemConfiguration\" -framework \"UIKit\" -weak_framework \"Accounts\" -weak_framework \"AdSupport\" -weak_framework \"AudioToolbox\" -weak_framework \"CoreGraphics\" -weak_framework \"CoreLocation\" -weak_framework \"CoreMotion\" -weak_framework \"Foundation\" -weak_framework \"JavaScriptCore\" -weak_framework \"QuartzCore\" -weak_framework \"SafariServices\" -weak_framework \"Security\" -weak_framework \"Social\" -weak_framework \"UIKit\" -weak_framework \"WebKit\""
    export PACKAGE_TYPE=com.apple.package-type.wrapper.application
    export PASCAL_STRINGS=YES
    export PATH="/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin:/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/local/bin:/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/libexec:/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/usr/bin:/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/usr/local/bin:/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/usr/bin:/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/usr/local/bin:/Applications/Xcode.app/Contents/Developer/usr/bin:/Applications/Xcode.app/Contents/Developer/usr/local/bin:/Applications/Xcode.app/Contents/Developer/Tools:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin"
    export PATH_PREFIXES_EXCLUDED_FROM_HEADER_DEPENDENCIES="/usr/include /usr/local/include /System/Library/Frameworks /System/Library/PrivateFrameworks /Applications/Xcode.app/Contents/Developer/Headers /Applications/Xcode.app/Contents/Developer/SDKs /Applications/Xcode.app/Contents/Developer/Platforms"
    export PBDEVELOPMENTPLIST_PATH=detox-expo-issue.app/pbdevelopment.plist
    export PFE_FILE_C_DIALECTS=objective-c
    export PKGINFO_FILE_PATH=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/PkgInfo
    export PKGINFO_PATH=detox-expo-issue.app/PkgInfo
    export PLATFORM_DEVELOPER_APPLICATIONS_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/Applications
    export PLATFORM_DEVELOPER_BIN_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/usr/bin
    export PLATFORM_DEVELOPER_LIBRARY_DIR=/Applications/Xcode.app/Contents/PlugIns/Xcode3Core.ideplugin/Contents/SharedSupport/Developer/Library
    export PLATFORM_DEVELOPER_SDK_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/SDKs
    export PLATFORM_DEVELOPER_TOOLS_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/Tools
    export PLATFORM_DEVELOPER_USR_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/usr
    export PLATFORM_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform
    export PLATFORM_DISPLAY_NAME="iOS Simulator"
    export PLATFORM_NAME=iphonesimulator
    export PLATFORM_PREFERRED_ARCH=x86_64
    export PLIST_FILE_OUTPUT_FORMAT=binary
    export PLUGINS_FOLDER_PATH=detox-expo-issue.app/PlugIns
    export PODS_BUILD_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products
    export PODS_CONFIGURATION_BUILD_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator
    export PODS_PODFILE_DIR_PATH=/Volumes/Guillaume/Projects/detox-expo-issue/ios/.
    export PODS_ROOT=/Volumes/Guillaume/Projects/detox-expo-issue/ios/Pods
    export PRECOMPS_INCLUDE_HEADERS_FROM_BUILT_PRODUCTS_DIR=YES
    export PRECOMP_DESTINATION_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/PrefixHeaders
    export PRESERVE_DEAD_CODE_INITS_AND_TERMS=NO
    export PRIVATE_HEADERS_FOLDER_PATH=detox-expo-issue.app/PrivateHeaders
    export PRODUCT_BUNDLE_IDENTIFIER=com.detox.issue
    export PRODUCT_MODULE_NAME=detox_expo_issue
    export PRODUCT_NAME=detox-expo-issue
    export PRODUCT_SETTINGS_PATH=/Volumes/Guillaume/Projects/detox-expo-issue/ios/detox-expo-issue/Supporting/Info.plist
    export PRODUCT_TYPE=com.apple.product-type.application
    export PROFILING_CODE=NO
    export PROJECT=detox-expo-issue
    export PROJECT_DERIVED_FILE_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/DerivedSources
    export PROJECT_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios
    export PROJECT_FILE_PATH=/Volumes/Guillaume/Projects/detox-expo-issue/ios/detox-expo-issue.xcodeproj
    export PROJECT_NAME=detox-expo-issue
    export PROJECT_TEMP_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build
    export PROJECT_TEMP_ROOT=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex
    export PUBLIC_HEADERS_FOLDER_PATH=detox-expo-issue.app/Headers
    export RECURSIVE_SEARCH_PATHS_FOLLOW_SYMLINKS=YES
    export REMOVE_CVS_FROM_RESOURCES=YES
    export REMOVE_GIT_FROM_RESOURCES=YES
    export REMOVE_HEADERS_FROM_EMBEDDED_BUNDLES=YES
    export REMOVE_HG_FROM_RESOURCES=YES
    export REMOVE_SVN_FROM_RESOURCES=YES
    export REZ_COLLECTOR_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/ResourceManagerResources
    export REZ_OBJECTS_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/ResourceManagerResources/Objects
    export REZ_SEARCH_PATHS="/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator "
    export SCAN_ALL_SOURCE_FILES_FOR_INCLUDES=NO
    export SCRIPTS_FOLDER_PATH=detox-expo-issue.app/Scripts
    export SCRIPT_INPUT_FILE_COUNT=0
    export SCRIPT_OUTPUT_FILE_COUNT=0
    export SDKROOT=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/SDKs/iPhoneSimulator11.4.sdk
    export SDK_DIR=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/SDKs/iPhoneSimulator11.4.sdk
    export SDK_DIR_iphonesimulator11_4=/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/SDKs/iPhoneSimulator11.4.sdk
    export SDK_NAME=iphonesimulator11.4
    export SDK_NAMES=iphonesimulator11.4
    export SDK_PRODUCT_BUILD_VERSION=15F79
    export SDK_VERSION=11.4
    export SDK_VERSION_ACTUAL=110400
    export SDK_VERSION_MAJOR=110000
    export SDK_VERSION_MINOR=400
    export SED=/usr/bin/sed
    export SEPARATE_STRIP=NO
    export SEPARATE_SYMBOL_EDIT=NO
    export SET_DIR_MODE_OWNER_GROUP=YES
    export SET_FILE_MODE_OWNER_GROUP=NO
    export SHALLOW_BUNDLE=YES
    export SHARED_DERIVED_FILE_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/DerivedSources
    export SHARED_FRAMEWORKS_FOLDER_PATH=detox-expo-issue.app/SharedFrameworks
    export SHARED_PRECOMPS_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/PrecompiledHeaders
    export SHARED_SUPPORT_FOLDER_PATH=detox-expo-issue.app/SharedSupport
    export SKIP_INSTALL=NO
    export SOURCE_ROOT=/Volumes/Guillaume/Projects/detox-expo-issue/ios
    export SRCROOT=/Volumes/Guillaume/Projects/detox-expo-issue/ios
    export STRINGS_FILE_OUTPUT_ENCODING=binary
    export STRIP_BITCODE_FROM_COPIED_FILES=NO
    export STRIP_INSTALLED_PRODUCT=YES
    export STRIP_STYLE=all
    export STRIP_SWIFT_SYMBOLS=YES
    export SUPPORTED_DEVICE_FAMILIES=1,2
    export SUPPORTED_PLATFORMS="iphonesimulator iphoneos"
    export SUPPORTS_TEXT_BASED_API=NO
    export SWIFT_PLATFORM_TARGET_PREFIX=ios
    export SYMROOT=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products
    export SYSTEM_ADMIN_APPS_DIR=/Applications/Utilities
    export SYSTEM_APPS_DIR=/Applications
    export SYSTEM_CORE_SERVICES_DIR=/System/Library/CoreServices
    export SYSTEM_DEMOS_DIR=/Applications/Extras
    export SYSTEM_DEVELOPER_APPS_DIR=/Applications/Xcode.app/Contents/Developer/Applications
    export SYSTEM_DEVELOPER_BIN_DIR=/Applications/Xcode.app/Contents/Developer/usr/bin
    export SYSTEM_DEVELOPER_DEMOS_DIR="/Applications/Xcode.app/Contents/Developer/Applications/Utilities/Built Examples"
    export SYSTEM_DEVELOPER_DIR=/Applications/Xcode.app/Contents/Developer
    export SYSTEM_DEVELOPER_DOC_DIR="/Applications/Xcode.app/Contents/Developer/ADC Reference Library"
    export SYSTEM_DEVELOPER_GRAPHICS_TOOLS_DIR="/Applications/Xcode.app/Contents/Developer/Applications/Graphics Tools"
    export SYSTEM_DEVELOPER_JAVA_TOOLS_DIR="/Applications/Xcode.app/Contents/Developer/Applications/Java Tools"
    export SYSTEM_DEVELOPER_PERFORMANCE_TOOLS_DIR="/Applications/Xcode.app/Contents/Developer/Applications/Performance Tools"
    export SYSTEM_DEVELOPER_RELEASENOTES_DIR="/Applications/Xcode.app/Contents/Developer/ADC Reference Library/releasenotes"
    export SYSTEM_DEVELOPER_TOOLS=/Applications/Xcode.app/Contents/Developer/Tools
    export SYSTEM_DEVELOPER_TOOLS_DOC_DIR="/Applications/Xcode.app/Contents/Developer/ADC Reference Library/documentation/DeveloperTools"
    export SYSTEM_DEVELOPER_TOOLS_RELEASENOTES_DIR="/Applications/Xcode.app/Contents/Developer/ADC Reference Library/releasenotes/DeveloperTools"
    export SYSTEM_DEVELOPER_USR_DIR=/Applications/Xcode.app/Contents/Developer/usr
    export SYSTEM_DEVELOPER_UTILITIES_DIR=/Applications/Xcode.app/Contents/Developer/Applications/Utilities
    export SYSTEM_DOCUMENTATION_DIR=/Library/Documentation
    export SYSTEM_KEXT_INSTALL_PATH=/System/Library/Extensions
    export SYSTEM_LIBRARY_DIR=/System/Library
    export TAPI_VERIFY_MODE=ErrorsOnly
    export TARGETED_DEVICE_FAMILY=1,2
    export TARGETNAME=detox-expo-issue
    export TARGET_BUILD_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator
    export TARGET_DEVICE_IDENTIFIER="dvtdevice-DVTiOSDeviceSimulatorPlaceholder-iphonesimulator:placeholder"
    export TARGET_NAME=detox-expo-issue
    export TARGET_TEMP_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build
    export TEMP_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build
    export TEMP_FILES_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build
    export TEMP_FILE_DIR=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build
    export TEMP_ROOT=/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex
    export TOOLCHAINS=com.apple.dt.toolchain.XcodeDefault
    export TOOLCHAIN_DIR=/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain
    export TREAT_MISSING_BASELINES_AS_TEST_FAILURES=NO
    export UID=501
    export UNLOCALIZED_RESOURCES_FOLDER_PATH=detox-expo-issue.app
    export UNSTRIPPED_PRODUCT=NO
    export USER=guillaumesarfati
    export USER_APPS_DIR=/Users/guillaumesarfati/Applications
    export USER_LIBRARY_DIR=/Users/guillaumesarfati/Library
    export USE_DYNAMIC_NO_PIC=YES
    export USE_HEADERMAP=YES
    export USE_HEADER_SYMLINKS=NO
    export VALIDATE_PRODUCT=NO
    export VALID_ARCHS="i386 x86_64"
    export VERBOSE_PBXCP=NO
    export VERSIONPLIST_PATH=detox-expo-issue.app/version.plist
    export VERSION_INFO_BUILDER=guillaumesarfati
    export VERSION_INFO_FILE=detox-expo-issue_vers.c
    export VERSION_INFO_STRING="\"@(#)PROGRAM:detox-expo-issue  PROJECT:detox-expo-issue-\""
    export WRAPPER_EXTENSION=app
    export WRAPPER_NAME=detox-expo-issue.app
    export WRAPPER_SUFFIX=.app
    export WRAP_ASSET_PACKS_IN_SEPARATE_DIRECTORIES=NO
    export XCODE_APP_SUPPORT_DIR=/Applications/Xcode.app/Contents/Developer/Library/Xcode
    export XCODE_PRODUCT_BUILD_VERSION=9F2000
    export XCODE_VERSION_ACTUAL=0941
    export XCODE_VERSION_MAJOR=0900
    export XCODE_VERSION_MINOR=0940
    export XPCSERVICES_FOLDER_PATH=detox-expo-issue.app/XPCServices
    export YACC=yacc
    export arch=x86_64
    export diagnostic_message_length=87
    export variant=normal
    /bin/sh -c /Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/Script-19D233B7204FDD7D0087ED51.sh
Skipping asset bundling in debug mode.

Touch build/Build/Products/Debug-iphonesimulator/detox-expo-issue.app
    cd /Volumes/Guillaume/Projects/detox-expo-issue/ios
    export PATH="/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/usr/bin:/Applications/Xcode.app/Contents/Developer/usr/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin"
    /usr/bin/touch -c /Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/detox-expo-issue.app

CodeSign build/Build/Products/Debug-iphonesimulator/detox-expo-issue.app
    cd /Volumes/Guillaume/Projects/detox-expo-issue/ios
    export CODESIGN_ALLOCATE=/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/codesign_allocate
    export PATH="/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/usr/bin:/Applications/Xcode.app/Contents/Developer/usr/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin"

Signing Identity:     "-"

    /usr/bin/codesign --force --sign - --entitlements /Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Intermediates.noindex/detox-expo-issue.build/Debug-iphonesimulator/detox-expo-issue.build/detox-expo-issue.app.xcent --timestamp=none /Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/detox-expo-issue.app
/Volumes/Guillaume/Projects/detox-expo-issue/ios/build/Build/Products/Debug-iphonesimulator/detox-expo-issue.app: replacing existing signature

** BUILD SUCCEEDED **

configuration="ios.sim.debug" artifactsLocation="artifacts/ios.sim.debug.2018-08-30 07-46-19Z" node_modules/.bin/jest e2e --config=e2e/config.json --maxWorkers=1 '--testNamePattern=^((?!:android:).)*$'
detox[88207] INFO:  [DetoxServer.js] server listening on localhost:49594...
 FAIL  e2e/firstTest.spec.js (121.137s)
  Example
    ✕ should have welcome screen (7ms)
    ✕ should show hello screen after tap (4ms)
    ✕ should show world screen after tap (1ms)

  ● Example › should have welcome screen

    Timeout - Async callback was not invoked within the 120000ms timeout specified by jest.setTimeout.

      at mapper (../node_modules/jest-jasmine2/build/queue_runner.js:41:52)

  ● Example › should have welcome screen

    ReferenceError: device is not defined

      2 | describe('Example', () => {
      3 |   beforeEach(async () => {
    > 4 |     await device.reloadReactNative();
        |           ^
      5 |   });
      6 |
      7 |   it('should have welcome screen', async () => {

      at Object.device (firstTest.spec.js:4:11)
      at tryCatch (../node_modules/regenerator-runtime/runtime.js:62:40)
      at Generator.invoke [as _invoke] (../node_modules/regenerator-runtime/runtime.js:296:22)
      at Generator.prototype.(anonymous function) [as next] (../node_modules/regenerator-runtime/runtime.js:114:21)
      at tryCatch (../node_modules/regenerator-runtime/runtime.js:62:40)
      at invoke (../node_modules/regenerator-runtime/runtime.js:152:20)
      at ../node_modules/regenerator-runtime/runtime.js:195:11
      at callInvokeWithMethodAndArg (../node_modules/regenerator-runtime/runtime.js:194:16)
      at AsyncIterator.enqueue (../node_modules/regenerator-runtime/runtime.js:217:13)
      at AsyncIterator.prototype.(anonymous function) [as next] (../node_modules/regenerator-runtime/runtime.js:114:21)
      at Object.<anonymous>.runtime.async (../node_modules/regenerator-runtime/runtime.js:241:14)
      at Object._callee (firstTest.spec.js:3:14)

  ● Example › should have welcome screen

    ReferenceError: element is not defined

       5 |   });
       6 |
    >  7 |   it('should have welcome screen', async () => {
         |                                    ^
       8 |     await expect(element(by.id('welcome'))).toBeVisible();
       9 |   });
      10 |

      at Object._callee2$ (firstTest.spec.js:7:36)
      at tryCatch (../node_modules/regenerator-runtime/runtime.js:62:40)
      at Generator.invoke [as _invoke] (../node_modules/regenerator-runtime/runtime.js:296:22)
      at Generator.prototype.(anonymous function) [as next] (../node_modules/regenerator-runtime/runtime.js:114:21)
      at tryCatch (../node_modules/regenerator-runtime/runtime.js:62:40)
      at invoke (../node_modules/regenerator-runtime/runtime.js:152:20)
      at ../node_modules/regenerator-runtime/runtime.js:195:11
      at callInvokeWithMethodAndArg (../node_modules/regenerator-runtime/runtime.js:194:16)
      at AsyncIterator.enqueue (../node_modules/regenerator-runtime/runtime.js:217:13)
      at AsyncIterator.prototype.(anonymous function) [as next] (../node_modules/regenerator-runtime/runtime.js:114:21)
      at Object.<anonymous>.runtime.async (../node_modules/regenerator-runtime/runtime.js:241:14)
      at Object._callee2 (firstTest.spec.js:7:36)

  ● Example › should show hello screen after tap

    Timeout - Async callback was not invoked within the 120000ms timeout specified by jest.setTimeout.

      at mapper (../node_modules/jest-jasmine2/build/queue_runner.js:41:52)

  ● Example › should show hello screen after tap

    ReferenceError: device is not defined

      2 | describe('Example', () => {
      3 |   beforeEach(async () => {
    > 4 |     await device.reloadReactNative();
        |           ^
      5 |   });
      6 |
      7 |   it('should have welcome screen', async () => {

      at Object.device (firstTest.spec.js:4:11)
      at tryCatch (../node_modules/regenerator-runtime/runtime.js:62:40)
      at Generator.invoke [as _invoke] (../node_modules/regenerator-runtime/runtime.js:296:22)
      at Generator.prototype.(anonymous function) [as next] (../node_modules/regenerator-runtime/runtime.js:114:21)
      at tryCatch (../node_modules/regenerator-runtime/runtime.js:62:40)
      at invoke (../node_modules/regenerator-runtime/runtime.js:152:20)
      at ../node_modules/regenerator-runtime/runtime.js:195:11
      at callInvokeWithMethodAndArg (../node_modules/regenerator-runtime/runtime.js:194:16)
      at AsyncIterator.enqueue (../node_modules/regenerator-runtime/runtime.js:217:13)
      at AsyncIterator.prototype.(anonymous function) [as next] (../node_modules/regenerator-runtime/runtime.js:114:21)
      at Object.<anonymous>.runtime.async (../node_modules/regenerator-runtime/runtime.js:241:14)
      at Object._callee (firstTest.spec.js:3:14)

  ● Example › should show hello screen after tap

    ReferenceError: element is not defined

       9 |   });
      10 |
    > 11 |   it('should show hello screen after tap', async () => {
         |                                            ^
      12 |     await element(by.id('hello_button')).tap();
      13 |     await expect(element(by.text('Hello!!!'))).toBeVisible();
      14 |   });

      at Object._callee3$ (firstTest.spec.js:11:44)
      at tryCatch (../node_modules/regenerator-runtime/runtime.js:62:40)
      at Generator.invoke [as _invoke] (../node_modules/regenerator-runtime/runtime.js:296:22)
      at Generator.prototype.(anonymous function) [as next] (../node_modules/regenerator-runtime/runtime.js:114:21)
      at tryCatch (../node_modules/regenerator-runtime/runtime.js:62:40)
      at invoke (../node_modules/regenerator-runtime/runtime.js:152:20)
      at ../node_modules/regenerator-runtime/runtime.js:195:11
      at callInvokeWithMethodAndArg (../node_modules/regenerator-runtime/runtime.js:194:16)
      at AsyncIterator.enqueue (../node_modules/regenerator-runtime/runtime.js:217:13)
      at AsyncIterator.prototype.(anonymous function) [as next] (../node_modules/regenerator-runtime/runtime.js:114:21)
      at Object.<anonymous>.runtime.async (../node_modules/regenerator-runtime/runtime.js:241:14)
      at Object._callee3 (firstTest.spec.js:11:44)

  ● Example › should show world screen after tap

    Timeout - Async callback was not invoked within the 120000ms timeout specified by jest.setTimeout.

      at mapper (../node_modules/jest-jasmine2/build/queue_runner.js:41:52)

  ● Example › should show world screen after tap

    ReferenceError: device is not defined

      2 | describe('Example', () => {
      3 |   beforeEach(async () => {
    > 4 |     await device.reloadReactNative();
        |           ^
      5 |   });
      6 |
      7 |   it('should have welcome screen', async () => {

      at Object.device (firstTest.spec.js:4:11)
      at tryCatch (../node_modules/regenerator-runtime/runtime.js:62:40)
      at Generator.invoke [as _invoke] (../node_modules/regenerator-runtime/runtime.js:296:22)
      at Generator.prototype.(anonymous function) [as next] (../node_modules/regenerator-runtime/runtime.js:114:21)
      at tryCatch (../node_modules/regenerator-runtime/runtime.js:62:40)
      at invoke (../node_modules/regenerator-runtime/runtime.js:152:20)
      at ../node_modules/regenerator-runtime/runtime.js:195:11
      at callInvokeWithMethodAndArg (../node_modules/regenerator-runtime/runtime.js:194:16)
      at AsyncIterator.enqueue (../node_modules/regenerator-runtime/runtime.js:217:13)
      at AsyncIterator.prototype.(anonymous function) [as next] (../node_modules/regenerator-runtime/runtime.js:114:21)
      at Object.<anonymous>.runtime.async (../node_modules/regenerator-runtime/runtime.js:241:14)
      at Object._callee (firstTest.spec.js:3:14)

  ● Example › should show world screen after tap

    ReferenceError: element is not defined

      14 |   });
      15 |
    > 16 |   it('should show world screen after tap', async () => {
         |                                            ^
      17 |     await element(by.id('world_button')).tap();
      18 |     await expect(element(by.text('World!!!'))).toBeVisible();
      19 |   });

      at Object._callee4$ (firstTest.spec.js:16:44)
      at tryCatch (../node_modules/regenerator-runtime/runtime.js:62:40)
      at Generator.invoke [as _invoke] (../node_modules/regenerator-runtime/runtime.js:296:22)
      at Generator.prototype.(anonymous function) [as next] (../node_modules/regenerator-runtime/runtime.js:114:21)
      at tryCatch (../node_modules/regenerator-runtime/runtime.js:62:40)
      at invoke (../node_modules/regenerator-runtime/runtime.js:152:20)
      at ../node_modules/regenerator-runtime/runtime.js:195:11
      at callInvokeWithMethodAndArg (../node_modules/regenerator-runtime/runtime.js:194:16)
      at AsyncIterator.enqueue (../node_modules/regenerator-runtime/runtime.js:217:13)
      at AsyncIterator.prototype.(anonymous function) [as next] (../node_modules/regenerator-runtime/runtime.js:114:21)
      at Object.<anonymous>.runtime.async (../node_modules/regenerator-runtime/runtime.js:241:14)
      at Object._callee4 (firstTest.spec.js:16:44)

Test Suites: 1 failed, 1 total
Tests:       3 failed, 3 total
Snapshots:   0 total
Time:        121.186s
Ran all test suites matching /e2e/i with tests matching "^((?!:android:).)*$".
child_process.js:644
    throw err;
    ^

Error: Command failed: node_modules/.bin/jest e2e --config=e2e/config.json --maxWorkers=1 '--testNamePattern=^((?!:android:).)*$'
    at checkExecSyncError (child_process.js:601:13)
    at Object.execSync (child_process.js:641:13)
    at runJest (/Volumes/Guillaume/Projects/detox-expo-issue/node_modules/detox/local-cli/detox-test.js:154:6)
    at run (/Volumes/Guillaume/Projects/detox-expo-issue/node_modules/detox/local-cli/detox-test.js:85:7)
    at Object.<anonymous> (/Volumes/Guillaume/Projects/detox-expo-issue/node_modules/detox/local-cli/detox-test.js:217:1)
    at Module._compile (module.js:652:30)
    at Object.Module._extensions..js (module.js:663:10)
    at Module.load (module.js:565:32)
    at tryModuleLoad (module.js:505:12)
    at Function.Module._load (module.js:497:3)
```
