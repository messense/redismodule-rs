[![license](https://img.shields.io/github/license/RedisLabsModules/redismodule-rs.svg)](https://github.com/RedisLabsModules/redismodule-rs/blob/master/LICENSE)
[![GitHub issues](https://img.shields.io/github/release/RedisLabsModules/redismodule-rs.svg)](https://github.com/RedisLabsModules/redismodule-rs/releases/latest)
[![Rust](https://github.com/RedisLabsModules/redismodule-rs/workflows/Rust/badge.svg)](https://github.com/RedisLabsModules/redismodule-rs/actions?query=workflow%3ARust)
[![CircleCI](https://circleci.com/gh/RedisLabsModules/redismodule-rs/tree/master.svg?style=svg)](https://circleci.com/gh/RedisLabsModules/redismodule-rs/tree/master)

# redismodule-rs

The Rust API for Redis Modules API is based on the https://github.com/brandur/redis-cell project.

# Running the example module
1. install [rust and cargo](https://www.rust-lang.org/tools/install) 
2. install redis [(mac)](https://gist.github.com/tomysmile/1b8a321e7c58499ef9f9441b2faa0aa8)
3. run `cargo build --example hello`
4. start a redis server with the hello module 
   * Linux: `redis-server --loadmodule ./target/debug/examples/libhello.so`
   * Mac: `redis-server --loadmodule ./target/debug/examples/libhello.dylib`	
5. open a redis cli. and run `HELLO.MUL 31 11`. 
