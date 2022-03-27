---
title: Elixir + Python = ❤️
layout: post
---

Python will always hold a special place in my heart. It was the first
programming language that I truly sank my teeth into and used it to _get stuff
done_. I later learned about Elixir, and it made it _easy_ to implement highly
concurrent, asynchronous systems. Both serve different purposes in my books - I
wouldn't want to do any general numerical computing with Elixir[^1] nor could I
imagine how to build the kind of resilience into a complex Python application
that the BEAM provides essentially for free.

[I gave a talk at ElixirConf](https://www.youtube.com/watch?v=dkdiwMONJF4) a few
years ago describing a service that enabled the execution of arbitrary Python
applications on a scientific compute cluster via an HTTP API provided by
Elixir. This provided a really clean separation of concerns between teams, and
also provided a simple interface on an existing application framework.

This is going to be the start on a small series of posts outlining how to get
such a system working, and considerations for your own needs. I'm working on an
example project called [Portage] to go along with this series as I expand on
various topics, but I don't yet know if it's something that could be turned into
a general purpose library...  Time will tell.

[^1]: To be fair, I haven't played with [Nx] yet... my opinions may change.
[Portage]: https://github.com/ngeraedts/portage
[Nx]: https://github.com/elixir-nx/nx
