![CI](https://github.com/turtlebrowser/get-conan/workflows/CI/badge.svg)
# Get Conan GitHub Action

Gets the most recent Conan

**Works on**: Linux, Windows and MacOS

## Inputs

No inputs

## Outputs

### `version`

The version string from "conan --version"

## Example usage

To install the latest conan version

~~~~
    - name: Install Conan
      id: conan
      uses: turtlebrowser/get-conan@main

    - name: Conan version
      run: echo "${{ steps.conan.outputs.version }}"
~~~~

It is also possible to specify the wanted conan version, by using the with:/version input to the action.

~~~~
    - name: Install Conan
      id: conan
      uses: turtlebrowser/get-conan@main
      with:
        version: 1.50.0

    - name: Conan version
      run: echo "${{ steps.conan.outputs.version }}"
~~~~
