target_sources(${PROJECT_NAME}
    PRIVATE
    # {{BEGIN_TARGET_SOURCES}}
    ${CMAKE_CURRENT_LIST_DIR}/startup.s
    ${CMAKE_CURRENT_LIST_DIR}/vector.s
    ${CMAKE_CURRENT_LIST_DIR}/eiint_handler.c
    ${CMAKE_CURRENT_LIST_DIR}/main.c
    ${CMAKE_CURRENT_LIST_DIR}/tests/RegTest.s
    ${CMAKE_CURRENT_LIST_DIR}/tests/main_blink.c
    ${CMAKE_CURRENT_LIST_DIR}/tests/main_full.c
    ${CMAKE_CURRENT_LIST_DIR}/tests/IntQueue.c
    ${CMAKE_CURRENT_LIST_DIR}/tests/IntQueueTimer.c
    ${CMAKE_CURRENT_LIST_DIR}/tests/blocktim.c
    ${CMAKE_CURRENT_LIST_DIR}/tests/countsem.c
    ${CMAKE_CURRENT_LIST_DIR}/tests/recmutex.c
    # {{END_TARGET_SOURCES}}
)

target_include_directories(${PROJECT_NAME}
    PUBLIC
    ${CMAKE_CURRENT_LIST_DIR}/include
    ${CMAKE_CURRENT_LIST_DIR}/tests/include
)
