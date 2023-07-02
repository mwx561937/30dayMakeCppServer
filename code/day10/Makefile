server:
	g++ src/util.cpp src/Buffer.cpp src/Socket.cpp src/InetAddress.cpp client.cpp -g -o client && \
	g++ server.cpp -g  \
	-pthread \
	src/util.cpp src/Epoll.cpp src/InetAddress.cpp src/Socket.cpp src/Connection.cpp \
	src/Channel.cpp src/EventLoop.cpp src/Server.cpp src/Acceptor.cpp src/Buffer.cpp \
	src/ThreadPool.cpp \
	-o server
clean:
	rm server && rm client

threadTest:
	g++ -pthread src/ThreadPool.cpp ThreadPoolTest.cpp -o -g ThreadPoolTest