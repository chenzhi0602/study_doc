# nio study
## java nio中的一些Channel
        FileChannel
        DatagramChannel
        SocketChannel
        ServerSocketChannel
其中涵盖了`IO`,`UDP`,`TCP`

## nio buffer
* ByteBuffer->byte
* CharBuffer->char
* DoubleBuffer->double
* FloatBuffer->float
* IntBuffer->int
* LongBuffer->long
* ShortBuffer->short

## Selector
要使用Selector，得向Selector注册Channel，然后调用它的select()方法。这个方法会一直阻塞到某个注册的通道有事件就绪。一旦这个方法返回，线程就可以处理这些事件，事件的例子有如新连接进来，数据接收等。








