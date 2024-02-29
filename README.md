# Rebel Build Action

Github Action for building Rebel Engine.

This Action provides a standardised way for building Rebel Engine and Rebel Editor. It uses [`actions/upload-artifact@v4`](https://github.com/actions/upload-artifact) to allow the executable or library that is built to be downloaded as an artifact.

## Usage

```
- uses: RebelToolbox/RebelBuildAction@v3
  with:
    # Name of the artifact to be uploaded
    artifact:
    
    # SCons build options
    build-options:
    
    # Use a build cache to make subsequent builds faster
    # Type: boolean
    # Default: true
    use-build-cache: true

    # Filename of the binary that will be built
    rebel-executable:
```
