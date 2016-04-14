# dckrm

Command Line tools for removing docker containers and images.

* dckrm - Remove Docker Containers
* dckrmi - Remove Docker Images

## Dependencies

* docker
* vim

## Install

Deploy these scripts in $PATH directory.


## How to Use

### dckrm

Execute the command

```
$ dckrm
```

The output of commands `docker ps` is written in the temporary file `/tmp/dckrm-%Y%m%d%H%M%s` 
and it is opened with vim.

Delete or Comment out (Add the hash character `#` to the beginning of line) lines 
which respond to containers which you don't want to remove, 
and save and close the file.

You will confirm whether you remove containers.
If you answer `y`, containers will be removed.

> #### Notice
> If you don't edit the temporary file and close it, and answer the confirm "y", 
> all containers may be removed.


### dckrmi

`dckrmi` is very similar to `dckrm`.

## License

MIT License
