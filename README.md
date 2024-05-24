# HTTP2 Secure Edition

Some environments are disabling all AES-128 bit ciphers for, security reasons.
This package aims to provide those specific environments the ability to
continue using the latest technologies (HTTP2) while still providing a level of
configuration ability to the administrator.

As this package aims to be an exact stand-in-replacement for the official Go
net/http2 package, but with additional security bindings to allow stronger
ciphers, one can use this as a stop-gap measure to provide more secure options
to system administrators.  When the RFC-9113 is amended to allow the ability to
turn off AES-128 cipher, this package may be reverted back to the official Go
package.  Meanwhile, this package provides a way to get higher than AES-128 bit
ciphers.
