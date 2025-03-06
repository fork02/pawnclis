Usage Instructions
==================

1. Renaming Your Files
----------------------
Before proceeding, rename your `*.pwn` files to one of the following formats:

- `*.io.pwn`
- `*.io.p`
- Or any other preferred variation.

2. Compiling with `paw`
-----------------------
To compile using the default settings, run the following command:

.. code-block:: sh

    paw -c

3. Preparing the Configuration File (`data.json`)
-------------------------------------------------
Before compiling, ensure that a `data.json` file exists in the `pawnclis` directory.
This file should contain the necessary configuration settings. Below is an example of its structure:

.. code-block:: json

    {
        "amx_opt": "-d2 -Z+",
        "allow_subdir": "/pawno/include",

        "ppm_dir": "pawno",
        "ppm_subdir": "include",
        "ppm_type": "urllib3",

        "chatbot_token": "",
        "chatbot_model": "",
        "chatbot_biodata": "",
        "chatbot_json_get": ""
    }

Configuration Details
---------------------
- **`amx_opt`**: Compilation optimization options (e.g., `-d0` for debugging).
- **`allow_subdir`**: Defines the allowed subdirectory path for includes.
- **`ppm_dir`** & **`ppm_subdir`**: Specifies the directory structure for package management.
- **`ppm_type`**: Determines the package manager type (e.g., `urllib3`).
- **`chatbot_token`**, **`chatbot_model`**, **`chatbot_biodata`**, **`chatbot_json_get`**: Reserved fields for AI-related `Groq.com <https://groq.com/>`_ configurations.

Make sure this file is properly configured before running the compilation process.

