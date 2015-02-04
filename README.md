Dockerfile for Subversion
===

The simplest subversion server by `svnserve`.

## Usage with boot2docker

```sh
docker pull mookjp/subversion
docker run -d --name=svn-repo -p 3690:3690 -v $(pwd)/data
mookjp/subversion
cd your/work/dir
svn co svn://$(boot2docker ip)/ repo
```
