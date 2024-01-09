file(GLOB_RECURSE EWMATH_INC  *.h *.hpp)
file(GLOB_RECURSE EWMATH_SRC  *.c *.cpp)

add_library(ewMath STATIC ${EWMATH_SRC} ${EWMATH_INC})

install (TARGETS ewMath DESTINATION lib)
install (FILES ${EWMATH_INC} DESTINATION include/ewMath)