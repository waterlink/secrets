# secrets

Simple bash script to manage your secrets with symmetric key.

Uses `openssl` under the hood.

## Installation

Install it with:

```bash
mkdir -p bin
curl -L https://github.com/waterlink/secrets/raw/master/secrets > bin/secrets
chmod a+x bin/secrets
```

## Usage

### Generate yourself a key

```bash
bin/secrets gen-key mykey
```

### Encrypt file

```bash
bin/secrets enc file.txt file.enc mykey
```

### Decrypt file

```bash
bin/secrets dec file.enc file.txt mykey
```

### Edit encrypted file

```bash
bin/secrets edit file.enc mykey
```

### Source secret file with environment variables and run command

```bash
bin/secrets source file.enc mykey my-super-app --debug
```

## Contributing

1. Fork it ( https://github.com/waterlink/secrets/fork )
1. Create your feature branch (git checkout -b my-new-feature)
1. Commit your changes (git commit -am 'Add some feature')
1. Push to the branch (git push origin my-new-feature)
1. Create a new Pull Request

## Contributors

* [waterlink](https://github.com/waterlink) Oleksii Fedorov - creator, maintainer
