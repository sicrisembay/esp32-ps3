set(srcs    "src/ps3.c"
            "src/ps3_spp.c"
            "src/ps3_parser.c"
            "src/ps3_l2cap.c"
)

set(reqs "nvs_flash"
         "bt")

set(include_dirs "src/include")

set(priv_include_dirs "src")

idf_component_register(SRCS ${srcs}
                    REQUIRES ${reqs}
                    PRIV_INCLUDE_DIRS ${priv_include_dirs}
                    INCLUDE_DIRS ${include_dirs})