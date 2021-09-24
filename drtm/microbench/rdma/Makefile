LIBS= -lzmq -lrt -libverbs
LDFLAGS = -pthread -L/usr/local/ofed/lib64 -L/usr/local/ofed/lib
PLATFORM_CCFLAGS=-I/usr/local/ofed/include   -pthread   
PLATFORM_CXXFLAGS=-I/usr/local/ofed/include   -pthread   		

CPP=g++
CPPFLAGS=-g2 -fpermissive 

micro:
	$(CPP) $(CPPFLAGS) -o micro -std=c++0x -I.. rdma_lib.cc  rdma_micro.cc    $(LDFLAGS) $(PLATFORM_CXXFLAGS) $(LIBS)	
