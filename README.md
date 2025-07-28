# MuddyPuddles
MuddyPuddles is designed to work with Gentoo to help find early issues with how new toolchains will work with Gentoo's stage3 tarballs.
After many years of manually creating a chroot to enable new toolchain versions to look for early bugs, I decided it was time to script something up for my needs as nothing else quite fit the bill.

# Features
 - Prepare a chroot to us the system's Portage repo directory
 - Copy over the correct `qemu-user` binary to test different arches to the host
 - Unmask the latest GCC version (Currently hardcoded to GCC-16)
 - Verify the chroot works with a quick toolchain and package test

# TODO
 - Enable test suites on all packages that support them in @system and @world per chroot need
 - Add more packages to an existing chroot as needed.
 - Finish automation script
 - Send logs via email with quick glance pass or failure

# Why the name
Everybody loves jumping in muddy puddles! Think this project as adding more water (packages) to your puddle (chroot) to have even more fun sploshing about in your muddy puddle.
Yes, Peppa Pig has ruined my life at this point.
