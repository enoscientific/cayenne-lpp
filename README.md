## A Cayenne LPP library written in C

This library provides functions for generating Cayenne LPP compatible payload.
For example, the generated payloads can be used with LoRaWAN devices.

## Source Driver Repository

Currently, this component clones this repo https://aabadie.github.io/cayenne-lpp and sets it up as a ESP-IDF component.

## Usage

To use, git clone/submodule to `components` directory.

Or add to `CmakeLists.txt` file:
```
# Adds a new cmake function
include(FetchContent)
# Add remote libraries, which will be pulled down when this project is first built, and cached.


FetchContent_Declare(
  cayenne
  GIT_REPOSITORY https://github.com/enoscientific/cayenne-lpp.git
)

FetchContent_MakeAvailable(cayenne)
set(EXTRA_COMPONENT_DIRS ${cayenne_SOURCE_DIR}/components)

```
