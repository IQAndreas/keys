---
layout: slate
title: My PGP (or GPG) and SSH Keys
---

{%comment%}{% raw %}
<nav id="menu" class="floating-menu left">
	<h3>Contents</h3>
    <ul>
        <li><a href="#pgp">PGP (or GnuPG)</a></li>
        <li><a href="#pgp-fingerprint">Fingerprint</a></li>
        <li><a href="#pgp-automatic-download">Automatic Download</a></li>
        <li><a href="#pgp-manual-download">Manual Download</a></li>
        <li><a href="#SSH">View source and report issues</a></li>
    </ul>
</nav>
{% endraw %}{%endcomment%}

## <a id="pgp"></a>PGP (or GnuPG)

This is my PGP (also called GPG or GnuPGP) key that is used for encrypting email and other sensitive data, or checking if the text in an email I have sent you has been modified or tampered with. If you are unfamiliar with GPG but would still like to send me encrypted messages, see [_Details regarding GPG (or PGP): New to GPG?_](/keys/gpg/#new-to-gpg).

### <a id="pgp-fingerprint"></a>Fingerprint

See also [_Details regarding GPG (or PGP): Verifying fingerprints_](/keys/gpg/#verifying-fingerprints)

```
Fingerprint:	E82F 46DD 8613 3D80 FDB8 A797 0E20 7194 8BBB 5F64
Long Key ID:	                              0E20 7194 8BBB 5F64  (0x0E2071948BBB5F64)
Short Key ID:	                                        8BBB 5F64  (0x8BBB5F64)
```

### <a id="pgp-automatic-download"></a>Automatic Download

Run the following command to automatically fetch the latest version from the keyserver:

```
$ gpg --keyserver pool.sks-keyservers.net --recv-key E82F46DD86133D80FDB8A7970E2071948BBB5F64
```

### <a id="pgp-manual-download"></a>Manual Download

You can manually retrieve the keys using `wget`, _"Save as..."_ in your browser, or opening the ASCII armored version and copying the text to your clipboard.

There is also a "minimal version" of the key containing the absolute bare-bones version without any non-essential signagures or additional data such as a photo IDs. Due to the exclusion of signatures, the minimal key is not recommended if you are using GPG in conjunction with a "web of trust" system. As most computers today won't bat an eyelash at an additional 100kb of data, the minimum version of the key is seldom necessary, but has been included for edge cases where it is necessary.

**Full Download:** \[ [ASCII](/keys/gpg/iqandreas-8BBB5F64.asc) \] \[ [binary](/keys/gpg/iqandreas-8BBB5F64.gpg) \]

**Minimal Download:** \[ [ASCII](/keys/gpg/iqandreas-minimal-8BBB5F64.asc) \] \[ [binary](/keys/gpg/iqandreas-minimal-8BBB5F64.gpg) \]


## <a id="ssh"></a>SSH

This is my SSH key that can be used for granting me access into remote servers. For both of our security, please setup your SSH server to use public key authentication instead of password authentication. This is also the key used for GIT authentication.

If you would like a verification of the fingerprint, use the same procedure as [verification of my GPG fingerprint](/keys/gpg/#verifying-fingerprints), but with the fingerprint listed below instead.

**Fingerprint:** `a9:a0:a9:9a:7e:a2:65:0b:5d:f5:d9:83:d9:85:fd:da`

**Download:** [`iqandreas-ssh-4096r.pub`](/keys/ssh/iqandreas-ssh-4096r.pub)

