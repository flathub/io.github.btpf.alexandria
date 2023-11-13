## Instructions:
### Update (If no dependencies changed)
0. Clone Project
    ```
    git clone https://github.com/flathub/io.github.btpf.alexandria
    ```
1. Create local branch of main
2. update metainfo.xml with changelog and alexandria.yml with new commit hash

### Update Dependencies
Note: Make sure these commands are run from linux

0. Clone Project
    ```
    git clone https://github.com/flatpak/flatpak-builder-tools
    ```
1. Generate Node Sources (generated-node-sources.json)
Install the flatpake-node-generator: https://github.com/flatpak/flatpak-builder-tools/tree/master/node
    ```
    flatpak-node-generator npm <path to package-lock.json>
    ```
2. Generate Cargo Sources (generated-cargo-sources.json)
Navigate To: https://github.com/flatpak/flatpak-builder-tools/blob/master/cargo/flatpak-cargo-generator.py
    ```
    flatpak-cargo-generator.py src-tauri/Cargo.lock
    ```

