# data-collection-rules

Disponible solo para VM, otras nubes o onpremise se usa a traves de Azure ARC

![](images\arch-general.png)

alta disponibilidad:

data almacenada en la region par
y en las tres zonas de disponibilidad en la region principal

partes:

fuentes de datos -> 
-   la fuente de datos se seleciona por tipo de SO


tipo de datos a recopilar
    - performance
    - eventos

destino de la informacion
	metrics
	workspace (debe estar en la misma locatizacion que la DCR)
	

tasK
-	automatizacion para el envio de rportes de costos de los recursos adicionados
-	crea por debajo una logic app


ejecucion de querys para la obtencion de resultados > se ejecutan sobre el workspace

![](images\workspace.png)

## Limites

![](.\images\limites-dcr.png)

## Agente instalado

azure monitor

![](.\images\agent.png)




## Referencias

- [data-collection-rule](https://docs.microsoft.com/en-us/azure/azure-monitor/agents/data-collection-rule-azure-monitor-agent)
- [azure cli commands](https://github.com/Azure/azure-cli-extensions/blob/main/src/monitor-control-service/README.md)
- Entendimiento de los tiempos de disponibilidad de la información [data-ingestion-time](https://docs.microsoft.com/en-us/azure/azure-monitor/logs/data-ingestion-time)