project(Cucumber)
enable_language(Fortran)

set(GCC_COVERAGE_COMPILE_FLAGS "-flto -Ofast -march=native")
#set(GCC_COVERAGE_COMPILE_FLAGS "-g -fsanitize=address")
set(CMAKE_Fortran_FLAGS "${GCC_COVERAGE_COMPILE_FLAGS}")


add_executable(Cucumber_f90 main.f90)