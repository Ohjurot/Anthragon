project("anthragon-core")

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)


add_library(${PROJECT_NAME}
    "UseDummy.cpp"
    "IoCContainer.cpp"
)

target_compile_features(${PROJECT_NAME} PUBLIC cxx_std_17)
target_include_directories(${PROJECT_NAME} PUBLIC "${CMAKE_SOURCE_DIR}/include")
