package(default_visibility = ["//visibility:public"])

cc_library(
  name = "base",
  srcs = [
    "flags.cc",
    "init.cc",
    "logging.cc",
    "status.cc",
    "strtoint.cc",
  ],
  hdrs = [
    "bitcast.h",
    "flags.h",
    "init.h",
    "logging.h",
    "macros.h",
    "port.h",
    "slice.h",
    "status.h",
    "strtoint.h",
    "types.h",
  ],
  linkopts = [
    "-lpthread",
  ],
)

cc_library(
  name = "libinit",
  srcs = ["libinit.cc"],
  deps = [
    ":base",
  ],
  alwayslink = 1,
)

cc_library(
  name = "registry",
  srcs = ["registry.cc"],
  hdrs = ["registry.h"],
  deps = [
    ":base",
  ],
)

cc_library(
  name = "clock",
  srcs = ["clock.cc"],
  hdrs = ["clock.h"],
  deps = [
    ":base",
  ],
)

