# cxxlint

CxxLint is a Web-CAT plugin designed to integrate C++ static code style checking with CxxTest unit testing. This plugin is specifically designed for Web-CAT and ensures that students adhere to proper C++ coding style while submitting their homework assignments.

## Features
- **C++ Static Code Analysis**: Uses Google's `cpplint.py` to enforce C++ coding standards.
- **Unit Testing**: Integrates with CxxTest for automated unit testing of C++ code.
- **Web-CAT Integration**: Provides seamless integration with Web-CAT for automated grading.

## Prerequisites
To use this plugin, you will need:
- [Cxxtest](https://github.com/CxxTest/cxxtest) for unit testing.
- The `cxxtest` folder should be cloned into the `cxl` folder.
- Perl installed on your system (for executing the scripts).
- Python (for `cpplint.py`).

## Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/your-repository/cxxlint.git
   cd cxxlint
   ```
2. Install CxxTest:
   ```sh
   git clone https://github.com/CxxTest/cxxtest.git cxl/cxxtest
   ```
3. Ensure that `cpplint.py` is executable:
   ```sh
   chmod +x cpplint.py
   ```

## Usage
Run the linting and testing scripts as follows:

### Running the Style Check
To check C++ style compliance:
```sh
python cpplint.py [your_cpp_file.cpp]
```

### Running CxxTest
To run the CxxTest unit tests:
```sh
perl execute.pl
```

## License
This project is licensed under the terms specified in the `LICENSE` file.
