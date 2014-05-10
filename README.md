# sesscrypt

**Session information encryption/decryption tool.**

This small tool provides ability to securely encrypt/decrypt session information
using AES encryption with 16, 32 or 64 byte-long keys.

## Getting started

Start from setting up the stack, then configure and run the app.

### Stack

1. Install Python interpreter and PIP package manager.

### Application

1. Clone the repo:

        $ git clone git@github.com:flipcomp/sesscrypto.git

2. Create your virtualenv:

        $ virtualenv .virtual

   Then enter it (you'll have to repeat this one every time you come back
   to development)

        $ source .virtual/bin/activate

   To leave virtual environment run:

        (.virtual)$ deactivate

3. Install requirements:

        (.virtual)$ ./scripts/requirements

4. Run tests:

        (.virtual)$ ./scripts/test

5. Encrypt something:

        (.virtual)$ bin/sesscrypt enc -k sess.key 1
        1HjqIVb2qIx+xImXzhAYm4eDGvxFuw969RfGfBmt0WCHgxr8RbsPevUXxnwZrdFgh4Ma/EW7D3r1F8Z8Ga3RYA==

6. Then decrypt it:

        (.virtual)$ bin/sesscrypt dec -k sess.key 1HjqIVb2qIx+xImXzhAYm4eDGvxFuw969RfGfBmt0WCHgxr8RbsPevUXxnwZrdFgh4Ma/EW7D3r1F8Z8Ga3RYA==
        1

5. You can install the app globally with:

        $ PREFIX=/usr ./scripts/install

## Encryption/decryption process

TODO: ...

## Contributing

1. Work on your changes in a feature branch.
2. Make sure that tests are passing.
3. Send a pull request.
4. Wait for feedback.
