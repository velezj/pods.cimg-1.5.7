cmake_minimum_required(VERSION 2.6.0)

# pull in the pods macros. See cmake/pods.cmake for documentation
set(POD_NAME cimg-1.5.7)
include(cmake/pods.cmake)


pods_install_headers(
    CImg-1.5.7/CImg.h
    DESTINATION
    cimg/
)
pods_install_pkg_config_file( cimg-1.5.7
  VERSION 1.5.7
  LIBS "-lX11"
)
