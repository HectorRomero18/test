@echo off
:: Navegar a la carpeta raíz del proyecto
cd /d "%~dp0"

:: Activar el entorno virtual de Python
call env\Scripts\activate

:: Entrar a la carpeta donde está el archivo main.py
cd backend

:: Ejecutar FastAPI desde la subcarpeta backend
uvicorn main:app --host 0.0.0.0 --port 8000

pause




### arrancar
Set WshShell = CreateObject("WScript.Shell")
WshShell.CurrentDirectory = "C:\Users\marlene.heredia\Desktop\CNEL ANALITYCS"
WshShell.Run "cmd /c activar_servidor.bat", 0, False
