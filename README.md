# go-benchmark
Benchmark tests in Go

# Run
1. `go test -bench`
2. `go test -bench -benchtime 10s` (great for end-to-end testing)

# Profiling

1. `go test -benchmem` (memory allocation statistics)

2. `go test -trace {trace.out}` (record execution trace for analysis)

3. `go test -{type} profile {file}` (generate profile of requested type)
    (e.g. block, cover, cpu, mem, mutex)

4. Example `go test -bench 512 -benchmem`

5. Tools `go tool pprof`

6. Run `go test -bench Alloc -memprofile profile.out` -> `go tool pprof profile.out`--> `svg` (Install Graphwiz from `graphwiz.org/download` !)




    