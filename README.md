# BEAM
## documentation
- [hello world](https://beam.apache.org/get-started/quickstart-py/)

## example repository
- [examples](https://github.com/apache/beam/tree/master/sdks/python/apache_beam/examples)
```bash
#cd beam/sdks/python/apache_beam/examples/;

mkdir tests;
wget "https://storage.cloud.google.com/apache-beam-samples/shakespeare/hamlet.txt" tests;

# execute
python -m apache_beam.examples.wordcount --input tests/hamlet.txt --output tests/hamlet.txt.out;
```


## Install env
```bash
python3.7.2 -m virtualenv venv;
source venv/bin/activate;
sudo chmod -R 755 .;
sudo chown -R developer:developer .;
python -m pip install apache-beam;
python -m pip install --upgrade timezonefinder==3.0.0 pytz 'apache-beam[gcp]';
python -m pip install apache-beam[test];
python -m pip install apache-beam[docs];
```
