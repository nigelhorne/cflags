Early stages of development, many architectures are not yet supported.

If you see "Can't locate Sys/Info.pm in @INC",
you'll need to grab and install Sys::Info from your favourite repository:

    cpan -i Sys::Info

On FreeBSD you can run:

    sudo pkg install p5-sys-info

Put this into your .bash_profile:

    export CFLAGS=$(src/cflags/cflags)

Note that on some systems CFLAGS will include -mfloat-abi=hard,
which you'll also need to add to LDFLAGS.
