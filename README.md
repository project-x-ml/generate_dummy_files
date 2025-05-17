# generate_dummy_files
generate dummy data for various MIME types for testing purposes

## Usage

The `generate_dummy_files.py` script allows you to generate dummy files for various MIME types.

### Arguments

- `--mime-types` or `-m`: Comma-separated list of MIME types to generate files for.  
    Example: `--mime-types text/plain,image/png`
- `--output-dir` or `-o`: Directory where the generated files will be saved.  
    Example: `--output-dir ./dummy_files`
- `--count` or `-c`: Number of files to generate for each MIME type.  
    Example: `--count 5`
- `--size` or `-s`: Size (in bytes) of each generated file.  
    Example: `--size 1024`

### Example

```bash
python3 generate_dummy_files.py --mime-types text/plain,image/png --output-dir ./dummy_files --count 3 --size 2048
```

This command generates 3 dummy files for each specified MIME type, each with a size of 2048 bytes, and saves them in the `./dummy_files` directory.

Refer to [MDN Common MIME types](https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/MIME_types/Common_types) and update the `CUSTOM_MIME_HANDLERS` list in the script for new MIME types as needed.
