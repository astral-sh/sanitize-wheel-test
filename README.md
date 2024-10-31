# sanitize-wheel-test

A test distribution to validate filename sanitization during wheel extraction.

Created as follows:

```shell
touch payload
uv init payload-package
cd payload-package
uv build
cd dist/
zip payload_package-0.1.0-py3-none-any.whl ../../payload
```

See: https://github.com/astral-sh/uv/issues/8731.
