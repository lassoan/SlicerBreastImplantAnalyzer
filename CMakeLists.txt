cmake_minimum_required(VERSION 3.13.4)

project(BreastImplantAnalyzer)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://github.com/lassoan/SlicerBreastImplantAnalyzer#breastimplantanalyzer")
set(EXTENSION_CATEGORY "Quantification")
set(EXTENSION_CONTRIBUTORS "Lance Levine (University of Miami Miller School of Medicine), Marc Levine (Penn State University College of Medicine), Dr. Wrood Kassira (University of Miami Department of Plastic & Reconstructive Surgery)")
set(EXTENSION_DESCRIPTION "This extension allows the user to calculate the volume of a breast implant from breast MRI data with minimal user input.")
set(EXTENSION_ICONURL "https://raw.githubusercontent.com/lancelevine/SlicerBreastImplantAnalyzer/master/BreastImplantAnalyzer.png")
set(EXTENSION_SCREENSHOTURLS "https://raw.githubusercontent.com/lancelevine/SlicerBreastImplantAnalyzer/master/Screenshot01.PNG")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(BreastImplantAnalyzer)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
