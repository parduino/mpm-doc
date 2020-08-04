# Run MPM

The CB-Geo MPM code uses `JSON` file type for input configuration.

## Usage {docsify-ignore}
```shell
   ./mpm  [-p <tbb_parallel>] [-i <input_file>] -f <working_dir> [--]
          [--version] [-h]
```

arguments listed within `[]` are optional

Where:
```shell
   -p <tbb_parallel>,  --tbb_parallel <tbb_parallel>
     Number of parallel TBB threads

   -i <input_file>,  --input_file <input_file>
     Input JSON file [mpm.json]

   -f <working_dir>,  --working_dir <working_dir>
     (required)  Current working folder

   --,  --ignore_rest
     Ignores the rest of the labeled arguments following this flag.

   --version
     Displays version information and exits.

   -h,  --help
     Displays usage information and exits.
```


For example:

```
./mpm -f /path/to/input-dir/ -i mpm-usf-3d.json -p 8
```
