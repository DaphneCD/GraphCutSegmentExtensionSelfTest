cmake_minimum_required(VERSION 2.8.9)

project(GraphCutSelfTest)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "http://slicer.org/slicerWiki/index.php/Documentation/Nightly/Extensions/GraphCutSelfTest")
set(EXTENSION_CATEGORY "Examples")
set(EXTENSION_CONTRIBUTORS "Danfeng Chen (Western University)")
set(EXTENSION_DESCRIPTION "This is an example of a simple extension")
set(EXTENSION_ICONURL "http://www.example.com/Slicer/Extensions/GraphCutSelfTest.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/GraphCutSelfTest/Screenshots/1.png")

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(GraphCutSegmentSelfTest)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
