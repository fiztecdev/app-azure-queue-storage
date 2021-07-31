# app-azure-queue-storage

# Configuración y Creación Storage Account para Queue Storage:

Reemplazar YOUR_STORAGE_ACCOUNT por el nombre que asigne y sea unico de manera global, y también reemplazar YOUR_RESOURCE_GROUP por un nombre que asigne al resoource group disponibile:

1. Crear Storage Account via Azure CLI o Cloud Shell:
`az storage account create --name YOUR_STORAGE_ACCOUNT -g YOUR_RESOURCE_GROUP --kind StorageV2 --sku Standard_LRS`

1. Obtener la Cadena de Conexión:

`az storage account show-connection-string --name `az storage account create --name YOUR_STORAGE_ACCOUNT -g YOUR_RESOURCE_GROUP --kind StorageV2 --sku Standard_LRS`
 --resource-group YOUR_RESOURCE_GROUP`


3. Modificar la constante ConnectionString en Program.cs por el valor obtenido en el anterior comando ejecutado.


4. Ejecutar la applicación:

  - `dotnet build`
  - `dotnet run Send this message`