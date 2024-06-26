@echo off
rem Cambiar directorio a donde se encuentra manage.py
cd /d "%~dp0\CatBeauty"

rem Instalar django
py -m pip install django

rem Instalar setuptools
py -m pip install setuptools

rem Instalar Pillow
py -m pip install pillow

rem Mostrar mensaje de instalación completada
echo Instalacion de bibliotecas completada.

echo - 

rem Mostrar credenciales de administrador
echo Credenciales de Admin:
echo Username: admin
echo Password: admin1234

echo -

rem Ejecutar el servidor
echo Iniciando servidor...
py manage.py runserver

rem Pausa para que el usuario pueda ver el resultado antes de que se cierre la ventana
pause
