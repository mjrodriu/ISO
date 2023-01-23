# OPERACIONES BÁSICAS: 
* Listar todos los procesos
```PowerShell
Get-Process 
# también se puede usar PS (como alias)
```
* Mostrar los 5 primeros procesos
```PowerShell
PS | Select -first 5 
```
* Mostrar los 5 últimos procesos 
```PowerShell
PS | Select -Last 5 
```
* Agrupar los procesos y mostrar aquellos que sean empiecen por "sv", es decir, filtrar por nombre de manera más específica.
```PowerShell
PS -Name sv* | Group-Object
```
* Ordenar procesos por consumo de CPU de forma descendente 

```PowerShell
PS | Sort-Object -Descending CPU
```
