# Repository of fuzzing targets for SideFuzz

See https://github.com/phayes/sidefuzz

## Adding a new target:

Create a new workspace member with a name in the format `<crate_name>_<function>_<input_name>`. For examle, to fuzz the `rsa` crate, checking to make sure the `encrypt` function is constant-time in relation to `message` input, create a new member called `rsa_encrypt_message`.
