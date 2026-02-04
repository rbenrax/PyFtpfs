# PyFtpfs
Python version of fuse ftpfs utlity

# Install dependencies
pip install fusepy

# Mount FTP (foreground modo to see logs)
python ftpfs.py ftp.miservidor.com /mnt/ftp -u usuario -P contraseña -f

# Or background mode
python ftpfs.py ftp.miservidor.com /mnt/ftp -u usuario -P contraseña

# To unmount
fusermount -u /mnt/ftp
