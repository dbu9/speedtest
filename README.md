# About

A simple way to test internet download speed.

# File generation

```bash
yes "Hello" | head -c 50M > 50mb.txt
```

# Speed test

```bash
wget -O /dev/null https://github.com/dbu9/speedtest/raw/master/100mb.txt -o test100.log
grep '/dev/null' test100.log
```

If your connection speed is high, the test will not reach the max because file of 100M is downloaded before peaking rate. Use some bigger file.
