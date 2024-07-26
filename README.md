 Rust Project Template
 =====================

This repository serves as a template for Rust projects, providing a structured starting point that encourages modular development and experimentation.

Purpose
-------

The purpose of this template is to streamline the setup process for new Rust projects while promoting best practices in software development. It includes a predefined folder structure and initial files tailored for Rust programming.

Folder Structure
----------------

```
project_root
├── sandbox/
│   ├── scripts/
│   │   └── create.sh
│   ├── README.md
│   └── (other components)
├── src/
│   └── main.rs
├── .gitignore
├── Cargo.toml
├── README.md
└── LICENSE
```

*   **sandbox/**: Contains experimental components and prototypes. It's recommended to keep each component in a separate folder (`component1/`, `component2/`, etc.) for better organization and clarity. Refer to [sandbox/README.md](./sandbox/README.md) for guidelines on using this folder effectively.
    
*   **src/**: Main source code directory where production-ready code is developed.
    

Getting Started
---------------

To use this template for a new Rust project:

1. Add the template:
    * **Using GitHub**: Click on the **"Use this template"** button to create a new repository based on this template.
    
    * **Using Git CLI**: Clone this repository using the command:
        ```
        gh repo create <your-project-name> --template IrregularCelery/template.rs --public
        ```

        >_useful tips:_
        >* Change `--public` to `--private` to create private repositories.
        >* Add `--clone` flag to clone your created repository right away.

3.  Change the default name:
    * In `Cargo.toml` file, change `name` and `default-run` under `[package]` to the name of your project.
    ```diff
    -name = "template-rs"
    +name = "<your-project-name>"
    ...
    -default-run = "template-rs"
    +default-run = "<your-project-name>"
    ```

3.  Customize the folder structure and files as per your project's requirements.
    
4.  Update this `README.md` file to provide specific details about your project, including installation instructions, usage guidelines, and any other relevant information.
    

About the Sandbox Folder
------------------------

The `sandbox/` folder is intended for developing and testing experimental components that may eventually be integrated into the main project (`src/`). These small projects are temporary and should be removed once integrated to reduce unused and duplicate code. Make sure to read the [sandbox/README.md](./sandbox/README.md) for detailed guidelines.

Why Use a Sandbox Folder?
-------------------------

### Difference from Branching

*   **Flexibility**: Unlike branching, which is typically used for features that will merge into a main branch, the `sandbox/` folder allows for more flexible experimentation and development. Components can be developed and tested independently and may end up in different parts of the main project.

### Benefits

*   **Modular Development**: Encourages modular development by isolating experimental components and prototypes.
    
*   **Reduced Clutter**: Helps maintain a clean main project directory by keeping temporary experiments separate until they are ready for integration.
    

### License

This project includes a [MIT License](./LICENSE) as a convenience. **You are not obligated to use this license**; feel free to replace it with your preferred license for your project.


