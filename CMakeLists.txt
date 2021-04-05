# CMakeList.txt : CMake project for LearnWxWidgets, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

project ("LearnWxWidgets")

# Add source to this project's executable.
add_executable (LearnWxWidgets	WIN32 "LearnWxWidgets.cpp" "LearnWxWidgets.h")


include_directories(LearnWxWidgets "C:/Users/adhir/Downloads/wxMSW-3.1.4_vc14x_x64_Dev/lib/vc14x_x64_dll/mswud")
include_directories(LearnWxWidgets "C:/Users/adhir/Downloads/wxWidgets-3.1.4-headers/include")

target_link_libraries(LearnWxWidgets LINK_PUBLIC "C:/Users/adhir/Downloads/wxMSW-3.1.4_vc14x_x64_Dev/lib/vc14x_x64_dll/wxmsw31ud_core.lib")
target_link_libraries(LearnWxWidgets LINK_PUBLIC "C:/Users/adhir/Downloads/wxMSW-3.1.4_vc14x_x64_Dev/lib/vc14x_x64_dll/wxbase31ud.lib")
target_link_libraries(LearnWxWidgets LINK_PUBLIC "C:/Users/adhir/Downloads/wxMSW-3.1.4_vc14x_x64_Dev/lib/vc14x_x64_dll/wxbase31ud_net.lib")

# TODO: Add tests and install targets if needed.
