# libarchives

Using DSpace for archiving metadata.

## Clone of DSpace

The archive of metadata uses [DSpace running on Docker](https://wiki.lyrasis.org/display/DSPACE/Try+out+DSpace+8#TryoutDSpace8-InstallviaDocker). We forked the original DSpace repository before cloning it.

## Configuration

### Admin user

Creating a _admin_ user `mgarcia@test.edu:`

```
docker compose -p d8 -f docker/cli.yml run --rm dspace-cli create-administrator -e mgarcia@test.edu -f Marcelo -l Garcia -p admin -c en
```

Where:

* `-f` is first name,
* `-l` is last name,
* `-p` is the password.
