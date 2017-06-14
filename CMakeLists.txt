add_library(winpthreads STATIC
    ./src/barrier.c
    ./src/barrier.h
    ./src/clock.c
    ./src/cond.c
    ./src/cond.h
    ./src/misc.c
    ./src/misc.h
    ./src/mutex.c
    ./src/nanosleep.c
    ./src/ref.c
    ./src/ref.h
    ./src/rwlock.c
    ./src/rwlock.h
    ./src/sched.c
    ./src/sem.c
    ./src/sem.h
    ./src/spinlock.c
    ./src/thread.c
    ./src/thread.h
    ./src/winpthread_internal.h
    ./src/wpth_ver.h
	"${CMAKE_CURRENT_SOURCE_DIR}/include/pthread.h")

target_include_directories(winpthreads PUBLIC "${CMAKE_CURRENT_LIST_DIR}/include")