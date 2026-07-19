# subhook-direct

A fork of [subhook](https://github.com/Zeex/subhook) that patches code
by writing through `/proc/[pid]/mem` instead of touching memory
directly, so it can install hooks into pages you don't have direct
write access to (e.g. from a separate process context) without relying
on `mprotect`.

## License

BSD 2-Clause, same as upstream subhook. See [LICENSE](LICENSE).
Original work Copyright (c) 2012-2014 Zeex. Modifications Copyright (c) 2026 3443e.