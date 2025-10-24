# eBPF Syscall Tracer using bpftrace

This project demonstrates a simple eBPF program written in bpftrace to trace `open` and `close` syscalls and measure their frequency.

## How It Works
- Traces `sys_enter_openat` and `sys_enter_close` tracepoints.
- Counts how many times each process opens and closes files.

## Example Command
```bash
sudo bpftrace trace.bt
