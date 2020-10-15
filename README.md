# Wrapper for File Browser

This project wraps [File Browser](https://filebrowser.org) for EmbassyOS.
File Browser is a file management interface that enables you to store, organize, edit, and share your files using a self-hosted solution.

## Dependencies

Install the following system dependencies to build this project by following the instructions on the provided links:

- [docker](https://docs.docker.com/get-docker)
- [docker-buildx](https://docs.docker.com/buildx/working-with-buildx/)
- [yq](https://mikefarah.gitbook.io/yq)
- [tiny-tmpl](https://github.com/Start9Labs/templating-engine-rs.git)
- [npm](https://www.npmjs.com/get-npm)
- [appmgr](https://github.com/Start9Labs/appmgr)
- [make](https://www.gnu.org/software/make/)

## Cloning

Clone the project locally. Note the submodule link to the original project. 

```
git clone git@github.com:Start9Labs/filebrowser-wrapper.git
cd filebrowser-wrapper
git submodule update --init
```

## Building

To build the project, run the following commands:

```
make
```

## Installing (on Embassy)

SSH into an Embassy device.
`scp` the `.s9pk` to any directory from your local machine.
Run the following command to determine successful install:

```
sudo appmgr install filebrowser.s9pk
```
