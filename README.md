# Non-root-users-to-use-pip

(1) Install Python

wget https://www.python.org/ftp/python/2.7.5/Python-2.7.5.tgz

tar -xzf Python-2.7.5.tgz

cd Python-2.7.5

mkdir -p /home/username/software/python27 

./configure --prefix="/home/username/software/python27"

make

make install

(2)Install setuptools

wget --no-check-certificate http://pypi.python.org/packages/source/s/setuptools/setuptools-2.0.tar.gz

tar -xzvf setuptools-2.0.tar.gz

cd setuptools-2.0

/home/username/software/python27/bin/python setup.py install

(3) Install pip

wget --no-check-certificate https://pypi.python.org/packages/41/27/9a8d24e1b55bd8c85e4d022da2922cb206f183e2d18fee4e320c9547e751/pip-8.1.1.tar.gz#md5=6b86f11841e89c8241d689956ba99ed7

tar -xzf pip-8.1.1.tar.gz

cd pip-8.1.1

/home/username/software/python27/bin/python setup.py install

(4)Try to install some libs:

cd /home/username/software/python27/bin/

./pip install selenium

./pip install bs4

