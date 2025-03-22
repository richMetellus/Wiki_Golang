# Quora

**What are the top 10 use cases of Go language?** - Martin Kock

Go is Turing complete and can therefore - theoretically - be utilised to build
pretty much anything. That being said, the language has strengths and weaknesses
just like any other language that makes it more suitable for certain types of
software and less suitable for others. The following is purely my own interpretation,
but it’s also based on knowledge about a variety of projects (open source as 
well as projects made for and by private companies).

Go is particularly good for:

1. **Containerisation**, ie. system-level software that interacts with the OS
through its public API. Examples: Docker, Kubernetes.

2. High-performance scalable database implementations. Examples: CockroachDB, InfluxDB.
3. Any server-side service, including but not limited to, pub/sub servers and clients,
caching mechanisms, integration layers, high-CPU utilisation jobs such as number
crunching, statistics and cryptographic algorithms, jobs involving high levels
of I/O and where there are extremely high requirements for simultaneous processing
of thousands or millions of HTTP requests. Examples: Handling 1 Million Requests
per Minute with Golang.
4. Any type of API using REST, GraphQL or gRPC. Examples are abundant, but both
Dropbox, Uber and GitHub are known to have built API’s in Go.
5. Any kind of CPU-bound or I/O-bound local processing. Example: my own XML parser
that was 85% faster than the corresponding XML parser in Node.js.
6. Cryptocurrency. Go has been used for the Bitcoin Lightning Network and Ethereum blockchain.
7. Command Line Tools. Examples: Snappy the package manager for Linux that is
taking over from APT in certain distros, is developed in Go.
8. Site building: I don’t (yet) see any WordPress killer written in Go, but I’ve
tried Hugo, a pretty awesome (and fast!) static site generator that will generate
your HTML with navigation and all, from a bunch of Markdown files.
9. DevOps: Go is being used within DevOps, for writing update scripts, server
maintenance software, batch processing etc. It’s as fast - if not faster - than Python to write, performs better and is easier to debug. Don’t ask me for sources on this one, I don’t remember where I got this from :-)
10. WASM (WebAssembly) support is new and still experimental, but I see a bright
future for Go in this category, due to Go’s excellent support for UTF-8, concurrency
and ease of use.

That was my Top Ten, I believe!

So, what is Go not good at? Although (small) games and UI-driven applications have
been developed with Go, it’s not really this kind of stuff that Go was designed for.
This is probably just a matter of getting enough traction (and interest) behind
the language for these use cases so that the bindings can be implemented for
whatever you need here, such as (this is really not my area, so I’m guessing)
DirectX, Qt and that kind of stuff. But we already have other languages that
does this well, so I doubt that Go will ever become a strong contender in these
areas. Go is "cloud-native", if that expression means anything at all.

Go is also a simple, fun and extremely capable language - I encourage you to
check it out! And don’t get intimidated by the lack of classes. Go does OO
differently - and, in my opinion, a lot better - than the classic (and intricately involved) approach to OO, but it might require a little effort to wrap one’s head around the
conceptual differences.

*Update: I noticed [this answer](https://www.quora.com/Other-than-Google-what-companies-are-using-Go-in-production/answer/Ayush-Jain-1?ch=10&share=0f830a9d&srid=5Wbp) which points out two games - Farmville: Harvest Swap
and Dawn of Titans - that are both developed in Go, so I guess the language is
making strides in that area as well!
