NAME=util
LIBDIR=lib  # تعریف مسیر ذخیره بایبلیوتک
SRC=$(wildcard *.cpp)
OBJS=$(SRC:.cpp=.o)

all: ${LIBDIR}/lib${NAME}.a

${LIBDIR}/lib${NAME}.a: ${OBJS}
    mkdir -p ${LIBDIR}
    ar rvs ${LIBDIR}/lib${NAME}.a ${OBJS}

clean:
    rm -rf *.o
    rm -rf ${LIBDIR}
