# CppLibPackage
* Runtime Library MT/MTd only, x86 and x64
* 2022 vcpkg사용해서 아래 커맨드로 빌드했음.
  * [LIB_NAME]:x64 or x86 -static

# 구성
* Cryptopp
   * cryptopp_8_5_0_x64_static
   * cryptopp_8_5_0_x86_static

* CURL
  * curl-7.81.0_x64_static
  * curl-7.80.0_x86_static => include zlib_1.2.11
  * Preprocessor => CURL_STATICLIB
  * Add Dependency => 
    * Debug : libcurl-d.lib, crypt32.lib, zlibd.lib
    * Release : libcurl.lib, crypt32.lib, zlib.lib

* JsonCpp
  * jsoncpp_1_9_5_x64_static
  * jsoncpp_1_9_5_x86_static
  * Preprocessor => Maybe Need? => _WINSOCK_DEPRECATED_NO_WARNINGS

* Protobuf
  * protobuf_3.18.0_x64_static
  * protobuf_3.18.0_x86_static

# CopyRight
각 파일안에 있음.
