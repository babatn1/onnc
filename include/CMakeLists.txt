
install(DIRECTORY onnc DESTINATION include
    FILES_MATCHING
    PATTERN "*"
    PATTERN "*.in" EXCLUDE
    PATTERN "Makefile.am" EXCLUDE)

install(DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}/onnc DESTINATION include
    FILES_MATCHING
    PATTERN "*.h"
    PATTERN "*.def")
