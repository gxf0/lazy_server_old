# lazy_deb

Basic Debian minimal, netinstall configuration

### Prerequisites

Don't forget to make the script executable.
```
chmod +x lazy_deb
```

### Optional Configure

You can define several variables at the beginning of the script.

```
serverip=$(ip route get 8.8.8.8 | awk 'NR==1 {print $NF}')
install_postfix="true"
```

### Script Options

```
./lazy_deb <option>

  -n  --nomail 	   don't install postifx
  -s  --screen		 show terminal output
  -x  --debug		   debug (dev-debug.log)
  -h  --help		   show this help
```

Examples:

Debug script :
```
 ./lazy_deb -x
 ./lazy_deb --debug
```

#### Author

* **Veit** - [gxf0](https://github.com/gxf0)

#### License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

#### Acknowledgments

* feel free to copy and adjust the scripts for your need
* feel free to improve the scripts - maybe you could also notice me - haha
* feel free to contact me, if you have any question