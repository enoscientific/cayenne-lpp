# bme280
ESP-IDF Bosch BME280 Driver
BME280 v3.5.0

Just the BME280 driver  organized as a ESP-IDF component.

To use, git clone/submodule to `components` directory.

Or add to `CmakeLists.txt` file:
```
# Adds a new cmake function
include(FetchContent)
# Add remote libraries, which will be pulled down when this project is first built, and cached.


FetchContent_Declare(
  bme280
  GIT_REPOSITORY https://github.com/enoscientific/bme280.git
)

FetchContent_MakeAvailable(bme280)
set(EXTRA_COMPONENT_DIRS ${bme280_SOURCE_DIR}/components)

```
