# clone
git clone --recursive https://github.com/mitenjain/signalAlign.git
which bwa
cp ~/bin/marginAlign/submodules/bwa/bwa ~/bin/anaconda/bin/
cd signalAlign/
virtualenv -p /path/to/python2.7 --no-site-packages --distribute env && source env/bin/activate && pip install -r requirements.txt

# compile
make
pip install -e .
./runSignalAlign 
cd bin 
./testSignalAlign 

