## CLI Reference

- Serve - `perla serve`

  Starts a development server for modern Javascript development

  - Auto Start - `perla serve -a false`, `perla serve --auto-start`

    Starts the server without action required by the user.

  - Port - `perla serve -p 8080`, `perla serve --port 8080`

    Select the server port, defaults to 7331

  - Host - `perla serve -h 0.0.0.0`, `perla serve --host 0.0.0.0`

    Server host, defaults to localhost

  - Use SSL - `perla serve -s true`, `perla serve --use-ssl true`

    Forces the requests to go through HTTPS. Defaults to false

- Build - `perla build`

  - Index File - `perla build -i start.html`, `perla build --index start.html`

    The Entry File for the web application. Defaults to index.html

  - Esbuild Version - `perla build -ev 0.13.1`, `perla build --esbuild-version 0.13.1`

    Use a specific esbuild version

  - Out Dir - `perla build -o ./public`, `perla build --out-dir ./public`

    Where to output the files. Defaults to ./dist

- Init - `perla init`

  Creates basic files and directories to start using perla.

  - Path - `perla init -p ./client`, `perla init --path ./client`

    Where to write the config file

  - With Fable - `perla init --wf true`, `perla init --with-fable true`

    Include fable options in the config file

- Search - `perla search`

  Searches a package in the skypack API.

  - Name - `perla -n lodash`, `perla --name lodash`

    The name of the package to search for.

  - Page - `perla -p 2`, `perla --page 2`

    Page number to search at.

- Show - `perla show`

  Gets the skypack information about a package.

  - Package - `perla -p lodash`, `perla show --package lodash`

    The name of the package to show information about.

- Add - `perla add`

  Generates an entry in the import map.

  - Package - `perla add -p react`, `perla add --package react`

    The name of the package to show information about.

  - Alias - `perla add -p react@16 -a react-sixteen`, `perla add -p react@16 --alias react-sixteen`

    Specifier for this particular module.

  - Source - `perla add -p react -s jspm`, `perla add -p react --source jspm`

    The name of the source you want to install a package from. e.g. unpkg or skypack. Available options:

    - `jspm`
    - `unpkg`

- Remove - `perla remove`

  Removes an entry in the import map.

  - Package - `perla remove -p react-sixteen`, `perla remvoe --package react-sixteen`

    The name of the package to remove from the import map this can also be aliased name.

- List - `perla list`

  List entries in the import map.

  - As Package Json - `perla list --as-package-json`

  List packages in npm's package.json format.

- Version - `perla version`

  Prints out the cli version to the console.
