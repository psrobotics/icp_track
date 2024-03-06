cmake_minimum_required(VERSION 3.10)
project(icp_track)

# Set the C++ standard
set(CMAKE_CXX_STANDARD 11)

# Find Eigen library
find_package(Eigen3 REQUIRED)

# Include directories for Eigen
include_directories(${EIGEN3_INCLUDE_DIR})

# Add your source files
set(SOURCE_FILES
    src/test.cpp
    src/icp.cpp
    # Add other source files if any
)

# Create the executable
add_executable(${PROJECT_NAME} ${SOURCE_FILES})
