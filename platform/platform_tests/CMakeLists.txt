project(platform_tests)

set(
  SRC
  country_file_tests.cpp
  jansson_test.cpp
  language_test.cpp
  measurement_tests.cpp
  mwm_version_test.cpp
  platform_test.cpp
)

geocore_add_test(${PROJECT_NAME} ${SRC})

geocore_link_libraries(
  ${PROJECT_NAME}
  platform_tests_support
  platform
)

