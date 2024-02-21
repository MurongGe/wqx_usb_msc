file(GLOB BSP_SRC
        sys/*.c
        w25qxx/*.c
        )

# 这句命令的位置不对会报错
add_library(bsp ${BSP_SRC})

target_include_directories(bsp PUBLIC
        sys
        w25qxx
        )