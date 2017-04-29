Debian-Go
=========

Go is an open source programming language that makes it easy to build simple, reliable, and efficient software.

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

go_version: "1.4.2"
go_os: "linux"
go_arch: "amd64"
go_root_path: "/usr/local"
go_path: "/usr/local/go/bin/go"

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: cowops.debian-go, go_version: "1.4.2", go_os: "linux", go_arch: "amd64", go_root_path: "/usr/local", go_path: "{{ go.root_path }}/go/bin/go" }

Tasks
-----

  - Install [Go](http://golang.org/) programming language

License
-------

BSD
