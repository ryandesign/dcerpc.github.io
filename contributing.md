---
title: Contributing
redirect_from: /contributing.html
---

## Reporting Bugs

If you find a bug or have an idea for an enhancement, please [file an issue on GitHub](https://github.com/dcerpc/dcerpc/issues).

## Projects

There are lots of interesting projects to work on in DCE/RPC. Here are some ideas:

* Clean up `dce_error_inq_text` to use `error_status_t` and
  `dce_error_string_t` parameters.
* Not all errors are in the message catalogue, e.g.
  `rpc_s_protseq_not_supported` is missing. Need to find and
  catalogue all errors.
* Fix the IDL compiler so that `[in]` reference parameters are
  declared with the const qualifier.
* Add support for `[out,unique]` parameters as used in the spoolss
  protocol.
* Add launchd (macOS) and systemd (Linux) support to rpcd.

### Projects specific to macOS

* Implement a `ncacn_mach` transport for local RPC on macOS.
* Add instant-off support to the RPC runtime.
* Replace the DCEThreads runtime with [libdispatch](https://github.com/apple/swift-corelibs-libdispatch).

## Contributing Code

We do not require copyright assignment, however we ask that you assert your rights to the code you contribute by [filing an issue on GitHub](https://github.com/dcerpc/dcerpc/issues) with your contribution.

If you are sending in modifications to existing DCE/RPC code, you
agree by submitting your modifications that the modifications are
licensed under the existing license terms of the files you are
modifying (i.e. BSD License). Please also add your copyright (name
and year) to the relevant files for modifications that include more
than 10 lines of code.

If you are submitting new files for inclusion in the DCE/RPC project
hosted here which are written by you (no code copied from another
source), you agree by submitting the files that your contributions
are licensed under the BSD License. Please include your copyright
(name and year) and the BSD License in your submitted files.

If you are not the author of the modifications, you agree to include
the original copyright notices and licensing terms with your
submission, to the extent that they exist. If there wasn't a copyright
notice or license in the original sources, please make a note of
it.

Generally, we can only take in contributions that are licensed under
the BSD License in order to maintain license compatibility within
the project. Contact us if you believe an exception is warranted,
prior to submitting the code.

## Licensing

DCE/RPC code and documentation contributions must be licensed under
the 3-clause BSD license below.

    Copyright (c) 2010 Apple Inc. All rights reserved.

    Redistribution and use in source and binary forms, with or without
    modification, are permitted provided that the following conditions
    are met:

    1.  Redistributions of source code must retain the above copyright
        notice, this list of conditions and the following disclaimer.
    2.  Redistributions in binary form must reproduce the above copyright
        notice, this list of conditions and the following disclaimer in the
        documentation and/or other materials provided with the distribution.
    3.  Neither the name of Apple Inc. ("Apple") nor the names of its
        contributors may be used to endorse or promote products derived from
        this software without specific prior written permission.

    THIS SOFTWARE IS PROVIDED BY APPLE AND ITS CONTRIBUTORS "AS IS" AND ANY
    EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
    WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
    DISCLAIMED. IN NO EVENT SHALL APPLE OR ITS CONTRIBUTORS BE LIABLE FOR ANY
    DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
    (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
    LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
    ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
    (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF
    THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
