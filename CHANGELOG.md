# Change Log

## v4.0

  - Return the Rebel build filename as the `build-filename` output (https://github.com/RebelToolbox/RebelBuildAction/pull/7)

    In v3.0 and earlier, Rebel Build Action required you to know the build filename, and pass it as the `rebel-executable` input.
    This filename needed to be correct, because it was used to specify the file to be uploaded as the artifact.
    Now, Rebel Build Action will determine the main build filename and return it as the `build-filename` output.
    Furthermore, Rebel Build Action will include all the build files in the artifact.

    ⚠️ This is a breaking change.
    It will require uses of Rebel Build Action to be updated to no longer specify the `rebel-executable` input.

## v3.0

  - Remove support for 32-bit Linux builds (https://github.com/RebelToolbox/RebelBuildAction/pull/6)

    32-bit hardware is no longer being produced.
    Although there are still Linux distributions that still support 32-bit hardware, most distributions are phasing out that support.
    Rebel Engine release versions are built on Ubuntu.
    Ubuntu 18.04 LTS was the last version that supported 32-bits.
    Ubuntu 18.04 was a long-term support version that was supported for five years, but that support ended in May 2023.
    Therefore, Rebel Toolbox has decide to no longer support 32-bit Linux.

## v2.1.2

  - Update Rebel Build Action tests to use the new platform names (https://github.com/RebelToolbox/RebelBuildAction/pull/5)

## v2.1.1

  - On macOS, use Python to install SCons (https://github.com/RebelToolbox/RebelBuildAction/pull/4)

## v2.1

  - Include building on Windows and macOS platforms (https://github.com/RebelToolbox/RebelBuildAction/pull/3)

## v2.0

  - Update GitHub Actions (https://github.com/RebelToolbox/RebelBuildAction/pull/2)

## v1

  - Initial version
