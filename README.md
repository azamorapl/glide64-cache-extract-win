docker build -t gliden64_cache_extract:0.0.1 src

docker run --rm --volume="%CD%\mount:/textures" gliden64_cache_extract:0.0.1