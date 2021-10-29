# Turbo Button

It's like the early 90s again, but for modern Linux machines.

## Background

In the dawn of the Personal Computer revolution, programs were written
with the clock speed in mind. As processors got faster, these programs
didn't function the same. The solution was the "turbo" button, which
ironically, was often wired such that when the button was pressed, the
CPU ran _slower_.

Modern CPUs have performance scaling for different
situations. Typically, this is probably something like "performance"
or "powersave." In some ways, "performance" is "turbo" mode. So, that's
what this is. A turbo button. For Linux. 

This button doesn't attempt to work for all CPUs and all configurations.
It literally just writes the values "performance" or "powersave" to
`/sys/devices/system/cpu/cpuN/cpufreq/scaling_governor` and fails otherwise.
If you're system doesn't support this on Linux, then, well, submit a PR,
I guess?

## Copyright

Copyright 2021 Andrew Gwozdziewycz, except for the button images,
which I found
[here](https://ux.stackexchange.com/questions/43250/is-there-a-better-way-to-design-switches-than-i-o). If
that's a problem, then by all means, let me know, and I'll replace them.
