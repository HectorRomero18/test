activar_servidor.bat
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



arrancar_oculto.vbs
Set WshShell = CreateObject("WScript.Shell")
WshShell.CurrentDirectory = "C:\Users\marlene.heredia\Desktop\CNEL ANALITYCS"
WshShell.Run "cmd /c activar_servidor.bat", 0, False




env: 

# Configuración del Servidor de Base de Datos SQL Server
DB_SERVER=MLGSRVSQL
DB_NAME=EEMCA
DB_USER=Consultas
DB_PASSWORD=Zeus2026
DB_DRIVER=ODBC Driver 17 for SQL Server

# Seguridad JWT
SECRET_KEY=d1d7aefde71dce24d8ac62f3ae49cd3192bf6f3cee487ae21273b7060fc5705c
ALGORITHM=HS256
ACCESS_TOKEN_EXPIRE_MINUTES=480


# --- 2. BASE DE DATOS LOCAL (Usuarios y Roles - ej. PostgreSQL o MySQL) ---
LOCAL_DB_HOST="localhost"
LOCAL_DB_PORT="5432"
LOCAL_DB_NAME="ZEUS"
LOCAL_DB_USER="postgres"
LOCAL_DB_PASSWORD="Milagro1"

## La otra contraseña posible es Zeus2026









# Configuración del Servidor de Base de Datos SQL Server
DB_SERVER=MLGSRVSQL
DB_NAME=EEMCA
DB_USER=Consultas
DB_PASSWORD=Zeus2026
DB_DRIVER=ODBC Driver 17 for SQL Server

# Seguridad JWT
SECRET_KEY=d1d7aefde71dce24d8ac62f3ae49cd3192bf6f3cee487ae21273b7060fc5705c
ALGORITHM=HS256
ACCESS_TOKEN_EXPIRE_MINUTES=480


# --- 2. BASE DE DATOS LOCAL (Usuarios y Roles - ej. PostgreSQL o MySQL) ---
# LOCAL_DB_HOST="localhost"
# LOCAL_DB_PORT="5432"
# LOCAL_DB_NAME="ZEUS"
# LOCAL_DB_USER="postgres"
# LOCAL_DB_PASSWORD="Milagro1"

## Base de datos en Render (PostgreSQL)
LOCAL_DB_HOST="dpg-db979c6k1f9s738mvda0-a.oregon-postgres.render.com"
LOCAL_DB_PORT="5432"
LOCAL_DB_NAME="zeus_c5o0"
LOCAL_DB_USER="consultas"
LOCAL_DB_PASSWORD="y6CiowQuJL02XoNFh2x4Np9Vr0fXyJBA"


# BASE DE DATOS EN RENDER mediante URL completa (opcional)
DATABASE_URL="postgresql+psycopg2://consultas:y6CiowQuJL02XoNFh2x4Np9Vr0fXyJBA@dpg-db979c6k1f9s738mvda0-a.oregon-postgres.render.com/zeus_c5o0"
## La otra contraseña posible es Zeus2026
