# CMakeLists.txt
cmake_minimum_required(VERSION 4.3)
project(MyProject)

# Find packages
find_package(fmt REQUIRED)
find_package(spdlog REQUIRED)
find_package(nlohmann_json REQUIRED)

# Link libraries
add_executable(app main.cpp)
target_link_libraries(app PRIVATE
    fmt::fmt
    spdlog::spdlog
    nlohmann_json::nlohmann_json)
set_target_properties(app PROPERTIES DEBUG_POSTFIX ${CMAKE_DEBUG_POSTFIX})

set(targetsFile ${PROJECT_NAME}-targets)
xpExternPackage(REPO_NAME tutorial
  TARGETS_FILE ${targetsFile} EXE app
  BASE v1.1 XPDIFF "patch"
  WEB "https://github.com/smanders/tutorial" UPSTREAM "github.com/externpro/tutorial"
  DESC "A simple externpro tutorial project"
  LICENSE "[MIT](https://github.com/externpro/tutorial?tab=MIT-1-ov-file#readme 'MIT License')"
  )
install(TARGETS app EXPORT ${targetsFile} DESTINATION ${CMAKE_INSTALL_BINDIR})
install(EXPORT ${targetsFile} DESTINATION ${CMAKE_INSTALL_CMAKEDIR} NAMESPACE tutorial::)
