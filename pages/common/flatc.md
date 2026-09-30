# flatc

> Compile FlatBuffers schemas and generate language-specific code.
> More information: <https://google.github.io/flatbuffers/flatbuffers_guide_using_schema_compiler.html>.

- Generate C++ headers for a schema:

`flatc --cpp -o {{path/to/output}} {{schema.fbs}}`

- Generate Python modules for a schema:

`flatc --python -o {{path/to/output}} {{schema.fbs}}`

- Generate code for several languages at once:

`flatc --cpp --rust -o {{path/to/output}} {{schema.fbs}}`

- Generate a JSON schema:

`flatc --jsonschema {{schema.fbs}}`

- Generate the binary schema:

`flatc --binary --schema -o {{path/to/output}} {{schema.fbs}}`

- Convert JSON data into a FlatBuffer:

`flatc --json --raw-binary -o {{path/to/output.bin}} {{schema.fbs}} -- {{path/to/data.json}}`

- Search for included schemas in an additional directory:

`flatc --include {{path/to/schemas}} -o {{path/to/output}} {{schema.fbs}}`

- Display the version number:

`flatc --version`
