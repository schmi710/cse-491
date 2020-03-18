---
layout: post
title: "std::bitset plus -msse4.2 equals popcnt"
date: 2019-11-20
author: Jamie Schmidt
---



(after quite a lot of revision, I decided to go for code that can be parallelized using the c++17 algorithms, because any alternative just took far, far too long)

Introduce and explain general concepts and limitations of parallelizing code. Include some statistics about the c++17 parallel algorithms.

List the c++17 parallel algorithms and describe what they do, if it's complex.

Give an example problem of a relatively complex, multifaceted algorithm.

Replace blocks of the code with the c++17 parallel algorithms.

Demonstrate the primary maxim of parallelization, that being putting all parallel code together by restructuring the code.

Properly parallelize parallel sections which can happen concurrently using pthreads.

Using pthreads, parallelize serial sections which can happen concurrently.

Note that, at this point, a race condition occurs.

Give a way to fix this by being efficient and using blocking, and show that this is very slow.

Give a way to fix this by being less efficient, and show that this is faster.
