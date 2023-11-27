# MACOS ansible_nodejs with vagrant and Parallels
NodeJs Test website with Ansible.

macOS: Sonoma 14.1.1

Vagrant Box: bento-rockylinux-9-aarch64

Parallels: 19.1.1

ATTENTION
1. If you are using bento-rockylinux-9-aarch64, remember to install firstly nodejs package (dnf) to use npm command in the future.
2. remote_src works only on EXTERNAL ENVIRONMENT, if you are using visual machine like me, don’t use it. (remote_scr=false default value)
3. Use physical path to copy files from your local machine, or u can add variable with your file path and use it this way.
4. Remember to specify good path to start node.js app

links: 2nd edition of Ansible for DevOps Jeff Geerling
