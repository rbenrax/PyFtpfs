# PyFtpfs
Python version of fuse ftpfs utlity

# Instalar dependencia
pip install fusepy

# Montar el FTP (modo foreground para ver logs)
python ftpfs.py ftp.miservidor.com /mnt/ftp -u usuario -P contraseña -f

# O en segundo plano
python ftpfs.py ftp.miservidor.com /mnt/ftp -u usuario -P contraseña

# Para desmontar
fusermount -u /mnt/ftp
