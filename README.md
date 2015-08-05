This is a somewhat skeleton eclipse project whose sole purpose is to build a static version of libpcap, libpcap is cloned from Android
Source site at:https://android.googlesource.com/platform/external/libpcap/, at my own descretion I removed some of those .3pcap, .3pcap.in files, also some multiplatform files are included, because I am not sure whether deleting them
will cause compile and build failure. Please refer to the original source trunk for all the original files.

Usage instruction (windows only, linux should be similar)

1) Open CMD.exe, type 
cd {Path_of_Unziped_File}
set NDK_PATH={path_to_where_NDK_installed}

2) Then in project root directory type:
   %NDK_PATH%/ndk-build
   
   Voila! Now you have a libpcap.a which can be used for many fun applications, for an example of how to use it see:
   http://blog.umitproject.org/2011/05/libpcap-for-android.html
   
   Have fun sniffing!
