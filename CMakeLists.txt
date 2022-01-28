cmake_minimum_required(VERSION 3.13.4)

project(LineIntensityProfileExtension)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://www.slicer.org/wiki/Documentation/Nightly/Extensions/LineIntensityProfileExtension")
set(EXTENSION_CATEGORY "Assignment")
set(EXTENSION_CONTRIBUTORS "Dineth Mudalige (UoM)")
set(EXTENSION_DESCRIPTION "This extension is developed as part of Slicer extension writing")
set(EXTENSION_ICONURL "http://www.example.com/Slicer/Extensions/LineIntensityProfileExtension.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/LineIntensityProfileExtension/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(LineIntensityProfile)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
