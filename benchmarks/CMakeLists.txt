project(benchmarks)

include_directories(BEFORE ${csympy_SOURCE_DIR}/src)
include_directories(BEFORE ${csympy_BINARY_DIR}/src)
include_directories(BEFORE ${teuchos_SOURCE_DIR})
include_directories(BEFORE ${teuchos_BINARY_DIR})

add_executable(expand1 expand1.cpp)
target_link_libraries(expand1 csympy teuchos ${LIBS})

add_executable(expand2 expand2.cpp)
target_link_libraries(expand2 csympy teuchos ${LIBS})

add_executable(expand2b expand2b.cpp)
target_link_libraries(expand2b csympy teuchos ${LIBS})

add_executable(expand3 expand3.cpp)
target_link_libraries(expand3 csympy teuchos ${LIBS})

add_executable(add1 add1.cpp)
target_link_libraries(add1 csympy teuchos ${LIBS})

add_executable(matrix_add1 matrix_add1.cpp)
target_link_libraries(matrix_add1 csympy teuchos ${LIBS})

add_executable(matrix_add2 matrix_add2.cpp)
target_link_libraries(matrix_add2 csympy teuchos ${LIBS})

add_executable(matrix_mul1 matrix_mul1.cpp)
target_link_libraries(matrix_mul1 csympy teuchos ${LIBS})

add_executable(matrix_mul2 matrix_mul2.cpp)
target_link_libraries(matrix_mul2 csympy teuchos ${LIBS})
