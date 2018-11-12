# Faster-related
Some notes and reminders

1. Using LabelImg https://github.com/tzutalin/labelImg to label bbox on image,
need install SIP4 http://pyqt.sourceforge.net/Docs/sip4/installation.html#ref-configuration-files and PyQt http://pyqt.sourceforge.net/Docs/PyQt4/installation.html first. 
Installation without root on Centos 7:

1) install sip:

wget https://sourceforge.net/projects/pyqt/files/sip/sip-4.19.13/sip-4.19.13.tar.gz
tar xzvf-sip-4.19.13.tar.gz
cd sip-4.19.13.tar.gz
python configure.py -b $HOME/local/bin -d $HOME/local/lib/python2.7/site-packages -e $HOME/local/include
make
make install

2)install PyQt:

wget https://sourceforge.net/projects/pyqt/files/PyQt4/PyQt-4.12.3/PyQt4_gpl_x11-4.12.3.tar.gz
tar xzvf-PyQt4_gpl_x11-4.12.3.tar.gz
cd PyQt4_gpl_x11-4.12.3
python configure.py --sip-module PyQt4.sip --no-dist-info --no-tools -b $HOME/local/bin -d $HOME/local/lib/python2.7/site-packages
make
make install

