# OSSU Website

An experimental unofficial static website for the [OSSU](https://github.com/ossu).

# Table of contents

- [Installation](#installation)
- [Usage](#usage)
- [Development](#development)
- [Contribute](#contribute)
- [License](#license)

# Installation
[(Back to top)](#table-of-contents)

To use this project:

1. install the **extended** version of [hugo](https://gohugo.io/getting-started/installing/)

2. clone the repo using the command:

```
git clone https://github.com/AshineFoster/ossu.git
```

3. change present working directory:

```
cd ossu
```

4. clone submodules:

```
git submodule update --init --recursive
```

# Usage
[(Back to top)](#table-of-contents)

In order to view the built website, run the following command from the project root folder:

```
hugo server
```

This will show you a link that you can open to view the website.

# Development
[(Back to top)](#table-of-contents)

[Hugo Documentation](https://gohugo.io/documentation/) pages contain information about hugo projects.

The git submodule located at `./content/ossu/` contains a modified version of the OSSU 
[computer science](https://github.com/AshineFoster/computer-science) repository.

The theme's git submodule for the website is located at `./themes/compose/`. Its relevant
documentation is avaliable at [Compose docs](https://docs.neuralvibes.com/).

# Contribute
[(Back to top)](#table-of-contents)

All contributions are welcome.

# License
[(Back to top)](#table-of-contents)

A copy of the license file can be found at `./LICENSE` or online at [Apache License](http://www.apache.org/licenses/).
