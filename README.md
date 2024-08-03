# webgraph
Webgraph++ code (http://cnets.indiana.edu/groups/nan/webgraph/)

This code worked for what I used it for, but I cannot promise it is
thorougly tested and there are almost certainly some strange bugs!
Your help would be greatly appreciated in adding tests and generally
cleaning it up.

I have moved on and do not have much time to answer questions about
setup and compilation, so this code is provided AS-IS. With that
said, I hope it is useful or at least interesting.

You will definitely need Boost (http://www.boost.org/) to make this
work.

You will notice a lot of TODOs and commented-out unimplemented
methods. Feel free to write them :)

## Make

Use `BOOST_ROOT` to specify the location of your Boost installation, as below:

```sh
make BOOST_ROOT=/path/to/boost
```

Compile success with g++ 11.4.0 and Boost 1.84.0.
