# nio study
nio核心组件：channel,buffer,selector
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


# Channel
    nio channel既可以从通道中读取数据，又可以写数据到通道。而流的读写通常是单向的
    channel可以异步地读写
    通道中数据总是先读取到一个buffer，或从一个buffer写入


# Buffer
capacity,position,limit
flip()将buffer从写模式切换到读模式

# Selector
一个Selector可以处理多个Channel
与Selector一起使用时，channel必须处于非阻塞模式下，这意味着不能将selector与filechannel一起使用，因为filechannel不能切换至非阻塞模式

# nio和io区别
        IO          NIO
        面向流      面向缓冲
        阻塞IO      非阻塞IO
        无          选择器

nio study url
http://ifeve.com/overview/





