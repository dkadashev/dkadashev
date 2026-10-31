# Dimitri Kadashev

Backend and systems software engineer with over 18 years of production experience, mostly C/C++ and Python on Linux, and 15 years as a tech lead for teams of 4-6. I like performance work, fault-tolerant systems, and the kind of problems that only show up in production.

## Open source

**Linux kernel: io_uring support for `mkdirat`, `symlinkat` and `linkat`**\
An 11-patch series, including refactoring of the path-handling code in `fs/namei.c` so that the new operations could share it. Accepted upstream in 2021 after nine revisions of review with the maintainers (authored as Dmitry Kadashev).
- [Patch series (v9 cover letter)](https://lore.kernel.org/io-uring/20210708063447.3556403-1-dkadashev@gmail.com/)
- [Merged commit: `io_uring: add support for IORING_OP_MKDIRAT`](https://github.com/torvalds/linux/commit/e34a02dc40c95d126bb6486dcf802bbb8d1624a0)

**Rust compiler: type parameter names in type-mismatch errors**\
Type-mismatch errors now show the name and definition of the type parameter involved. Merged in 2019.
- [rust-lang/rust#66014](https://github.com/rust-lang/rust/pull/66014)

## Selected professional work

This work was closed source, so there is no code to link to.

- **HTTP proxy rewrite (C++):** led the rewrite of a high-load transparent caching proxy deployed as appliances at ISP sites. The new modular architecture, built around event loops, multithreading, custom memory allocation and state-machine-based protocol parsing, ran in production for 8+ years and was 3-10x faster than its predecessor.
- **Disk I/O back-end:** a new back-end for the proxy with 2-3x lower latency, which is what led to the kernel patches above.
- **CDN back-end rewrite (Python):** cut average response time 11x and daily traffic by 93%, and eliminated request timeouts.
- **Object storage:** led a Ceph-based service to replace a Gluster-based one; in synthetic tests, listing requests that took minutes on the old system completed in seconds.

## Tech

C++, C, Python, Rust · Linux, networking, io_uring · distributed and fault-tolerant systems · performance and profiling

## Contact

[LinkedIn](https://www.linkedin.com/in/dkadashev/)
