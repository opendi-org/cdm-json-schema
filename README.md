# (DRAFT) OpenDI Causal Decision Model JSON Schema

Source files defining the OpenDI Causal Decision Model data structure, as a JSON Schema.

## How to use

If you plan to include the OpenDI JSON Schema in the source files for your own project, include this repository as a [Git Submodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules).

Follow the above instructions to add the submodule to some subdirectory within your project.  
**NOTE:** For stricter environments, files like `LICENSE` and `README.md` may cause issues. In these cases, after adding the submodule, edit the entry for this submodule in `.gitmodules` to add `branch = main-sourceonly` or `branch = dev-sourceonly`. These branches exclude `LICENSE`, `README.md`, and `test-data.json`. 

Including these schemas as a submodule allows you to reference them directly in the `$schema` property at the top of a `.json` data file.

**The main schema to reference is `Causal-Decision-Model.json`.**  
This schema includes relative file references to most of the other schema files in this repo.

See [test-data.json](./test-data.json) for an example of this.

## Projects that use these schemas:

- [OpenDI Api Specification](https://github.com/opendi-org/api-specification)
- [CDD Authoring Tool](https://github.com/opendi-org/cdd-authoring-tool)
