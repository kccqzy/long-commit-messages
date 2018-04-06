# Long Commit Messages

This is a experimental repo to see what would happen if the commit messages
are exceptionally long.

It is my understanding that Git internally uses `size_t` for the commit
messages, which means the maximum length is platform-dependent.

It would be interesting to see what would happen when the length exceeds
`~(size_t)0`, or 4294967295 bytes in 32-bit platforms. But my guess is that
before we reach that length, many things would have already stopped
working.
