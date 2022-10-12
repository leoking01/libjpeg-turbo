project(TestInstallation)
cmake_minimum_required(VERSION 3.5)

find_package(jpeg 1.0  PATHS  "E:\\downloadBaidu\\a_png\\aa_libjpeg-turbo\\libjpeg-turbo_19.0.24215.1_install")

add_executable(mymathApp mymathApp.cc tjexample.c )
target_link_libraries(mymathApp  turbojpeg )
target_include_directories(mymathApp  PRIVATE  "E:\\downloadBaidu\\a_png\\aa_libjpeg-turbo\\libjpeg-turbo_19.0.24215.1_install/include")
target_link_directories(mymathApp  PRIVATE  "E:\\downloadBaidu\\a_png\\aa_libjpeg-turbo\\libjpeg-turbo_19.0.24215.1_install/lib")
