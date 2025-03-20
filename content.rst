Go Programming Language 
########################

:Date: 03/19/2025 

Intro
*******

**Context & Purpose**

I am exploring new way to build microservices architecture product as part 
of x as Code for documentation and diagramming as code. I want performance 
and easy to use tool. So I started looking into Go and Rust. This is where 
I document my progress, notes, courses, and tricks to accomplish certain 
programmatic patterns in `Go`_. This doc will serve as a roadmap for what 
works for me.

**What is Go**

Go, Golang 

* is a high-level general purpose programming language that is statically typed 
  and compiled.

  * *statically typed* -> a variable's date type is known and checked at compile 
    time and not at run-time like Python or Javascript.
  
  * *compiled* means Go is a compiled language i.e the source code is translated
    into machine code by a compiler before execution.
    
    * Examples of pure compiled languages are C, C++, Erlang, Haskell, Rust, 
      and Go.

.. card:: Go Features 

   * Go was created at Google as an alternative of C++ with with the following goals in mind: 
     
     1. scalability (easy onboarding developer, scale up team, scale up services)
     2. made with a limited feature set and designed for faster compilation.
        
        * Simple syntax - easy to use.

        * fast source code compilation (developer time), rather than optimum
          runtime speed.

     3. concurrency 
   
   [1]_ 
   Problem: An increasing number of Google users were accessing google search servers, and 
   Google was having a hard time keeping up the pace. Scaling new server in 
   C++ or Java to keep up with demands was tedious and took hours to compile.
     
   * Go emphasizes ease of use and low memory overhead.

   **Go Features** [1]_

   * **Concurrency.** Hands down, the best feature of Go is its advanced 
     scalability and concurrency features. Go is designed to be lightweight 
     and to take advantage of *Goroutines* and channels to create sleek, 
     responsive streaming services and web applications. 
   * **Simple syntax.** One of the best features of Go is one most people will 
     notice immediately—it is surprisingly simple to read. This reduces 
     developer ramp-up time and the time required to maintain the software.
   * **Cross-platform support.** Go can be used anywhere it needs to be, 
     whether it is Linux, Mac or Windows. This is as opposed to other languages 
     like Swift, PowerShell, or Visual-Basic. These languages are pretty much 
     restricted to their respective architecture.
   
   other features: 

   * **Garbage collection**: Go feature garbage collection, and automatic memory 
     management. [2]_

     .. warning:: garbage collection, with its performance overhead and 
        stop-the-world pauses, can make programs behave unpredictably at run-time, 
        and some people find this inconsistency unacceptable.

        Languages (such as Rust) where the programmer must take explicit 
        responsibility for allocating and freeing every byte of memory, are better 
        for real-time or ultra-high-performance applications.

.. card:: Go Use Cases [1]_

   * **Web servers:** One of the great features of Go is that it has a built-in 
     library solely for HTTP interactions. Combine this with its hallmark 
     concurrency and lightweight framework, and you have the perfect language 
     for writing a backend server.

   * **ETL (Extract, Transform, Load):** An ETL application takes data from 
     several existing sources and loads them into a central data lake for 
     analysis. This operation will handle billions of records potentially. 
     The use of channels and Goroutines make this the perfect project to tackle 
     using Go.

   * **System Utilities:** Go is a great language for low-level manipulation. 
     For example, if your organization needs to write a command-line interface 
     to analyze network traffic, build code scaffolding, or more, Go is the 
     way to go. There is already plenty of precedent for doing so, such as 
     GoTTY, ngRok, and Caddy, all of which are CLI’s written in Go.

.. card:: Why and When to use Go? [1]_

   Go is a programming language developed by Google to be 
   simple to use and highly scalable. Go is perfect 
   
   1. for creating backend servers, 
   #. ETL operation, 
   #. system utilities, 
   #. Web services, API,
   #. Distributed systems 
   #. and more. 
   
   The rule of thumb is this: If you expect your app to need a great 
   deal of data processing, string manipulation, concurrency, 
   or all of the above, go with Go.

   * For large projects and rapid development cycles, (onboard junior dev) 
     go with Go due its fast compilation times.


**Roadmap**

.. uml::

   @startmindmap
   * Golang Roadmap
   ** Download Go
   ** Get Started
   *** New to coding (Eduruka)
   *** Go by Example
   *** Go Standard Library
   *** Explore Advanced Topics \n \
   by Creating or exploring more projects
   **** CLI in Go \n ex. docker/cli
   **** Web Dev in Go
   **** microservices in Go

   @endmindmap


1. Head over to the `Go`_ website.
#. `Download Go <https://go.dev/doc/install>`_ by following the installation 
   process from the go website.

#. Once Go is installed on your host machine, head to the 
   `Go learning page <https://go.dev/learn/>`_
   
   .. image:: ./_images/GO-001.0_GolangIntro_1.0_LearnPage.png
      :width: 500px
      :alt: Go learn page

   I. To get familiar with the language, I found the 
      `New to coding? <https://www.youtube.com/watch?v=Q0sKAMal4WQ>`_ card
      as a very useful quick tutorial.

      * Start with this. Take notes and summarize the video.
   
   #. Then Reinforce the learning, Golang syntax by seeing more advance examples
      using this curated `Go by Example`_ site.
   
   #. Checkout the `Go Standard Library`_ to see built-in features offered by the
      language
   #. Explore more advanced topics such as Go CLI and Go Web dev.
       

.. only:: personal

   Journal and Log
   *****************

   .. toctree::
      :caption: Journal
      :glob:
      :numbered:
      :maxdepth: 1

      _Logs_Journal/JNL-*

Courses 
*********

.. toctree::
    :caption: Journal
    :glob:
    :numbered:
    :maxdepth: 1

    Courses/CourseName_git/content

.. [1] `Go vs Python`_ 
.. [2] `Go vs Rust`_

.. include:: ./relevant_urls.rst