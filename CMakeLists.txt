CMAKE_MINIMUM_REQUIRED(VERSION 2.4.5)

PROJECT(vtkLandmarkAndICP)

FIND_PACKAGE(VTK REQUIRED)
INCLUDE(${VTK_USE_FILE})

ADD_EXECUTABLE(lmicp main.cpp)
TARGET_LINK_LIBRARIES(lmicp ${VTK_LIBRARIES})