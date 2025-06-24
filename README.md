# NXP Repo
NXP Package Manager Default repository.
Repo must have packages (`.nxp`) and `repoc.toml` file.
## How to create package?
First, create `PACKAGE NAME` directory. Then create 2 directories and meta file like this:
> #### Package name must be in lower-case
- `bin` - your binaries
- `scripts` - lua-scripts
- `meta.toml` - info about your package
`meta.toml` must contain `name`, `author`, `version` and `dep` options.
```toml
# meta.toml example
name="your awsome package" # Package name
version="1.0.0" # Package version
author="You" # Package author
dep=[] # Package dependencies (not working yet)
```
To build your package you have to download NXP Package Manager (not avaiable yet).
Then enter in your terminal `nxp -bp <folder with your package>`.
> #### You can add your folders and change installation with your lua-scripts!
