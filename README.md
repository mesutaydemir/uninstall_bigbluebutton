# Uninstall_bigbluebutton

To remove the packages just clone the `uninstall_package.py` file and run it as follows:
<pre>
apt install python3 -y
python3 uninstall_package.py
</pre>

<!--
~ To Delete Files That Are't Deleted 
<pre>
python3 resUn.py 
</pre>
#(not recomended because maybe some files still available)
<pre>
#Copy result from "python3 uninstall_package.py" and paste on dump.txt
cat dump.txt | grep "not removed" # and place on resUn.py
python3 resUn.py
</pre>
* OR Just-->

## Uninstall Apache2
```bash
apt --purge remove apache2-bin
```

## Downgrade nodejs to 16.14.2
```bash
cd ~
curl -sL https://deb.nodesource.com/setup_16.x | sudo bash -
sudo apt install curl
sudo apt-get install -y nodejs
npm install -g n
n 16.14.2
hash -r
node -v
```

## To Re-install the previous version
`wget -qO- https://ubuntu.bigbluebutton.org/bbb-install-2.5.sh | bash -s -- -v focal-250 -s vk.anadolu.edu.tr -e info@mail.com -a -w`
