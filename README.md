# Get Conan GitHub Action

Gets the most recent Conan

**Works on**: Linux, Windows and MacOS 

## Inputs

No inputs

## Outputs

### `version`

The version string from "conan --version"

## Example usage

~~~~
    - name: Install Conan
      id: conan
      uses: turtlebrowser/get-conan@main

    - name: Conan version
      run: echo "${{ steps.conan.outputs.version }}"
~~~~
