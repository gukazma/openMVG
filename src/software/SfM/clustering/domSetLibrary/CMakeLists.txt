add_library( domset STATIC domset.cc domset.h types.h )
target_include_directories(domset PUBLIC ${EIGEN_INCLUDE_DIRS})
target_link_libraries(domset PRIVATE openMVG_matching Eigen3::Eigen)
set_property(TARGET domset PROPERTY FOLDER OpenMVG/software/clustering)
